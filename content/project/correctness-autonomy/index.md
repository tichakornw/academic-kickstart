---
title: "CAREER: Establishing Correctness of Learning-Enabled Autonomous Systems with Conflicting Requirements (NSF)"
summary: Develop specification formalisms, control synthesis algorithms, and quantitative verification frameworks for autonomous systems that include learning-based components, operate in uncertain environments, and are subject to conflicting requirements with partially established priorities.
tags:
- Autonomy
- Formal methods
- Specifications
- Motion planning
- Current projects
date: "2022-02-15T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: ""
  focal_point: Smart

links:
#- icon: linkedin
#  icon_pack: fab
#  url: https://www.linkedin.com/in/tichakorn-wongpiromsarn-3a9b2782/
#  name: Follow
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

**Award Number:** CNS-2141153<br />
**Amount:** 502,352<br />
**Start Date:** 02/15/2022<br />
**End Date:** 01/31/2027<br />

Autonomous systems are subject to multiple regulatory requirements due to their safety-critical nature. In general, it is infeasible to guarantee the satisfaction of all requirements under all conditions. In such situations, the system needs to decide how to prioritize among them. Two main factors complicate this decision. First, the priorities among the conflicting requirements may not be fully established. Second, the decision needs to be made under uncertainties arising from both the learning-based components within the system and the unstructured, unpredictable, and non-cooperating nature of the environments. Therefore, establishing the correctness of autonomous systems requires specification languages that capture the unequal importance of the requirements, quantify the violation of each requirement, and incorporate uncertainties faced by the systems.

The proposed effort targets a major gap in theoretical foundations and computational tools to enable practical applications of formal methods throughout the development process of autonomous systems that include learning-based components, operate in uncertain environments, and are subject to conflicting requirements with partially established priorities. Its key novelty lies in the development of (1) probabilistic rulebooks, a new specification formalism that captures the tradeoffs between the uncertainty and the degree of violation of the requirements and utilizes such violation risk together with partially established priorities among the requirements to establish a consistent order among the trajectories of the system, (2) minimum-violation control synthesis algorithms that minimize the total violation risk based on the probabilistic rulebooks and allow learning-based functionality to be incorporated in a provably correct manner, and (3) quantitative verification frameworks that utilize statistical analysis of the learning-based components and the environment as well as the probabilistic rulebooks to provide quantitative analysis of the system. Such development will serve as a critical step towards establishing assurance of autonomous systems. This project will validate the theoretical results and algorithms developed under the proposed effort on a small autonomy platform that will also be utilized for educational purposes.
