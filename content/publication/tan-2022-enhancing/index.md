---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: Enhancing System-level Safety in Autonomous Driving via Feedback Learning
subtitle: ''
summary: ''
authors:
- Sin Yong Tan
- Weisi Fan
- Qisai Liu
- Tichakorn Wongpiromsarn
- Soumik Sarkar
tags: []
categories: []
date: '2022-01-01'
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
projects: ["correctness-autonomy"]
publishDate: '2023-06-22T02:30:08.882372Z'
publication_types:
- 1
abstract: The perception component of autonomous driving systems is often designed
  and tuned in isolation from the control component based on well-known performance
  measures such as accuracy, precision, and recall. Commonly used loss functions such
  as cross-entropy loss and negative log-likelihood only focus on minimizing the loss
  with respect to misclassification without considering the consequences that follow
  after the misclassifications. In other words, this approach fails to take into account
  the difference in the severity of system-level failures due to misclassification
  and other errors in perception components. Therefore in this work, we proposed a
  novel feedback learning training framework to build the perception component of
  an autonomous system that is aware of system-level safety objectives, which in turn,
  enhances the safety of the vehicle as a whole. The crux of the idea is to utilize
  the concept of a rulebook to provide feedback on system-level performance as safety
  scores and leverage them in designing and computing the loss functions for the models
  in the framework. The framework was trained and tested on an open-sourced dataset,
  and the experimental results showed that the resulting model had shown superior
  system-level safety performance over the baseline perception model.
publication: '*NeurIPS 2022 Workshop on Machine Learning for Autonomous Driving*'
---
