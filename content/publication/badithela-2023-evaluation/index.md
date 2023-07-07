---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: Evaluation Metrics for Object Detection for Autonomous Systems
subtitle: ''
summary: ''
authors:
- Apurva Badithela
- Tichakorn Wongpiromsarn
- Richard M. Murray
tags: []
categories: []
date: '2023-01-01'
lastmod: 2022-10-17T16:32:14-05:00
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
publishDate: '2022-10-17T21:32:14.900008Z'
publication_types:
- 10
abstract: This paper studies the evaluation of learning-based object detection models
  in conjunction with model-checking of formal specifications defined on an abstract
  model of an autonomous system and its environment. In particular, we define two
  metrics -- emphproposition-labeled and emphclass-labeled confusion matrices -- for
  evaluating object detection, and we incorporate these metrics to compute the satisfaction
  probability of system-level safety requirements. While confusion matrices have been
  effective for comparative evaluation of classification and object detection models,
  our framework fills two key gaps. First, we relate the performance of object detection
  to formal requirements defined over downstream high-level planning tasks. In particular,
  we provide empirical results that show that the choice of a good object detection
  algorithm, with respect to formal requirements on the overall system, significantly
  depends on the downstream planning and control design. Secondly, unlike the traditional
  confusion matrix, our metrics account for variations in performance with respect
  to the distance between the ego and the object being detected. We demonstrate this
  framework on a car-pedestrian example by computing the satisfaction probabilities
  for safety requirements formalized in Linear Temporal Logic (LTL).
publication: '*2023 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)*'
---
