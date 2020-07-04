---
title: Temporal Logic Planning (TuLiP) Toolbox
summary: A Python-based software toolbox for the synthesis of embedded control software that is provably correct with respect to an expressive subset of linear temporal logic (LTL) specifications.
tags:
- Formal methods
- Hybrid systems
- Software tools
date: "2020-07-02T00:00:00Z"

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
url_code: "https://github.com/tulip-control/tulip-control"
url_pdf: ""
url_slides: "slides/tulip.pdf"
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

The Temporal Logic Planning (TuLiP) Toolbox is a Python-based software toolbox for the synthesis of embedded control software that is provably correct with respect to an expressive subset of linear temporal logic (LTL) specifications. TuLiP combines routines for (1) finite state abstraction of control systems, (2) digital design synthesis from LTL specifications, and (3) receding horizon planning. The underlying digital design synthesis routine treats the environment as adversary; hence, the resulting controller is guaranteed to be correct for any admissible environment profile. TuLiP applies the receding horizon framework, allowing the synthesis problem to be broken into a set of smaller problems, and consequently alleviating the computational complexity of the synthesis procedure, while preserving the correctness guarantee.