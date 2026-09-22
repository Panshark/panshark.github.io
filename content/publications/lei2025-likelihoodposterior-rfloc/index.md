---
title: "Beyond Point Estimates: Likelihood-Based Full-Posterior Wireless Localization"
authors:
  - me
  - Hao Guo
  - Tommy Svensson
  - Sundeep Rangan
roles:
  - First author
  - Corresponding author
date: "2026-01-01"
publishDate: "2026-01-01"
publication_types:
  - "paper-conference"
publication: "Asilomar"
publication_short: ""
abstract: "Wireless localization is often reported as a point estimate even when sparse multipath measurements support several physically plausible positions. MC-CLE learns candidate-wise likelihoods from compact angle-of-arrival and signal-strength observations, preserving directional, multimodal uncertainty as a full spatial posterior that can be fused across measurements."
summary: "MC-CLE learns full spatial posteriors from sparse AoA/SNR measurements, preserving multipath ambiguity beyond Gaussian point-error models."
tags:
  - Wireless
  - Localization
  - Probabilistic Inference
featured: true
hugoblox:
  ids:
    arxiv: 2509.25719
links:
  - type: pdf
    url: "https://arxiv.org/pdf/2509.25719"
image:
  caption: "MC-CLE maps the ray-traced scene, receiver pose geometry, and channel signature to a full spatial posterior."
  focal_point: ""
  preview_only: false
projects:
  - "rf-belief-inference"
slides: ""
---

<div class="author-role-note">
  <span>First and corresponding author</span>
</div>

MC-CLE scores candidate transmitter states rather than regressing directly to one coordinate. The resulting posterior retains spatial ambiguity created by blockage, antenna directivity, and multipath, and provides a probabilistic interface for multi-view fusion and downstream decisions.

The continuing journal study, [*Learning a Measurement-to-Posterior Map for Wireless Localization*](/publications/lei2025-likelihoodposterior-wirelessloc/), is under review at IEEE Transactions on Vehicular Technology.
