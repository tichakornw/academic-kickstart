---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Formal Methods for Control Synthesis of Autonomous Systems"
event: "GALCIT Colloquium"
event_url: https://galcit.caltech.edu/events/88978
location: Caltech
address:
  street:
  city: Pasadena
  region: CA
  postcode:
  country: USA
summary:
abstract: " This talk provides an overview of practical applications of formal methods in the design of autonomous systems that are subject to complex rules. First, I will discuss the key assumptions and guarantees of different controller synthesis techniques for systems that are subject to temporal logic specifications, including closed system synthesis, probabilistic synthesis, and reactive synthesis.

The second part of the talk focuses on self-driving cars that are subject to potentially conflicting rules, i.e., there are situations where the rules cannot be simultaneously satisfied. In order to handle such situations, I will introduce the concept of prioritized safety specifications and a class of temporal logic formulas that is sufficiently expressive to describe many traffic rules. Then, I will present an efficient, incremental sampling-based algorithm to compute a trajectory that minimizes the amount of rule violation. By avoiding the conversion of specifications into finite automata, the algorithm allows temporal logic specifications to be handled with the same computational complexity as traditional motion planning algorithms such as RRT* and RRG.

Finally, I will wrap up the talk with a key bottleneck that prevents formal methods from realizing their full potential in the autonomous system domain---the (un)availability of formal specifications, which is a common, fundamental assumption all the temporal logic synthesis techniques rely on. I will discuss our early effort to partially address this problem and the remaining challenges."

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: 2020-10-30T15:00:00
date_end: 2020-10-30T16:00:00
all_day: false

# Schedule page publish date (NOT talk date).
publishDate: 2020-10-23T16:22:42-05:00

authors: []
tags: []

# Is this a featured talk? (true/false)
featured: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

# Optional filename of your slides within your talk's folder or a URL.
url_slides:

url_code:
url_pdf:
url_video:

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---
