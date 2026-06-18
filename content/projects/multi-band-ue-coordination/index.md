---
title: Multi-Band UE Coordination Under Mobility
summary: UE-centric multi-cell multi-band handset digital twins for closed-loop array, band, and rate prediction under mobility.
date: 2025-01-01
featured: true
weight: 4
tags:
  - Wireless
  - Systems
  - Machine Learning
---

I am developing **MCMB-HDT** (Multi-Cell Multi-Band Handset Digital Twin), a UE-centric framework that couples real urban geometry, base-station topology, FR1/FR3/mmWave ray tracing, embodied handset antenna radiation, pedestrian motion, handset pose, and measurement-limited feedback. On top of this twin, we study Transformer-based rate prediction from sparse asynchronous histories and PPO-based power-aware array/band activation under rate, power, and exploration constraints.

![NYU Tandon geographic data and 3D digital-twin scene](digital_twin_scene.png)

*This figure shows how geographic data are converted into a 3D digital-twin scene for multi-band ray-tracing simulation.*

![Multi-band capacity map and UE mobility setup](ue_capacity_map.png)

*The capacity maps illustrate why the best band and antenna choice changes with location, handset pose, and pedestrian mobility.*

![Handset antenna geometry and multi-band array layout](ue_device.png)

*The UE layout defines the active antenna elements and frequency bands used by the prediction and activation policies.*

![Policy exploration and achievable-rate tradeoff](policy_risk_results.png)

*The policy result summarizes the tradeoff between exploration risk and achievable rate when the handset activates only a subset of arrays and bands.*

**Related papers**
- [Transformer-Based Rate Prediction for Multi-Band Cellular Handsets](https://arxiv.org/pdf/2509.25722) (IEEE ICC Workshops 2026)
- MCMB-HDT: A Multi-Cell Multi-Band Handset Digital Twin for Learning-Based Closed-Loop Array Activation (IEEE JSAC, under review)
