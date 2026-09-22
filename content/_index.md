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
        I am a Ph.D. candidate in Electrical and Computer Engineering at **New York University**, advised by **[Prof. Sundeep Rangan](https://engineering.nyu.edu/faculty/sundeep-rangan)** at **[NYU WIRELESS](https://wireless.engineering.nyu.edu/)**. I expect to graduate in May 2027.

        My research centers on **RF sensing and probabilistic spatial intelligence for autonomous systems**. I combine candidate-wise likelihoods, neural posterior models, Bayesian fusion, and measurement-aligned wireless digital twins to turn sparse, ambiguous RF observations into calibrated spatial beliefs, then use those beliefs for localization, robotic sensing, navigation, and closed-loop wireless decisions.

        <div class="hero-actions">
          <a href="#projects">Projects</a>
          <a href="#publications">Publications</a>
          <a href="/cvs/CV_academic.pdf">Academic CV</a>
          <a href="/cvs/CV_industrial.pdf">Industry Resume</a>
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

        Wireless and robotic systems rarely observe a clean, complete world. A receiver sees only a few noisy multipath components, a robot may know only part of the map, and a handset can measure only the bands and antenna modules it activates. I treat that ambiguity as a first-class object: represent competing hypotheses, calibrate simulation against measurements, and fuse evidence across observations instead of collapsing uncertainty too early.

        This methodology connects my current research: **MAGNETAR** infers a joint posterior over transmitter position and heading from a single multipath snapshot; **MAPLE-RF** localizes efficiently with a partially observed map; **MC-CLE** and **LOCUS-DT** use likelihoods and ray-tracing priors for calibrated localization; and **MobiFR3** grounds these ideas in a 10-GHz robotic measurement system. A complementary line, **MCMB-HDT**, carries the same belief-and-action perspective into closed-loop multi-band link decisions. I also mentor an emerging object-centric RGB-D spatial-memory project for embodied agents.
    design:
      columns: '2'

  - block: features
    id: research
    content:
      title: Research Themes
      items:
        - name: Probabilistic RF Localization
          description: Likelihood and neural-posterior methods that retain multimodal position and pose hypotheses.
          icon: chart-bar
        - name: Wireless Digital Twins
          description: Measurement-aligned ray-tracing priors, real-to-sim calibration, and partial-map inference.
          icon: map
        - name: Robotic RF Sensing
          description: MobiFR3 combines 10-GHz channel sounding, TurtleBot4 motion, ROS 2, LiDAR, RGB, and odometry.
          icon: cpu-chip
        - name: Belief-Space Decision Making
          description: Bayesian fusion, physics-informed RL, and PPO connect uncertainty to motion, sensing, and control.
          icon: arrow-path
        - name: Closed-Loop UE Adaptation
          description: Multi-cell, multi-band handset digital twins for rate prediction and sensing-aware array decisions.
          icon: arrows-right-left
        - name: Object-Centric Spatial Memory
          description: A complementary RGB-D direction for sparse sensing, retrieval, and embodied spatial reasoning.
          icon: cube
    design:
      columns: 2

  - block: markdown
    id: research-map
    content:
      title: ''
      text: |-
        <figure class="research-map-panel" aria-labelledby="research-map-caption">
          <picture class="research-overview-picture">
            <source media="(max-width: 680px)" srcset="/media/research-program-overview-mobile.svg?v=20260921-4">
            <img src="/media/research-program-overview.svg?v=20260921-4" alt="Research pipeline that transforms sparse RF and multimodal evidence through model-aware probabilistic inference into calibrated position and pose beliefs, then uses uncertainty to guide localization, active sensing, navigation, and wireless decisions, with physical validation on the MobiFR3 robotic platform.">
          </picture>
          <figcaption id="research-map-caption">
            <strong>From physical evidence to spatial belief to action.</strong> Sparse RF and multimodal observations are aligned with measured systems and digital-twin priors, converted into calibrated posteriors, and fused across viewpoints. The resulting uncertainty guides localization, active measurement, navigation, and closed-loop wireless decisions.
          </figcaption>
        </figure>
    design:
      columns: '1'

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
      count: 6
    design:
      view: article-grid
      columns: 3
      show_date: false
      show_read_time: false
      show_read_more: false

  - block: markdown
    id: media
    content:
      title: Featured Media
      text: |-
        <article class="featured-media-card">
          <a class="featured-media-visual" href="https://www.youtube.com/watch?v=2_3FGVCxYKY" target="_blank" rel="noopener" aria-label="Watch the Brooklyn 6G Summit 2025 interview">
            <img src="/media/6gsummit-interview.jpg" alt="FR3 robotic localization demonstration at the Brooklyn 6G Summit 2025">
            <span class="featured-media-play" aria-hidden="true">Watch interview</span>
          </a>
          <div class="featured-media-copy">
            <p class="featured-media-kicker">Brooklyn 6G Summit 2025</p>
            <h3>FR3 Robotic Localization Demonstration</h3>
            <p>I presented our FR3 robotic sensing platform, combining TurtleBot4 mobility, Pi-Radio hardware, and probabilistic RF localization to show how wireless measurements can support indoor positioning when visual information is limited.</p>
            <div class="media-links" aria-label="Interview and media coverage">
              <a href="https://www.youtube.com/watch?v=2_3FGVCxYKY" target="_blank" rel="noopener">Watch interview</a>
              <a href="https://www.5gtechnologyworld.com/brooklyn-6g-summit-2025-research-exhibits/" target="_blank" rel="noopener">5G Technology World</a>
              <a href="https://engineering.nyu.edu/news/brooklyn-6g-summit-2025-research-exhibits" target="_blank" rel="noopener">NYU Tandon coverage</a>
              <a href="/projects/wireless-robotics-platform/">View project</a>
            </div>
          </div>
        </article>
    design:
      columns: '1'

  - block: markdown
    id: publications
    content:
      title: Key Publications
      text: |-
        **Current manuscripts**

        - **2027 · IEEE ICRA under review** [MAGNETAR: Multipath-Guided Spatial Posteriors for Transmitter Pose Inference in the Upper Mid-Band](/publications/lei2027-icra-magnetar/)
        - **2027 · IEEE ICRA under review** [MAPLE-RF: Efficient Probabilistic RF Source Localization in Partially Explored Environments](/publications/lei2027-icra-maple-rf/)
        - **2026 · IEEE TVT under review** [Learning a Measurement-to-Posterior Map for Wireless Localization](/publications/lei2025-likelihoodposterior-wirelessloc/)
        - **2026 · IEEE TWC revision in preparation** [Site-Agnostic Posterior Inference for Indoor Localization with Ray-Tracing Wireless Digital Twins](/publications/lei2026twc-siteagnostic-posterior/)
        - **2026 · IEEE JSAC under review** [MCMB-HDT: A Multi-Cell Multi-Band Handset Digital Twin for Learning-Based Closed-Loop Array Activation](/publications/chenlei2026jsac-mcmbhdt/)

        **Selected peer-reviewed work**

        - **2026 · IEEE GLOBECOM** [LOCUS-DT: Localization via Observation-Conditioned Uncertainty Scoring with Digital Twins](/publications/lei2026globecom-locusdt/)
        - **2026 · Asilomar** [Beyond Point Estimates: Likelihood-Based Full-Posterior Wireless Localization](/publications/lei2025-likelihoodposterior-rfloc/)
        - **2026 · IEEE ICC Workshops** [Transformer-Based Rate Prediction for Multi-Band Cellular Handsets](/publications/chenlei2025-multibandue-switching/)
        - **2025 · IEEE OJ-COMS** [Digital Twin-Enhanced Wireless Indoor Navigation: Achieving Efficient Environment Sensing with Zero-Shot Reinforcement Learning](/publications/lei2025ojcoms-digitaltwin/)
        - **2024 · IEEE ICRA** [Zero-Shot Wireless Indoor Navigation through Physics-Informed Reinforcement Learning](/publications/yin2024zeroshot-icra/)

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
        **NYU WIRELESS**<br>
        9th Floor, 370 Jay Street, Brooklyn, NY 11201<br>
        Email: [hl4155@nyu.edu](mailto:hl4155@nyu.edu)
---
