---
title: "MAPLE-RF: Localization with Partial Maps"
summary: Efficient neural posterior inference for RF source localization while a robot has explored only part of its environment.
date: 2026-09-17
featured: true
weight: 4
project_tier: core
project_label: Core project
project_layout: core-row-start
tags:
  - Wireless
  - Localization
  - Robotics
  - Partial Maps
image:
  preview_only: true
---

I lead **MAPLE-RF**, an efficient probabilistic RF source-localization method for environments that are still being mapped. The core problem is common in robotic search: a receiver knows its own pose, but most of the surrounding floor plan may remain unobserved, including obstacles that could block or reflect the signal.

<div class="project-video-shell">
  <video controls playsinline preload="metadata" poster="featured.png" aria-describedby="maple-video-description">
    <source src="maple-rf-demo.mp4" type="video/mp4">
    Your browser does not support embedded MP4 video.
  </video>
</div>

<p id="maple-video-description"><em>The simulation follows a receiver along a recorded route while the observed map grows and the transmitter posterior is updated.</em></p>

<div class="project-figure-grid" aria-label="MAPLE-RF method and exploration figures">
  <figure class="project-figure-card">
    <img src="maple-method.png" alt="MAPLE-RF pipeline aligning multipath measurements with partial-map and receiver-centered spatial channels to infer a transmitter posterior." loading="lazy" decoding="async">
    <figcaption><strong>Inference before the map is complete.</strong> RF paths are aligned with map knownness, occupancy, visibility, receiver pose, bearing, and range before one network pass scores candidate source locations.</figcaption>
  </figure>
  <figure class="project-figure-card">
    <img src="maple-exploration.png" alt="MAPLE-RF current and accumulated source-location posteriors as a receiver follows an exploration route and reveals more of the map." loading="lazy" decoding="async">
    <figcaption><strong>Belief accumulation during exploration.</strong> Current measurements and accumulated posteriors sharpen the source belief as the receiver moves and the observed map expands.</figcaption>
  </figure>
</div>

## Method

MAPLE-RF aligns estimated path angles and SNRs with spatial channels for map knownness, occupancy, line-of-sight visibility, receiver pose, bearing, and range. A residual U-Net then scores every candidate transmitter location in one pass. Unlike a full-grid digital-twin query, inference does not ray-trace every candidate whenever the map or receiver pose changes.

## Findings

- Training across mixed levels of map coverage is essential for localization with unexplored space.
- MAPLE-RF retained about 94% of its complete-map 1-m recall when 75-85% of the map was unobserved.
- Fresh-query inference was about 218 times faster than full-grid general-purpose ray tracing in the evaluated configuration.
- Bayesian accumulation along exploration routes placed more posterior probability near the source than the compared baselines.

The current study is simulation-based. Its role in the broader research program is to make posterior RF localization practical when a robot must localize and map concurrently, before a complete digital twin is available.

**Paper:** [MAPLE-RF: Efficient Probabilistic RF Source Localization in Partially Explored Environments](https://arxiv.org/abs/2609.21026) — first and corresponding author; IEEE ICRA 2027, under review.
