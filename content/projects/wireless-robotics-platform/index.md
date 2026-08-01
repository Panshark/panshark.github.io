---
title: Wireless Robotics Platform (FR3 / TurtleBot4 & Jackal UGV)
summary: RFSoC/Pi-Radio FR3 channel-sounding platform for robotic localization and navigation experiments with TurtleBot4 and Jackal UGV.
date: 2025-01-01
featured: true
weight: 2
tags:
  - Wireless
  - Robotics
  - Systems
---

I am building and validating a 10-GHz FR3 robotic measurement platform for closed-loop localization and navigation experiments. The system combines Xilinx RFSoC 4×2 boards, Pi-Radio FR3 front ends, Vivaldi antennas, 2D LiDAR/RGB sensing, fixed and linear-track/D48 measurements, TurtleBot4 transmitter mobility, Jackal UGV receiver mobility, and Vicon ground truth under controlled LOS/NLOS transitions.

![Vicon validation area with Jackal and TurtleBot platforms](validation_setup.png)

*The validation setup provides repeatable ground truth for robot motion and obstacle-induced LOS/NLOS experiments.*

![Platform demo](demo.gif)

*The demo shows the robotic measurement platform executing controlled motion while RF sensing data are collected.*

<img class="turtlebot-video" src="/media/6gsummit_turtlebot.gif" alt="TurtleBot demo" />

*This public demo shows the TurtleBot4-mounted FR3 hardware operating in a live measurement setting.*

**System capabilities**
- RFSoC transmit/receive waveform generation, capture, synchronization, channel estimation, SNR estimation, and AoA processing.
- Pi-Radio/Sivers front-end control, remote TCP/REST control, and synchronized physical metadata logging.
- Scripted TurtleBot4, linear-track, and D48 pan-tilt motion for reproducible measurement grids.
- Physical support for MC-CLE/LOCUS-DT posterior localization and wireless-aware navigation experiments.

![Pi-Radio and RFSoC hardware bench](rf_hardware_bench.jpg)

*The hardware bench combines the Pi-Radio FR3 front end, RFSoC 4×2 baseband, Vivaldi antennas, and local compute/control equipment.*

<img class="turtlebot-portrait" src="rf_robot.jpg" alt="RF-enabled TurtleBot platform" />

*The hardware photo shows the deployed TurtleBot4 stack with the RF front end, compute, power, and control layers integrated on the robot.*
