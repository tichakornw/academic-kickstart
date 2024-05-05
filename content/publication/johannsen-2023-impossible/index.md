---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: 'Impossible Made Possible: Encoding Intractable Specifications via Implied
  Domain Constraints'
subtitle: ''
summary: ''
authors:
- Chris Johannsen
- Brian Kempa
- Phillip H. Jones
- Kristin Y. Rozier
- Tichakorn Wongpiromsarn
tags: []
categories: []
date: '2023-01-01'
lastmod: 2024-05-05T15:47:16-05:00
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
publishDate: '2024-05-05T20:47:16.131906Z'
publication_types:
- 1
abstract: We take another look at intractable temporal logic specifications, where the intractability stems from self-reference, unboundedness, or the need for explicit counting. A classic example is the specification, Every file that gets opened eventually gets closed. In all cases, we show that we can capitalize on realistic constraints implied by the operating environment to generate Mission-time Linear Temporal Logic (MLTL) encodings with reasonably-sized memory signatures. We derive a new set of rewriting rules for MLTL, accompanied by proofs of correctness for each rule, and memory optimizations. We utilize these in creating MLTL encodings for all three patterns of intractability, proving correctness, time complexity, and space complexity for each type of specification encoding.
publication: '*28th International Conference on Formal Methods for Industrial Critical Systems (FMICS)*'
---
