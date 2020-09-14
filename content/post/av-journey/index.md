---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "The Journey of Autonomous Vehicles"
subtitle: "From the DARPA Challenges to the AV Industry"
summary: "A summary of technological progress and challenges over the past 10+ years."
authors: []
tags: []
categories: []
date: 2020-07-19T12:24:09-05:00
lastmod: 2020-07-19T12:24:09-05:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: ["darpa-urban-challenge"]
---

*Disclaimer: This post is based on my own opinion, which is not necessarily representative of the opinion of my previous and current employers.*

<!---
The history of autonomous vehicles dates back to at least the 1920s when Houdina Radio Control demonstrated a radio-controlled car driving through the streets of New York City.
-->
A series of Grand Challenges organized by DARPA in March 2004, October 2005, and November 2007 marked a major milestone in the history of autonomous vehicles as it attracted significant research attention and spurred rapid progress in this field.
The first two challenges featured a race of autonomous vehicles through a desert with dirt roads, cliffs, ditches, boulders, underpasses, open water, etc., as shown in the video below.
The vehicles were required to stay within a corridor specified in the <a href='https://archive.darpa.mil/grandchallenge05/RDDF_Document.pdf'>RDDF (Route Data Definition File)</a>, which was distributed to the teams 2 hours before the race, and contained a list of waypoint coordinates together with the associated corridor widths and speed limits.
The corridor was not guaranteed to be obstacle-free.
Thus, the vehicles had to be able to find a "road" (i.e., drivable, reasonably flat surface) and avoid obstacles, which were mostly static, with the exception of other autonomous vehicles competing in the race.

{{< youtube S4Ud7nYRwwQ >}}

<br />
The third race of the series, the DARPA Urban Challenge, shifted the focus to an urban environment, requiring the vehicles to execute a series of mock military supply missions while obeying California traffic laws, including lane keeping, merging, passing, negotiating intersections, making U-turns, parking, and avoiding obstacles.
As in the previous two races, the vehicles were fully autonomous.
No humans were allowed inside the vehicles.
Any communication to and from the vehicles was also prohibited.
The only possible intervention was through a <a href='https://archive.darpa.mil/grandchallenge05/Estop_Guidance.pdf'>wireless emergency stop safety system (E-stop)</a>, which was operated by DARPA to pause or completely disable the vehicle in case of emergency.

**The development timeframe:**
The Urban Challenge was announced in May 2006.
The teams had to go through the qualification process, including the site visit (June--July 2007) and the National Qualification Event (NQE, 26--31 October 2007) before proceeding to the Urban Challenge Final Event (UFE, 3 November 2007).
This gave each team about 1 year to implement the *Basic Navigation* and *Basic Traffic* functionalities required for the site visit as described in the <a href='https://www.grandchallenge.org/grandchallenge/docs/Technical_Evaluation_Criteria_031607.pdf'>Technical Evaluation Criteria</a>, after which the team had about 6 more months to implement the advanced functionalities required for both the NQE and the UFE such as navigating obstacle fields, parking lots, and partially blocked intersections, handling road blockages, merging into moving traffic, and performing an evasive maneuver by pulling to the side to avoid head-on collisions.

**The race:** The specific location (George Air Force Base, Victorville, CA) of the NQE and UFE was kept secret until August 2007, less than 3 months before the NQE.
Furthermore, the teams did not have access to the site, so it was not possible to build a prior, HD map that most autonomous vehicles these days rely on.

DARPA used two file formats to describe a mission: <a href='https://www.grandchallenge.org/grandchallenge/docs/RNDF_MDF_Formats_031407.pdf'>the Route Network Definition File (RNDF) and the Mission Data File (MDF)</a>.
The RNDF was basically a digital street map, which specified accessible road segments and free-travel zones <!--- (i.e., areas within which the vehicles can move freely) -->
and provided information such as waypoints, checkpoints, parking spots, stop signs, lane widths, lane boundaries, connections between lanes, zone boundaries, and entry and exit points to each zone.
Although the RNDF was reasonably accurate, it had 3 key limitations.
First, even though the waypoints were guaranteed to be within their associated lanes, a straight line connecting them might go off road.
Second, connectivity of waypoints was not guaranteed as the road could be completely or partially blocked.
Finally, part of the zones might not be drivable.

The MDF specified the sequence of checkpoints to be visited by the vehicle as well as the minimum and maximum speed limits for each segment in the RNDF.
The mission length and complexity varied in different runs.
In particular, the UFE was split into 3 missions, covering the total of approximately 60 miles, and consisting of interactions with both human-driven vehicles and other autonomous vehicles.
The objective of the vehicles was to complete the missions as quickly as possible while satisfying all the rules specified in the <a href='https://www.grandchallenge.org/grandchallenge/docs/Technical_Evaluation_Criteria_031607.pdf'>Technical Evaluation Criteria</a>.
Any infraction of the rules could lead to time penalties or disqualification.
(However, as far as I know, the specific penalty for each violation was not provided before the race.)

While the RNDF was provided at least 24 hours in advance, the MDF was given to the team right before each run.
After receiving the MDF, the team had only 5 minutes to load it and get the vehicle ready in autonomous mode to begin the run.

The video below was taken from a camera mounted on Team Caltech's vehicle, Alice, during one of the tests in the NQE and illustrated the maneuvers required by the *Basic Navigation* functionality.
In fact, around the 34th second, Alice was paused as it was heading towards a concrete barrier.
DARPA then asked the team whether to let her continue the mission, a decision that was very difficult to make without any access to the vehicle---we did not even know whether the sensors or the computers were still running.
We decided to take the risk, and Alice successfully completed the mission with quite a bit of difficulty to satisfy the obstacle clearance requirement due to her size.

{{< youtube 1eZdc1hsBkU >}}

<br />
**Key technological development:**
<a href='https://royalsocietypublishing.org/doi/pdf/10.1098/rsta.2010.0110'>The article by Campbell et al.</a> provides a very good description of approaches and challenges faced by different teams (Cornell, Georgia Tech, MIT, and Caltech).
In summary, most vehicles consisted of 4 main components: sensing, perception (+ localization), planning, and control.
The key sensors included GPS, IMU, odometry, lidar, radar, and cameras.
The perception component used the measurements from these sensors to localize the vehicle within the map, detect and track objects and relevant features (e.g., road, lane marking, stop lines, etc.), and create a representation of the world around the vehicle.
The planning component used this information to compute a trajectory (path + speed) for the vehicle to follow.
Finally, the control component sent actuation commands (brake, throttle, steering, gear shifting) to keep the vehicle on the trajectory.

The 18-month timeframe was quite short for any new technological development, especially as many teams consisted mainly of students, who also had to worry about classes and exams.
So, the effort was mainly directed towards putting together and extending existing approaches, rather than inventing radically new ones. <!--- (This is quite an over-simplistic statement as it still took a lot of effort to figure out how to get things to work robustly together.) -->
Perhaps, a key exception to this statement was the Velodyne’s HDL-64E sensor, which was used by 5 out of the 6 vehicles that finished the race, and was an essential technology emerging from the Challenge.
This spinning lidar and its successors, including the more affordable models with 16 and 32 beams and the high-end models with 128 beams, became a key component of many autonomous vehicles nowadays.

While the architectures and algorithms of the perception subsystem varied greatly among different teams, a more common structure was observed in the planning and control subsystems.
In particular, the planning subsystem was typically decomposed into 3 levels---the mission planner, the behavioral planner, and the trajectory planner---although the name and detail of responsibilities and algorithms used in each level varied.
Roughly, the mission planner computed a high-level route for the vehicle to complete the mission.
The behavioral planner was responsible for making local decisions (e.g., whether to stay in lane, proceed through an intersection, etc.) and typically implemented as a finite-state machine.
The trajectory planner then translated the decision into a trajectory for the vehicle to follow, using variations of optimization-based (e.g., MPC) and graph-based (e.g., RRT, PRM) approaches. <!--- with graphs constructed based on variations of RRT and PRM algorithms or directly from RNDF -->
Most vehicles employed different trajectory planners for different driving situations.
Finally, the controller was typically based on pure pursuit and PID.
More details about planning and control algorithms can be found in <a href='https://arxiv.org/pdf/1604.07446.pdf'>the article by Paden et al.</a>

**Major technological challenges:**
The Urban Challenge expanded the scientific community's exposure to the complexity of designing safety-critical autonomous systems.
Not only the challenges associated with individual components (perception, planning, control, contingency management, etc.)
but also their integration needed to be addressed.
In particular, subtle design bugs may arise from the unforeseen interactions among different components
and manifest as undesirable behavior only under a very specific set of conditions,
making them very hard to catch using simulation and testing.
For example, consider the following components, which were implemented on Alice:
1. the path planner, which generated a path for Alice to follow,
2. the safety system, which rapidly decelerated the vehicle when it deviated too much from the planned path and got too close to an obstacle, and
3. the low-level steering controller, which limited the steering rate at low speeds to protect the vehicle steering system.

Each of these functionalities seemed reasonable by itself.
However, when combined together, they led to an unsafe behavior under a very specific circumstance where
Alice had to make a tight turn while merging into traffic,
with a concrete barrier next to the major road.
In this case, the planned path contained a sharp turn.
Accelerating from a low speed, the controller was unable to execute the turn closely due to the limited steering rate.
As a result, Alice deviated from the path and headed towards the concrete barrier; the safety system activated and slowed it down, leading to an even stricter limit on the steering rate.
This cycle continued, causing Alice to be stuck at the corner of a sharp turn,
dangerously stuttering in the middle of an intersection.

In short, I think the key technical challenges evolved around the following factors:
uncertainties, complex tasks, and interconnection of computing, communication, and physical components.
The uncertain and unstructured nature of environments led to an unreasonably large number of test scenarios and drove the question of edge cases.
The complex interaction of different components caused any change in one component to potentially affect the others in an unexpected way.
Finally, complex tasks were primarily handled by handcrafted finite state machines,
which ended up hosting several hacks to handle corner cases encountered during testing.
In particular, Alice's behavioral planner was initially implemented as a finite state machine with less than 5 states,
but it quickly turned into 3 interacting finite state machines, each containing more than 20 states,
making it almost impossible to analyze or debug.


**AV industry, key enablers, and challenges:**
Google pioneered the AV industry with the Google X's Project Chauffeur (now Waymo) in 2009.
Several years later, many startups were founded, including Cruise (founded in 2013, acquired by GM in 2016), nuTonomy (founded in 2013, acquired by Aptiv in 2017), Zoox (founded in 2014, acquired by Amazon in 2020), Drive.ai (founded in 2015, acquired by Apple in 2019), Argo AI (founded in 2016), Pony.ai (founded in 2016), and Aurora (founded in 2017), just to name a few.
<a href='https://spectrum.ieee.org/transportation/self-driving/surprise-2020-is-not-the-year-for-selfdriving-cars'>Early predictions</a> indicated that autonomous vehicles would be ready to roam the streets in 2020.

The hype of the industry was primarily driven by several technological advances that were not sufficiently mature at the time of the Urban Challenge---the most notable one being deep learning, which has become a core part of most state-of-the-art object classification and intent prediction algorithms.
Some companies went further and adopted end-to-end learning that directly maps raw sensor data to vehicle actuation commands.

Other relevant technologies include <a href='https://en.wikipedia.org/wiki/Simultaneous_localization_and_mapping'>SLAM (simultaneous localization and mapping)</a>,
which is often used to generate a pre-built map and enables accurate map-based localization.
Advances in optimization-based control, particularly <a href='https://en.wikipedia.org/wiki/Model_predictive_control'>model predictive control (MPC)</a>,
allow real-time computation of control signals with complex nonlinear cost functions.
New planning algorithms such as <a href='https://en.wikipedia.org/wiki/Rapidly-exploring_random_tree'>RRT*</a> provide asymptotic optimality guarantee.
Finally, <a href='https://en.wikipedia.org/wiki/Formal_methods'>formal methods</a> eliminate the need of handcrafted finite state machines and enable complex tasks to be handled in a provably correct way.

Many of the aforementioned algorithms have been implemented in open-source software such as
<a href='https://www.tensorflow.org/'>TensorFlow</a>,
<a href='https://pytorch.org/'>PyTorch</a>,
<a href='https://www.ros.org/'>ROS</a>, and
<a href='https://ompl.kavrakilab.org/'>OMPL</a>.
In fact, one can build an autonomous vehicle out of open-source software,
and it might already handle most of the "nominal" scenarios.
These technological advances greatly simplify the initial phase of building autonomous vehicles,
making the estimate of their arrival to market overly optimistic.
(Recall that it took a team of mostly students only a year to make a vehicle drive itself
for the DARPA Urban Challenge when most of these technologies and open-source software did not even exist.)

Unfortunately, the number of off-nominal cases, as well as their complexity, may have been underappreciated.
Additionally, in many situations, it is not even clear how the vehicle should behave as there are no
<a href='https://archive.darpa.mil/grandchallenge/docs/Technical_Evaluation_Criteria_031607.pdf'>precisely defined rules as in the DARPA Urban Challenge</a>.

An <a href='https://trid.trb.org/view/1727480'>article from MIT task force</a> (<a href='https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwjWraHgz-frAhWFcc0KHWxKCBwQFjAAegQIAxAB&url=https%3A%2F%2Fouravfuture.org%2Fwp-content%2Fuploads%2F2020%2F08%2FWotF-2020-Research-Brief-Leonard-Mindell-Stayton.pdf&usg=AOvVaw2JXuYPKeoGd7uCEC7gfyhE'>pdf</a>) predicts that deployment of fully automated driving systems that have no safety driver onboard will take at least a decade. Additionally, expansion will likely be gradual and will happen region-by-region in specific categories of transportation, resulting in wide variations in availability across the country.

I feel extremely privileged to be a part of this exciting journey from its early days.
Autonomous vehicles, and more generally autonomous systems, will remain an active area of research and new ideas will be needed to bring this journey through the last mile.
