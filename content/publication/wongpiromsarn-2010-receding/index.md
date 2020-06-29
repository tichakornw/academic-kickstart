---
title: "Receding Horizon Control for Temporal Logic Specifications"
date: 2010-01-01
publishDate: 2020-06-29T02:59:15.531855Z
authors: ["Tichakorn Wongpiromsarn", "Ufuk Topcu", "Richard M. Murray"]
publication_types: ["1"]
abstract: "In this paper, we describe a receding horizon framework that satisfies a class of linear temporal logic specifications sufficient to describe a wide range of properties including safety, stability, progress, obligation, response and guarantee. The resulting embedded control software consists of a goal generator, a trajectory planner, and a continuous controller. The goal generator essentially reduces the trajectory generation problem to a sequence of smaller problems of short horizon while preserving the desired system-level temporal properties. Subsequently, in each iteration, the trajectory planner solves the corresponding short-horizon problem with the currently observed state as the initial state and generates a feasible trajectory to be implemented by the continuous controller. Based on the simulation property, we show that the composition of the goal generator, trajectory planner and continuous controller and the corresponding receding horizon framework guarantee the correctness of the system. To handle failures that may occur due to a mismatch between the actual system and its model, we propose a response mechanism and illustrate, through an example, how the system is capable of responding to certain failures and continues to exhibit a correct behavior."
featured: false
publication: "*Proceedings of the 13th ACM International Conference on Hybrid Systems: Computation and Control*"
---
