---
title: Robotic RF Localization & Experimental Systems
summary: A 10-GHz robotic RF testbed connecting channel sounding, mobile sensing, localization, and SLAM-based navigation experiments.
date: 2025-01-01
featured: true
weight: 5
project_tier: flagship
project_label: Flagship experimental system
project_layout: tablet-wide
tags:
  - Wireless
  - Robotics
  - Systems
---

I lead the architecture and development of **MobiFR3**, a heterogeneous 10-GHz robotic RF testbed for localization experiments and SLAM-based navigation. The current system connects RFSoC/PiRadio channel sounding and Sivers front ends with TurtleBot4/ROS 2, odometry, 2D LiDAR, and RGB sensing. Jackal UGV integration is in progress; a Vicon-based ground-truth extension is planned but is not part of the current platform.

My role spans system architecture, experiment design, RF-robot synchronization, measurement-aligned simulation, localization inference, and evaluation. I mentor student collaborators in RF hardware operation, calibration, and data collection; routine RF acquisition is conducted as a team rather than presented as a single-person hardware effort.

<img class="turtlebot-portrait" src="rf_robot.jpg" alt="MobiFR3 RF-enabled TurtleBot4 platform" />

*MobiFR3 integrates the mobile robot, RF front end, compute, power, and control layers into one experimental platform.*

![Pi-Radio and RFSoC hardware bench](rf_hardware_bench.jpg)

*The team-operated RF stack combines a Pi-Radio/Sivers front end, Xilinx RFSoC baseband hardware, Vivaldi antennas, and local compute/control equipment.*

## From system to inference

MobiFR3 provides the measured data and controlled geometry used by [MAGNETAR](/projects/magnetar-joint-rf-pose-inference/). The algorithm learns a joint posterior over transmitter position and heading from asynchronous AoA/SNR multipath snapshots, with real-to-sim calibration based on measured antenna patterns and RF-chain/noise effects. This connects the physical system directly to probabilistic inference rather than treating the robot as a demonstration platform alone.

## Media & Public Demonstrations

<div class="media-video-shell">
  <iframe src="https://www.youtube-nocookie.com/embed/2_3FGVCxYKY" title="Brooklyn 6G Summit 2025 interview on FR3 robotic localization" loading="lazy" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>

*Interview recorded at the Brooklyn 6G Summit 2025.*

At the 2025 Brooklyn 6G Summit, I demonstrated the FR3 robotic sensing and localization system, combining TurtleBot4 mobility, Pi-Radio hardware, angle-of-arrival measurements, and SLAM-based mapping. The demonstration showed how RF observations can support indoor positioning when visual information is incomplete or unavailable.

<div class="media-links" aria-label="Interview and media coverage">
  <a href="https://www.youtube.com/watch?v=2_3FGVCxYKY" target="_blank" rel="noopener">Watch the interview</a>
  <a href="https://www.5gtechnologyworld.com/brooklyn-6g-summit-2025-research-exhibits/" target="_blank" rel="noopener">5G Technology World feature</a>
  <a href="https://engineering.nyu.edu/news/brooklyn-6g-summit-2025-research-exhibits" target="_blank" rel="noopener">NYU Tandon coverage</a>
</div>

**System capabilities**
- Xilinx RFSoC with PYNQ/Vivado-based control and PiRadio/Sivers RF front ends for 10-GHz channel sounding.
- Transmit/receive waveform control, capture, synchronization, channel estimation, SNR estimation, and AoA processing in a team-operated workflow.
- Scripted TurtleBot4, linear-track, and D48 pan-tilt motion for reproducible measurement grids.
- Measurement-aligned Sionna RT scenes with TX/RX pose and motion, measured antenna patterns, and stochastic RF-chain/noise effects.
- Physical validation for posterior localization and future closed-loop sensing/navigation experiments.
