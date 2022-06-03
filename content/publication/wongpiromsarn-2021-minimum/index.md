---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: 'Minimum-Violation Planning for Autonomous Systems: Theoretical and Practical
  Considerations'
subtitle: ''
summary: ''
authors:
- Tichakorn Wongpiromsarn
- Konstantin Slutsky
- Emilio Frazzoli
- Ufuk Topcu
tags: []
categories: []
date: '2021-01-01'
lastmod: 2020-09-27T20:42:08-05:00
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
projects: ["planning-conflicting-specifications"]
publishDate: '2020-09-28T01:42:07.986741Z'
publication_types:
- 1
abstract: This paper considers the problem of computing an optimal trajectory for
  an autonomous system that is subject to a set of potentially conflicting rules.
  First, we introduce the concept of prioritized safety specifications, where each
  rule is expressed as a temporal logic formula with its associated weight and priority.
  The optimality is defined based on the violation of such prioritized safety specifications.
  We then introduce a class of temporal logic formulas called si-FLTLGX and develop
  an efficient, incremental sampling-based approach to solve this minimum-violation
  planning problem with guarantees on asymptotic optimality. We illustrate the application
  of the proposed approach in autonomous vehicles, showing that si-FLTLGX formulas
  are sufficiently expressive to describe many traffic rules. Finally, we discuss
  practical considerations and present simulation results for a vehicle overtaking
  scenario.
publication: '*2021 American Control Conference*'

links:
- name: "full version"
  url: wongpiromsarn-2021-minimum-full.pdf
---
