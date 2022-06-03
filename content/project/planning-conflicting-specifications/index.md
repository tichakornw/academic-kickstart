---
title: Planning with Conflicting Specifications
summary: Develop planning and decision-making algorithms with multiple, potentially conflicting objectives.
tags:
- Autonomy
- Formal methods
- Motion planning
- Past projects
date: "2020-01-01T00:00:00Z"

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

Autonomous systems may be subject to several requirements. Consider, as an example, autonomous vehicles that need to follow the road rules. Often, these rules cannot be simultaneously satisfied. For instance, when encoutering a vehicle that is (improperly) parked next to the solid line, an autonomous vehicle may need to violate the lane keeping rule (which prohibits the vehicle from crossing solid lane boundary) or the obstacle clearance rule (which requires the vehicle to keep some safety gap when passing a parked vehicle). Another example is the [trolley problem](https://en.wikipedia.org/wiki/Trolley_problem) where autonomous systems need to choose which safety requirements to violate. More complications arise when taking into account uncertainties, e.g., in perception, prediction, control, etc.

The goal of this project is to develop planning and decision-making algorithms for systems that are subject to multiple, potentially conflicting objectives. These objectives may be represented by a combination of cost functions (e.g., control efforts) and temporal logic formulas (e.g., rules of the road), with associated violation metrics.