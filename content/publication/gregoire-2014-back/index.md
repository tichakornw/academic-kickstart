---
title: "Back-pressure traffic signal control with unknown routing rates"
date: 2014-01-01
publishDate: 2020-06-29T03:28:52.981952Z
authors: ["Jean Gregoire", "Emilio Frazzoli", "Arnaud de La Fortelle", "Tichakorn Wongpiromsarn"]
publication_types: ["2"]
abstract: "The control of a network of signalized intersections is considered. Previous works proposed a feedback control belonging to the family of the so-called back-pressure controls that ensures provably maximum stability given pre-specified routing probabilities. However, this optimal back-pressure controller (BP*) requires routing rates and a measure of the number of vehicles queuing at a node for each possible routing decision. It is an idealistic assumption for our application since vehicles (going straight, turning left/right) are all gathered in the same lane apart from the proximity of the intersection and cameras can only give estimations of the aggregated queue length. In this paper, we present a back-pressure traffic signal controller (BP) that does not require routing rates, it requires only aggregated queue lengths estimation (without direction information) and loop detectors at the stop line for each possible direction. A theoretical result on the Lyapunov drift in heavy load conditions under BP control is provided and tends to indicate that BP should have good stability properties. Simulations confirm this and show that BP stabilizes the queuing network in a significant part of the capacity region."
featured: false
publication: "*IFAC Proceedings Volumes*"
---
