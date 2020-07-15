---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---


## Online optimization
Technological advances in many disciplines have recently motivated a growing interest in *online* (or *time-varying*) *optimization*. In traditional *static optimization* (also called *batch* or *time-invariant*), the data of a problem are collected once and then a solver is applied until a solution (or good approximation thereof) is reached. Online optimization instead features streaming data sources, in the sense that new data are revealed in a sequential manner over time, rather than all at once. As a consequence, online solvers need to be lightweight and reactive, capable of processing new data and adapt to changes in the problem in real time. Examples of problems that fit into this framework arise in signal and image processing, machine learning, model predictive control (MPC), cooperative robotics, smart grids.

My research into online optimization has been mainly focused on providing a unified framework for online algorithms, which would allow to both design and study the convergence of a wide class of methods. The recent [pre-print](https://arxiv.org/abs/2004.11709) is a first step in this direction. This work builds on the *prediction-correction* framework, which allows to exploit the time-varying nature of the problem in order to deliver better performance, and combines it with operator theoretical solvers, that model for example proximal gradient methods and ADMM. Other papers that build towards this goal are [this](https://arxiv.org/abs/1903.00298) and [this](https://ieeexplore.ieee.org/document/8770071).


## Distributed optimization
The possibility of outfitting many devices with computational and connectivity capabilities has given rise to a wide variety of *multi-agent* (or *distributed*) systems, ranging from cooperative mobile robots to sensor networks (and more broadly the Internet-of-Things, IoT, paradigm), from connected vehicles to smart grids. Many of the tasks that distributed systems need to perform can be modeled as distributed optimization problems, which have attracted a lot of attention in the literature. The decentralized nature of these systems guarantees *(i)* robustness (no single point of failure) and *(ii)* privacy (data is not directly shared between components of the system). The framework of distributed optimization can also model *parallel optimization* and *federated learning*, in which a central unit offloads computations on subsets of data to agents, and then aggregates the results.

Distributed systems however present some challenges that need to be addressed during the design of distributed algorithms. For example, a distributed system may be asynchronous, that is, the agents do not agree on a common schedule, or the communications between agents may be prone to failures, noise or quantization. My research into distributed optimization has focused on the design of *robust* distributed algorithms, for example the ADMM-based algorithm of [pre-print](https://arxiv.org/abs/1901.09252), and the online proximal gradient method in this [pre-print](https://arxiv.org/abs/2001.00870), which is robust to additive errors caused for example by quantization.