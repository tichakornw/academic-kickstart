---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: Parallelized Outlook Graphs for Multi-Objective Optimal Path Planning
subtitle: ''
summary: ''
authors:
- Keivan Sabet
- Tichakorn Wongpiromsarn
tags: []
categories: []
date: '2024-03-31'
lastmod: 2024-03-31T15:47:15-05:00
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
publishDate: '2024-03-31T20:47:15.899945Z'
publication_types:
- 9
abstract: Finding a path to optimally balance several objectives, known as the Multi-Objective Optimal Path Planning (MOPP) problem, frequently manifests an NP-Hard problem that impacts several domains, including robotics. Systems, like autonomous vehicles, need to compute paths that balance several, often conflicting criteria, and the inherent complexity of MOPP leads to the open question of how to address it. We introduce an approach that efficiently explores the search space of a given MOPP problem and uses information obtained from the exploration to find a path with an informed search strategy. The approach uses multi-threading to simultaneously explore individual objectives and find paths that reduce the cost of an objective. Exploring ultimately leads to the creation of a model we call an Optimistic Outlook Graph (OOG). An OOG estimates the optimal cost for a solution if an edge is chosen to be part of the solution. We investigate how well an OOG can inform a search by examining the performance of Dijkstra’s algorithm enhanced with an OOG. Our results show that the time needed to create an OOG is fast enough for real-time path planning to be viable, and using an OOG improves Dijkstra’s ability to make decisions and returns better paths compared to standard Dijkstra's algorithm.
publication: '*2024 IEEE/RSJ International Conference on Intelligent Robots and Systems
  (IROS)*'
---
