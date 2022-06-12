---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: Temporal Shift Reinforcement Learning
subtitle: ''
summary: ''
authors:
- Deepak George Thomas
- Tichakorn Wongpiromsarn
- Ali Jannesari
tags:
- '"sample efficiency"'
- '"deep reinforcement learning"'
categories: []
date: '2022-04-05'
lastmod: 2022-06-12T12:49:50-05:00
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
projects: [correctness-autonomy]
publishDate: '2022-06-12T17:49:50.530258Z'
publication_types:
- 1
abstract: The function approximators employed by traditional image-based Deep Reinforcement
  Learning (DRL) algorithms usually lack a temporal learning component and instead
  focus on learning the spatial component. We propose a technique, Temporal Shift
  Reinforcement Learning (TSRL), wherein both temporal, as well as spatial components
  are jointly learned. Moreover, TSRL does not require additional parameters to perform
  temporal learning. We show that TSRL outperforms the commonly used frame stacking
  heuristic on all of the Atari environments we test on while beating the SOTA for
  all except one of them. This investigation has implications in the robotics as well
  as sequential decision-making domains. Our code is available at - https://github.com/Deepakgthomas/TSM_RL
publication: '*Proceedings of the 2nd European Workshop on Machine Learning and Systems*'
doi: 10.1145/3517207.3526968
---
