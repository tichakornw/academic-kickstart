---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: 'Locally Homotopic Paths: Ensuring Consistent Paths in Hierarchical Path Planning'
subtitle: ''
summary: ''
authors:
- Tichakorn Wongpiromsarn
- Marcelo Kallmann
- Andreas Kolling
tags: []
categories: []
date: '2024-02-15'
lastmod: 2024-02-15T15:47:15-05:00
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
publishDate: '2024-02-15T20:47:15.553592Z'
publication_types:
- 2
abstract: We consider a local planner that utilizes model predictive control   to locally deviate from a prescribed global path in response to dynamic environments, taking into account the system dynamics. To ensure the consistency between the local and global paths, we introduce the concept of locally homotopic paths for paths with different origins and destinations. We then formulate a hard constraint to ensure that local paths are locally homotopic to a given global path. Additionally, we propose a cost function to penalize any violation of this requirement, rather than completely prohibiting it. Experimental results show that both variants of our approach are more resilient to localization errors, compared to existing methods that represent the homotopy class constraint as an envelope around the global path.
publication: '*IEEE Robotics and Automation Letters (RAL)*'

url_pdf: https://www.amazon.science/publications/locally-homotopic-paths-ensuring-consistent-paths-in-hierarchical-path-planning
---
