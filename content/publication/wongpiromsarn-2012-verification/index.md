---
title: "Verification of Periodically Controlled Hybrid Systems: Application to an Autonomous Vehicle"
date: 2012-01-01
publishDate: 2020-06-29T03:28:52.984094Z
authors: ["Tichakorn Wongpiromsarn", "Sayan Mitra", "Andrew Lamperski", "Richard M. Murray"]
publication_types: ["2"]
abstract: "This article introduces Periodically Controlled Hybrid Automata (PCHA) for modular specification of embedded control systems. In a PCHA, control actions that change the control input to the plant occur roughly periodically, while other actions that update the state of the controller may occur in the interim. Such actions could model, for example, sensor updates and information received from higher-level planning modules that change the set point of the controller. Based on periodicity and subtangential conditions, a new sufficient condition for verifying invariant properties of PCHAs is presented. For PCHAs with polynomial continuous vector fields, it is possible to check these conditions automatically using, for example, quantifier elimination or sum of squares decomposition. We examine the feasibility of this automatic approach on a small example. The proposed technique is also used to manually verify safety and progress properties of a fairly complex planner-controller subsystem of an autonomous ground vehicle. Geometric properties of planner-generated paths are derived which guarantee that such paths can be safely followed by the controller."
featured: false
publication: "*ACM Transactions on Embedded Computing Systems*"

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

links:
- name: "full version"
  url: wongpiromsarn-2012-verification-full.pdf
---