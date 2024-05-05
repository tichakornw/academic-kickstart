---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: 'TRELPy: Toolbox for Task-Relevant Evaluation of Perception'
subtitle: ''
summary: ''
authors:
- Ranai Srivastav
- Apurva Badithela
- Tichakorn Wongpiromsarn
- Richard M. Murray
tags: []
categories: []
date: '2024-04-30'
lastmod: 2024-04-30T15:47:16-05:00
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
publishDate: '2024-04-30T20:47:15.976388Z'
publication_types:
- 10
abstract: In safety-critical autonomous systems, deriving system-level guarantees requires evaluation of individual subsystems in a manner consistent with the system-level task. These safety guarantees require careful reasoning about how to evaluate each subsystem, and the evaluations have to be consistent with subsystem interactions and any assumptions made therein. A common example is the interaction between perception and planning. TRELPy is a Python-based toolbox that can evaluate the performance of perception models and leverage these evaluations in computing system-level guarantees via probabilistic model checking. The tool implements this framework for popular detection metrics such as confusion matrices, and implements new metrics such as proposition-labeled confusion matrices. The propositional formulae for the labels of the confusion matrix are chosen such that the confusion matrices are relevant to the downstream planner and system-level task. TRELPy can also group objects by egocentric distance or by orientation relative to the ego vehicle to further make the confusion matrix more task relevant. These metrics are leveraged to compute the combined performance of the perception and planner and calculate the satisfaction probability of system-level requirements.
publication: '*ICRA Workshop on How to Ensure Correct Robot Behaviors? Software Challenges in Formal Methods for Robotics*'
---
