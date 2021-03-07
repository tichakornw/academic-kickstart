---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: 'The Reasonable Crowd: Towards evidence-based and interpretable models of driving
  behavior'
subtitle: ''
summary: ''
authors:
- Bassam Helou
- Aditya Dusi
- Anne Collin
- Noushin Mehdipour
- Zhiliang Chen
- Cristhian Lizarazo
- Calin Belta
- Tichakorn Wongpiromsarn
- Radboud Duintjer Tebbens
- Oscar Beijbom
tags: []
categories: []
date: '2021-01-01'
lastmod: 2021-03-06T21:29:33-06:00
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
publishDate: '2021-03-07T03:29:33.236138Z'
publication_types:
- 9
abstract: Autonomous vehicles must balance a complex set of objectives. There is no
  consensus on how they should do so, nor on a model for specifying a desired driving
  behavior. We created a dataset to help address some of these questions in a limited
  operating domain. The data consists of 92 traffic scenarios, with multiple ways
  of traversing each scenario. Multiple annotators expressed their preference between
  pairs of scenario traversals. We used the data to compare an instance of a rulebook,
  carefully hand-crafted independently of the dataset, with several interpretable
  machine learning models such as Bayesian networks, decision trees, and logistic
  regression trained on the dataset. To compare driving behavior, these models use
  scores indicating by how much different scenario traversals violate each of 14 driving
  rules. The rules are interpretable and designed by subject-matter experts. First,
  we found that these rules were enough for these models to achieve a high classification
  accuracy on the dataset. Second, we found that the rulebook provides high interpretability
  without excessively sacrificing performance. Third, the data pointed to possible
  improvements in the rulebook and the rules, and to potential new rules. Fourth,
  we explored the interpretability vs performance trade-off by also training non-interpretable
  models such as a random forest. Finally, we make the dataset publicly available
  to encourage a discussion from the wider community on behavior specification for
  AVs.
publication: '*2021 IEEE/RSJ International Conference on Intelligent Robots and Systems
  (IROS)*'
---
