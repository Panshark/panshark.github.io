---
title: Wireless Robotics Platform (FR3 / TurtleBot4)
summary: RFSoC/Pi-Radio FR3/mmWave channel-sounding platform for robotic localization and navigation experiments.
date: 2025-01-01
featured: true
weight: 2
tags:
  - Wireless
  - Robotics
  - Systems
---

I built an FR3/mmWave robotic measurement platform for closed-loop localization and navigation experiments. The system combines Xilinx RFSoC boards, Pi-Radio or Sivers RF front ends, fixed transmitter/receiver baselines, linear-track and D48 pan-tilt sweeps, TurtleBot4 transmitter mobility, and Jackal UGV receiver mobility.

![Platform demo](demo.gif)

*The demo shows the robotic measurement platform executing controlled motion while RF sensing data are collected.*

<img class="turtlebot-video" src="/media/6gsummit_turtlebot.gif" alt="TurtleBot demo" />

*This public demo shows the TurtleBot4-mounted FR3 hardware operating in a live measurement setting.*

**System capabilities**
- RFSoC transmit/receive waveform generation, capture, synchronization, channel estimation, SNR estimation, and AoA processing.
- Pi-Radio/Sivers front-end control, remote TCP/REST control, and synchronized physical metadata logging.
- Scripted TurtleBot4, linear-track, and D48 pan-tilt motion for reproducible measurement grids.
- Physical support for MC-CLE/LOCUS-DT posterior localization and wireless-aware navigation experiments.

<img class="turtlebot-portrait" src="rf_robot.jpg" alt="RF-enabled TurtleBot platform" />

*The hardware photo shows the deployed TurtleBot4 stack with the RF front end, compute, power, and control layers integrated on the robot.*
