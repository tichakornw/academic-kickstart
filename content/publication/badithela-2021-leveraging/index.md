---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: Leveraging Classification Metrics for Quantitative System-Level Analysis with
  Temporal Logic Specifications
subtitle: ''
summary: ''
authors:
- Apurva Badithela
- Tichakorn Wongpiromsarn
- Richard M. Murray
tags: []
categories: []
date: '2021-03-25'
lastmod: 2021-03-26T14:46:30-05:00
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
projects: []
publishDate: '2021-03-26T19:46:29.970236Z'
publication_types:
- 1
abstract: In many autonomy applications, performance of perception algorithms is important
  for effective planning and control. In this paper, we introduce a framework for
  computing the probability of satisfaction of formal system specifications given
  a confusion matrix, a statistical average performance measure for multi-class classification.
  We define the probability of satisfaction of a linear temporal logic formula given
  a specific initial state of the agent and true state of the environment. Then, we
  present an algorithm to construct a Markov chain that represents the system behavior
  under the composition of the perception and control components such that the probability
  of the temporal logic formula computed over the Markov chain is consistent with
  the probability that the temporal logic formula is satisfied by our system. We illustrate
  this approach on a simple example of a car with pedestrian on the sidewalk environment,
  and compute the probability of satisfaction of safety requirements for varying parameters
  of the vehicle. We also illustrate how satisfaction probability changes with varied
  precision and recall derived from the confusion matrix. Based on our results, we
  identify several opportunities for future work in developing quantitative system-level
  analysis that incorporates perception models.
publication: '*Proceedings of the 60th IEEE Conference on Decision and Control (CDC)*'

url_pdf: https://arxiv.org/abs/2105.07343
---
