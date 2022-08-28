---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: 'MLTL Multi-type: A logic to reason over signals of different types'
subtitle: ''
summary: ''
authors:
- Gokul Hariharan
- Brian Kempa
- Tichakorm Wongpiromsarn
- Phillip H. Jones
- Kristin Y. Rozier
tags: []
categories: []
date: '2022-01-01'
lastmod: 2022-08-28T12:03:39-05:00
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
projects: ["runtime-verification"]
publishDate: '2022-08-28T17:03:39.367381Z'
publication_types:
- 1
abstract: "Modern cyber-physical systems (CPS) operate in complex systems of systems that must seamlessly work together to control safety- or mission-critical functions. Capturing specifications in a logic like LTL enables verification and validation of CPS requirements, yet an LTL formula specification can imply unrealistic assumptions, such as that all signals populating the variables in the formula are of type Boolean and agree on a standard time step. To achieve formal verification of CPS systems of systems, we need to write validate-able requirements that reason over (sub-)system signals of different types, such as signals with different timescales, or levels of abstraction, or signals with complex relationships to each other that populate variables in the same formula. Validation includes both transparency for human validation and tractability for automated validation, e.g., since CPS often run on resource-limited embedded systems. Specifications for correctness of numerical algorithms for CPS need to be able to describe global properties with precise representations of local components. Therefore, we introduce Mission-time Linear Temporal Logic Multi-type (MLTLM), a logic building on MLTL, to enable writing clear, formal requirements over finite input signals (e.g., sensor signals, local computations) of different types, cleanly coordinating the temporal logic and signal relationship considerations without significantly increasing the complexity of logical analysis, e.g., model checking, satisfiability, runtime verification (RV). We explore the common scenario of CPS systems of systems operating over different timescales, including a detailed analysis with a publicly-available implementation of MLTLM. We contribute:

1. the definition and semantics of MLTLM, a lightweight extension of MLTL allowing a single temporal formula over variables of multiple types;

2. the construction and use of an MLTLM fragment for time-granularity, with proof of the language's expressive power; and

3. the design and empirical study of an MLTLM runtime engine suitable for real-time execution on embedded hardware.
'

publication: '*In Proceedings of the 15th International Workshop on Numerical Software
  Verification (NSV)*"

links:
- name: "artifacts"
  url: http://temporallogic.org/research/NSV2022/
---
