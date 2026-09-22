---
title: Multi-Band UE Coordination Under Mobility
summary: UE-centric multi-cell multi-band handset digital twins for closed-loop array, band, and rate prediction under mobility.
date: 2025-01-01
featured: true
weight: 7
project_tier: related
project_label: Complementary system line
tags:
  - Wireless
  - Systems
  - Machine Learning
image:
  focal_point: Right
---

I lead **MCMB-HDT** (Multi-Cell Multi-Band Handset Digital Twin), including the research direction, system formulation, digital-twin design, and learning methods, while mentoring a Ph.D. student on implementation and evaluation. The framework couples urban geometry, base-station topology, FR1/FR3 ray tracing, handset antenna patterns, pedestrian motion, device pose, and measurement-limited feedback.

On top of this twin, a Transformer predicts per-array rates from sparse asynchronous histories, reducing average per-array rate MSE by 28% in our study. A recurrent PPO policy then makes retain-or-explore array decisions and outperforms the evaluated greedy and bandit baselines while trading link quality against measurement overhead.

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
- [MCMB-HDT: A Multi-Cell Multi-Band Handset Digital Twin for Learning-Based Closed-Loop Array Activation](/publications/chenlei2026jsac-mcmbhdt/) (IEEE JSAC, under review)
