---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: Quantifying Faulty Assumptions in Heterogeneous Multi-Agent Systems
subtitle: ''
summary: ''
authors:
- Steven Carr
- Tichakorn Wongpiromsarn
- Ufuk Topcu
tags: []
categories: []
date: '2023-01-01'
lastmod: 2023-06-21T21:30:08-05:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: ["inconsistencies"]
publishDate: '2023-06-22T02:30:08.809676Z'
publication_types:
- 1
abstract: We study the problem of analyzing the effects of inconsistencies in perception,
  intent prediction, and decision making among interacting agents. When accounting
  for these effects, planning is akin to synthesizing policies in uncertain and potentially
  partially-observable environments. We consider the case where each agent, in an
  effort to avoid a difficult planning problem, does not consider the inconsistencies
  with other agents when computing its policy. In particular, each agent assumes that
  other agents compute their policies in the same way as it does, i.e., with the same
  objective and based on the same system model. While finding policies on the composed
  system model, which accounts for the agent interactions, scales exponentially, we
  efficiently provide quantifiable performance metrics for them using probabilistic
  model checking. We showcase our approach using two realistic autonomous vehicle
  case-studies and implement it in an autonomous vehicle simulator.
publication: '*2023 7th IEEE Conference on Control Technology and Applications (CCTA)*'

url_video: https://youtu.be/yrHslmGohek
---
