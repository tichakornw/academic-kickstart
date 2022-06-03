---
title: Resource-Aware Hierarchical Runtime Verification for Mixed-Abstraction-Level Systems of Systems (NSF)
summary: Develop runtime verification techniques that incorporate mixed-abstraction-level granularity in specifications and enable on-deadline mitigation triggering

tags:
- Formal methods
- Runtime verification
- Current projects
date: "2021-01-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: ""
  focal_point: Smart

links:
#- icon: linkedin
#  icon_pack: fab
#  url: https://www.linkedin.com/in/tichakorn-wongpiromsarn-3a9b2782/
#  name: Follow
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

**Award Number:** CNS-2038903<br />
**Amount:** 1,200,000<br />
**Start Date:** 01/01/2021<br />
**End Date:** 12/31/2023<br />
**Collaborators:** Kristin  Rozier (PI), Phillip Jones

Piloting an aircraft is popularly described as hours of abject boredom punctuated by periods of abject terror. Similarly, a spacecraft in transit to a distant target remains largely dormant but for periodic heightened activity required for maintenance and staying on course. Aircraft and spacecraft are complex systems of systems that must seamlessly work together, switching control through a carefully orchestrated hierarchy representing different levels of abstraction, e.g., exemplified by different timescales for events. Each on-board system presents its own verification challenge; verifying that the symphony of all of them playing together at the same time, in the face of potentially unexpected environmental inputs, is particularly daunting. We can supplement design-time verification with efficient runtime verification engines, but they need to grow to be able to reason about the hierarchical nature of complex systems-of-systems, where single requirements may need to encapsulate multiple levels of abstraction. The final result must be able to execute in real time, within system resource constraints. Existing tools for runtime verification aren't capable of obeying constraints imposed by running them on real systems (or in real missions), and don't have parameters to focus their computational demands on the tasks most impactful on system safety. Achieving safe CPS depends on growing the tools and algorithms of real-time verification to integrate realistic safety checks into their control architectures and dynamic environments.

This project adapts techniques from formal methods, control theory, hardware-software integration, and software engineering to design runtime monitors that inspect cyber-physical systems of systems without interfering with their normal operation. The project designs, analyzes, and implements fundamental runtime verification techniques by dealing with three general and orthogonal problems: mixed-abstraction-level granularity in specifications, resource-awareness to ensure non-intrusiveness of runtime monitors, and augmenting monitors with model-prediction to enable on-deadline mitigation triggering. Key innovations stem from this rigorous foundation in establishing a new formal semantics for hierarchical, mixed-abstraction-level specification, and evaluating formal specifications without interfering with the system's normal operation, while maximizing utilization of resources within realistic constraints of embedded CPS. The project generalizes the new theory into specification patterns for hierarchical functional requirements and synthesize predictive models to enable better, more automated creation of runtime verification configurations to meet scalability demands of modern CPS. Flight tests of small aircraft swarms are used to validate this approach.