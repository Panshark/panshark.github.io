---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

design:
  spacing: '2.75rem'

sections:
  - block: resume-biography-3
    content:
      username: me
      text: |-
        I am a Ph.D. candidate in Electrical and Computer Engineering at **New York University**, advised by **[Prof. Sundeep Rangan](https://engineering.nyu.edu/faculty/sundeep-rangan)** at **[NYU WIRELESS](https://wireless.engineering.nyu.edu/)**.

        My research develops **spatially aware, uncertainty-aware wireless intelligence** for embodied autonomy and adaptive 6G systems. I build algorithms, wireless digital twins, and physical FR3/mmWave testbeds that turn sparse RF and multimodal observations into calibrated spatial beliefs and closed-loop decisions.

        <div class="hero-actions">
          <a href="#research">Research themes</a>
          <a href="#publications">Key publications</a>
          <a href="/cvs/CV_academic.pdf">Academic CV</a>
        </div>
      headings:
        about: About
        education: Education
        interests: Research Interests
    design:
      background:
        gradient_mesh:
          enable: false
      name:
        size: md
      avatar:
        size: large
        shape: square

  - block: markdown
    id: about
    content:
      title: Research Overview
      text: |-
        <img class="about-portrait" src="/media/casual.png" alt="Casual portrait">

        My work starts from a simple problem: future wireless and robotic systems rarely see the world through clean measurements. A receiver may observe only a few multipath components; a robot may have partial visual context; a handset may only measure the bands and antenna modules it chooses to activate. In these settings, a single point estimate is often less useful than a belief over competing spatial hypotheses.

        I use this view to connect four threads: **posterior RF localization** through MC-CLE and LOCUS-DT, **wireless digital twins** for zero-shot robot navigation and SLAM, **UE-centric multi-band adaptation** under mobility and blockage, and **multimodal spatial memory** for embodied agents. The long-term goal is to make wireless systems not only communicate, but also reason about space, uncertainty, and action.
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
      title: Key Projects
      text: Wireless systems and embodied AI pipelines that move from probabilistic inference to real-world experiments.
      sort_by: weight
      order: asc
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

  - block: markdown
    id: publications
    content:
      title: Key Publications
      text: |-
        - **2026 · IEEE TWC**: [Site-Agnostic Posterior Inference for Indoor Localization with Ray-Tracing Wireless Digital Twins](/publications/lei2026twc-siteagnostic-posterior/)
        - **2026 · IEEE JSAC**: [MCMB-HDT: A Multi-Cell Multi-Band Handset Digital Twin for Learning-Based Closed-Loop Array Activation](/publications/chenlei2026jsac-mcmbhdt/)
        - **2026 · IEEE ICC Workshops**: [Transformer-Based Rate Prediction for Multi-Band Cellular Handsets](/publications/chenlei2025-multibandue-switching/)
        - **2026 · IEEE GLOBECOM**: [LOCUS-DT: Localization via Observation-Conditioned Uncertainty Scoring with Digital Twins](/publications/lei2026globecom-locusdt/)
        - **2026 · Asilomar**: [Beyond Point Estimates: Likelihood-Based Full-Posterior Wireless Localization](/publications/lei2025-likelihoodposterior-rfloc/)
        - **2025 · IEEE OJ-COMS**: [Digital Twin-Enhanced Wireless Indoor Navigation: Achieving Efficient Environment Sensing with Zero-Shot Reinforcement Learning](/publications/lei2025ojcoms-digitaltwin/)
        - **2025 · RLC**: [Reinforcement Learning with Physics-Informed Symbolic Program Priors for Zero-Shot Wireless Indoor Navigation](/publications/li2025rlc-symbolicpriors/)
        - **2024 · IEEE ICRA**: [Zero-Shot Wireless Indoor Navigation through Physics-Informed Reinforcement Learning](/publications/yin2024zeroshot-icra/)

        [Full publication list](/publications/)
    design:
      columns: '1'

  - block: markdown
    id: lab
    content:
      title: 'Our Center: NYU WIRELESS'
      text: |-
        <a class="lab-photo-link" href="/uploads/NYU_wireless.pdf" aria-label="Open NYU WIRELESS overview PDF">
          <img src="/media/lab.jpg" alt="NYU WIRELESS group photo">
        </a>

        ---

        I am proud to be part of **NYU WIRELESS**, a leading 6G research center at NYU Tandon and the home base for my work on wireless sensing, localization, digital twins, and robotic measurement systems. The center gives my research a rare mix of theory, simulation, RF hardware, and mobile robotic platforms.

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
