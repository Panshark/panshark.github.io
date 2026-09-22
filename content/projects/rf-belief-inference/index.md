---
title: Probabilistic RF Localization & Wireless Digital Twins
summary: Likelihood, neural-posterior, and digital-twin methods that turn sparse multipath observations into calibrated spatial beliefs.
date: 2026-01-01
featured: true
weight: 1
tags:
  - Wireless
  - Localization
  - Digital Twins
  - Uncertainty
---

I lead a research line on posterior RF localization that preserves competing spatial hypotheses instead of collapsing a sparse wireless observation into one point estimate. The common methodology is to score candidate locations or poses, calibrate simulation to the measurement process, and fuse multiple posterior beliefs over time.

The line includes **MC-CLE** for candidate-likelihood inference, **LOCUS-DT** for observation-conditioned scoring against ray-tracing libraries, direct neural measurement-to-posterior models, **MAGNETAR** for joint position-and-heading inference, and **MAPLE-RF** for efficient localization when most of the map is still unexplored.

<div style="background: #fff; padding: 12px; border-radius: 6px;">
  <img src="mccle_flow.png" alt="MC-CLE posterior inference workflow" style="display: block; width: 100%; height: auto;" />
</div>

*MC-CLE uses the ray-tracing scene, receiver pose geometry, and channel signature to score candidate transmitter locations and produce a posterior belief map.*

![LOCUS-DT probability heatmap results](locus_dt_probability_heatmaps.png)

*The LOCUS-DT heatmaps show how digital-twin likelihoods preserve multipath-driven spatial hypotheses, while simpler Gaussian baselines tend to smooth out the uncertainty structure.*

**Related papers**
- [Beyond Point Estimates: Likelihood-Based Full-Posterior Wireless Localization](https://arxiv.org/pdf/2509.25719) (Asilomar 2026)
- [Likelihood-Based Wireless Localization with Last-Bounce Spatial Features](/publications/bomfinlei2026-lastbounce/) (Asilomar 2026)
- [Learning a Measurement-to-Posterior Map for Wireless Localization](/publications/lei2025-likelihoodposterior-wirelessloc/) (IEEE TVT, under review)
- [LOCUS-DT: Localization via Observation-Conditioned Uncertainty Scoring with Digital Twins](/publications/lei2026globecom-locusdt/) (IEEE GLOBECOM 2026)
- [Site-Agnostic Posterior Inference for Indoor Localization with Ray-Tracing Wireless Digital Twins](/publications/lei2026twc-siteagnostic-posterior/) (revision in preparation for resubmission to IEEE TWC)
- [MAGNETAR: Multipath-Guided Spatial Posteriors for Transmitter Pose Inference in the Upper Mid-Band](/projects/magnetar-joint-rf-pose-inference/) (IEEE ICRA 2027, under review)
- [MAPLE-RF: Efficient Probabilistic RF Source Localization in Partially Explored Environments](/projects/maple-rf-partial-map-localization/) (IEEE ICRA 2027, under review)
