---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: 'MLTL Multi-type: A Typed Logic for Cyber-Physical Systems'
subtitle: ''
summary: ''
authors:
- Gokul Hariharan
- Brian C. Kempa
- Tichakorn Wongpiromsarn
- Phillip H. Jones
- Kristin Y. Rozier
tags: []
categories: []
date: '2024-01-31'
lastmod: 2024-01-31T15:47:15-05:00
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
publishDate: '2024-01-31T20:47:15.738284Z'
publication_types:
- 9
abstract: Modern cyber-physical systems (CPS) operate in complex systems-of-systems that must seamlessly work together to control safety-or mission-critical functions. Linear Temporal Logic (LTL) and Mission-time Linear Temporal logic (MLTL) intuitively express CPS requirements for automated system verification and validation. However, both LTL and MLTL presume that all signals populating the variables in a formula are sampled over the same rate and type (e.g., time or distance), and agree on a standard “time” step. Formal verification of cyber-physical systems-of-systems needs validate-able requirements expressed over (sub-)system signals of different types, such as signals sampled at different timescales, distances, or levels of abstraction, expressed in the same formula. Previous works developed more expressive logics to account for types (e.g., timescales) by sacrificing the intuitive simplicity of LTL. However, a legible direct one-to-one correspondence between a verbal and formal specification will ease validation, reduce bugs, increase productivity, and linearize the workflow from a project’s conception to actualization. Validation includes both transparency for human interpretation, and tractability for automated reasoning, as CPS often run on resource-limited embedded systems. To address these challenges, we introduced Mission-time Linear Temporal Logic Multi-type (Hariharan et al., Numerical Software Verification Workshop, 2022), a logic building on MLTL. MLTLM enables writing formal requirements over finite input signals (e.g., sensor signals and local computations) of different types, while maintaining the same simplicity as LTL and MLTL. Furthermore, MLTLM allows maintaining a direct correspondence between a verbal requirement and its corresponding formal specification. Additionally, reasoning a formal specification in the intended type (e.g., hourly for an hourly rate, and per second for a seconds rate) will use significantly less memory in resource-constrained hardware. This article extends the previous work with (1) many illustrated examples on types (e.g., time and space) expressed in the same specification, (2) proofs that were skipped in the workshop version, (3) proofs of succinctness of MLTLM compared to MLTL, and (4) a translation to MLTL of optimally minimal length.
publication: '*ACM Transactions on Embedded Computing Systems*'
---
