---
title: "Formal Methods for Design and Verification of Embedded Control Systems: Application to an Autonomous Vehicle"
date: 2010-05-01
publishDate: 2020-06-29T21:46:04.933424Z
authors: ["Tichakorn Wongpiromsarn"]
publication_types: ["7"]
abstract: "The design of reliable embedded control systems inherits the difficulties involved in designing both control systems and distributed (concurrent) computing systems. Design bugs in these systems may arise from the unforeseen interactions among the computing, communication and control subsystems. Motivated by the difficulties of finding this type of design bugs, this thesis develops mathematical frameworks, based on formal methods, to facilitate the design and analysis of such embedded systems. An expressive specification language of linear temporal logic (LTL) is used to specify the desired system properties. The practicality of the proposed frameworks is demonstrated through autonomous vehicle case studies and autonomous urban driving problems.<br/><br/>

Our approach incorporates methodology from computer science and control, including model checking, theorem proving, synthesis of digital designs, reachability analysis, Lyapunov-type methods and receding horizon control. This thesis consists of two complementary parts, namely, verification and design. First, we introduce Periodically Controlled Hybrid Automata (PCHA), a subclass of hybrid automata that abstractly captures a common design pattern in embedded control systems. New sufficient conditions that exploit the structure of PCHAs in order to simplify their invariant verification are presented.<br/><br/>

Although the aforementioned technique simplifies an invariant verification of PCHAs, finding a proper invariant remains a challenging problem. To complement the verification efforts, in the second part of the thesis, we present a methodology for automatic synthesis of embedded control software that provides a formal guarantee of system correctness, with respect to its desired properties expressed in linear temporal logic. The correctness of the system is guaranteed even in the presence of an adversary (typically arising from changes in the environments), disturbances and modeling errors. A receding horizon framework is proposed to alleviate the associated computational complexity of LTL synthesis. The effectiveness of this framework is demonstrated through the autonomous urban driving problems."
featured: false
publication: ""

# Summary. An optional shortened abstract.
summary: ""

# Digital Object Identifier (DOI)
doi: ""

# Tags (optional).
#   Set `tags = []` for no tags, or use the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags: []

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["deep-learning"]` references
#   `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: ["formal-methods"]
---
