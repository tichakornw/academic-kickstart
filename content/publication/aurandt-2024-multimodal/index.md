---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: Multimodal Model Predictive Runtime Verification for Safety of Autonomous Cyber-Physical
  Systems
subtitle: ''
summary: ''
authors:
- Alexis Aurandt
- Phillip H. Jones
- Kristin Yvonne Rozier
- Tichakorn Wongpiromsarn
tags: []
categories: []
date: '2024-04-15'
lastmod: 2024-04-15T15:47:16-05:00
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
projects: [runtime-verification]
publishDate: '2024-04-15T20:47:16.051692Z'
publication_types:
- 9
abstract: Autonomous cyber-physical systems must be able to operate safely in a wide range of complex environments. To ensure safety without limiting mitigation options, these systems require detection of safety violations by mitigation trigger deadlines. As a result of these system's complex environments, multimodal prediction is often required. For example, an autonomous vehicle (AV) operates in complex traffic scenes that result in any given vehicle having the ability to exhibit several plausible future behavior modes (e.g., stop, merge, turn, etc.); therefore, to ensure collision avoidance, an AV must be able to predict the possible multimodal behaviors of nearby vehicles. In previous work, model predictive runtime verification (MPRV) successfully detected future violations by a given deadline, but MPRV only considers a single mode of prediction (i.e., unimodal prediction). We design multimodal model predictive runtime verification (MMPRV) to extend MPRV to consider multiple modes of prediction, and we introduce Predictive Mission-Time Linear Temporal Logic (PMLTL) as an extension of MLTL to support the evaluation of probabilistic multimodal predictions. We examine the correctness and real-time feasibility of MMPRV through two AV case studies where MMPRV utilizes (1) a physics-based multimodal predictor on the F1Tenth autonomous racing vehicle and (2) current state-of-the-art deep neural network multimodal predictors trained and evaluated on the Argoverse motion forecasting dataset. We found that the ability to meet real-time requirements was a challenge for the latter, especially when targeting an embedded computing platform.

publication: '*26th International Symposium on Formal Methods*'
---
