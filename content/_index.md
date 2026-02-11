---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

design:
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      username: me
      text: |-
        Ph.D. candidate at **NYU Wireless** working on RF sensing, wireless robotics, ISAC, and reinforcement learning.
        **Open to faculty and research scientist roles (2026).**

        [Download Academic CV](/cvs/CV_academic.pdf) · [Download Industry CV](/cvs/CV_industrial.pdf)
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      background:
        gradient_mesh:
          enable: true
      name:
        size: md
      avatar:
        size: large
        shape: circle

  - block: markdown
    id: about
    content:
      title: About
      text: |-
        ![Formal portrait](/media/formal.jpg)

        ---

        I am a Ph.D. candidate in Electrical and Computer Engineering at New York University, supervised by **Prof. Sundeep Rangan** in NYU Wireless. My research spans **RF sensing**, **wireless robotics**, **ISAC**, and **reinforcement learning**, with recent focus on likelihood-based RF localization and multi-band UE coordination under mobility. I build end-to-end systems that connect theory, simulation, and robotics experiments.
    design:
      columns: '2'

  - block: features
    id: research
    content:
      title: Research Themes
      items:
        - name: Likelihood-Based RF Localization
          description: Full-posterior inference pipelines for 6G decision making and risk-aware control.
          icon: chart-bar
        - name: Wireless Indoor Navigation
          description: Physics-informed RL and digital twins for zero-shot navigation and sensing.
          icon: map
        - name: Wireless Robotics Systems
          description: FR3/TurtleBot4 platform for closed-loop localization and navigation.
          icon: cpu-chip
        - name: Multi-Band UE Coordination
          description: Transformer-based antenna and band coordination under mobility.
          icon: arrows-right-left
    design:
      columns: 2

  - block: collection
    id: projects
    content:
      title: Selected Projects
      text: Wireless systems that move from theory to real-world experiments.
      filters:
        folders:
          - projects
        featured_only: true
    design:
      view: article-grid
      columns: 3
      show_date: false
      show_read_time: false
      show_read_more: false

  - block: collection
    id: publications
    content:
      title: Selected Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: citation

  - block: collection
    id: all-publications
    content:
      title: All Publications
      filters:
        folders:
          - publications
    design:
      view: citation

  - block: markdown
    id: lab
    content:
      title: Lab
      text: |-
        ![NYU Wireless group photo](/media/lab.jpg)

        ---

        I am part of **NYU Wireless**, a leading 6G research center at NYU Tandon. For an overview of the center's scope, facilities, and research programs, see the NYU Wireless overview deck.

        [NYU Wireless Overview (PDF)](/uploads/NYU_wireless.pdf)
    design:
      columns: '2'

  - block: markdown
    id: contact
    content:
      title: Contact
      text: |-
        Email: [hl4155@nyu.edu](mailto:hl4155@nyu.edu)
---
