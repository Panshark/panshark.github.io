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
        Ph.D. candidate in Electrical and Computer Engineering at **NYU WIRELESS**, advised by **Prof. Sundeep Rangan**. I build uncertainty-aware wireless intelligence for embodied autonomy and adaptive 6G systems.

        [Download Academic CV](/cvs/CV_academic.pdf)
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

        I am a Ph.D. candidate in Electrical and Computer Engineering at New York University, advised by **[Prof. Sundeep Rangan](https://engineering.nyu.edu/faculty/sundeep-rangan)** in **NYU WIRELESS**. My research asks how future wireless systems can move beyond point estimates and link metrics to represent competing spatial hypotheses, quantify uncertainty, and use those beliefs for sensing, navigation, and resource activation when observations are sparse, noisy, blocked, and environment-dependent.

        My current work combines **posterior RF localization**, **wireless digital twins**, **wireless robotics**, **multi-band UE adaptation**, and **multimodal spatial reasoning**. I developed MC-CLE and LOCUS-DT for likelihood-based RF belief inference; study PIRL and digital-twin priors for zero-shot wireless robot navigation; develop MCMB-HDT for closed-loop multi-band handset adaptation; and build object-centric graph memories for robot grounding and search. I also build physical FR3/mmWave RFSoC/Pi-Radio measurement systems with TurtleBot4 and Jackal UGV platforms.
    design:
      columns: '2'

  - block: features
    id: research
    content:
      title: Research Themes
      items:
        - name: Belief-Aware RF Sensing
          description: Posterior localization methods that retain multimodal spatial hypotheses for 6G and robotics.
          icon: chart-bar
        - name: Wireless Digital Twins
          description: Ray-tracing priors for zero-shot indoor navigation, wireless SLAM, and robot policies.
          icon: map
        - name: Wireless Robotics Systems
          description: FR3/mmWave RFSoC/Pi-Radio testbeds with TurtleBot4, Jackal UGV, D48 pan-tilt, and linear-track motion.
          icon: cpu-chip
        - name: Closed-Loop UE Adaptation
          description: Multi-cell multi-band handset digital twins for array, band, and rate prediction under mobility.
          icon: arrows-right-left
    design:
      columns: 2

  - block: collection
    id: projects
    content:
      title: Selected Projects
      text: Wireless systems and embodied AI pipelines that move from probabilistic inference to real-world experiments.
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
        ![NYU WIRELESS group photo](/media/lab.jpg)

        ---

        I am part of **NYU WIRELESS**, a leading 6G research center at NYU Tandon. For an overview of the center's scope, facilities, and research programs, see the NYU WIRELESS overview deck.

        [NYU WIRELESS Overview (PDF)](/uploads/NYU_wireless.pdf)
    design:
      columns: '2'

  - block: markdown
    id: contact
    content:
      title: Contact
      text: |-
        Email: [hl4155@nyu.edu](mailto:hl4155@nyu.edu)
---
