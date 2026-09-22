---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

design:
  spacing: '3.25rem'

sections:
  - block: resume-biography-3
    id: hero
    content:
      username: me
      text: |-
        My research develops **RF sensing and probabilistic spatial inference for autonomous systems**. I start from sparse multipath and multimodal measurements, score competing spatial hypotheses with likelihood-based and neural posterior models, and calibrate wireless digital twins against physical measurements. The resulting beliefs support localization and joint pose inference, guide where robots sense and move, and inform closed-loop wireless decisions.

        <div class="academic-status" role="list" aria-label="Current academic status">
          <span role="listitem">NYU ECE Ph.D. Candidate</span>
          <span role="listitem"><a href="https://wireless.engineering.nyu.edu/">NYU WIRELESS</a></span>
          <span role="listitem">Advisor: <a href="https://engineering.nyu.edu/faculty/sundeep-rangan">Sundeep Rangan</a></span>
          <span role="listitem">Expected May 2027</span>
        </div>

        <div class="research-signals" aria-label="Research methodology from sensing to action">
          <div><span>01</span><strong>Physical sensing</strong><small>RF and multimodal evidence</small></div>
          <div><span>02</span><strong>Spatial belief</strong><small>Posterior inference and calibration</small></div>
          <div><span>03</span><strong>Decision and action</strong><small>Localization, sensing, and control</small></div>
        </div>

        <div class="hero-actions">
          <a href="#projects">Explore projects</a>
          <a href="#publications">Publications</a>
          <a href="/cvs/cv_academic.pdf">Academic CV</a>
          <a href="/cvs/CV_industrial.pdf">Industry resume</a>
        </div>
      headings:
        about: Research Focus
        education: Education
        interests: Research Interests
    design:
      css_class: hero-section
      background:
        gradient_mesh:
          enable: false
      name:
        size: md
      avatar:
        size: large
        shape: square

  - block: markdown
    id: research
    content:
      title: Research Program
      text: |-
        <p class="section-lede">A shared methodology connects the program: physical evidence is tested against model-aware hypotheses, retained as calibrated spatial belief, and actively refined through new measurements and actions.</p>

        <figure class="research-map-panel" aria-labelledby="research-map-caption">
          <a class="research-map-link" href="/media/research-program-overview.svg?v=20260921-4" target="_blank" rel="noopener" aria-label="Open the full-size research program map">
            <picture class="research-overview-picture">
              <source media="(max-width: 680px)" srcset="/media/research-program-overview-mobile.svg?v=20260921-4">
              <img src="/media/research-program-overview.svg?v=20260921-4" alt="Research pipeline that transforms sparse RF and multimodal evidence through model-aware probabilistic inference into calibrated position and pose beliefs, then uses uncertainty to guide localization, active sensing, navigation, and wireless decisions, with physical validation on the MobiFR3 robotic platform.">
            </picture>
          </a>
          <figcaption id="research-map-caption">
            <strong>One methodology across the program.</strong> Open the full-size map to follow the evidence, inference, and active-update pipeline in detail.
          </figcaption>
        </figure>
    design:
      css_class: research-program-section
      columns: '1'

  - block: collection
    id: projects
    content:
      title: Selected Projects
      text: Three flagship efforts define the current program, supported by earlier and complementary work and one mentored emerging direction.
      sort_by: weight
      order: asc
      filters:
        folders:
          - projects
        featured_only: true
      count: 6
    design:
      css_class: projects-section
      view: article-grid
      columns: 3
      fill_image: false
      show_date: false
      show_read_time: false
      show_read_more: false

  - block: markdown
    id: publications
    content:
      title: Selected Publications
      text: |-
        <p class="section-lede">Representative manuscripts and peer-reviewed work tracing the progression from wireless posterior inference to robot-facing spatial belief and action.</p>

        <div class="publication-columns">
          <section class="publication-column" aria-labelledby="current-work-heading">
            <p class="publication-group-label" id="current-work-heading">Current manuscripts</p>
            <ul>
              <li><strong>IEEE ICRA 2027 · under review</strong><a href="/publications/lei2027-icra-magnetar/">MAGNETAR: Multipath-Guided Spatial Posteriors for Transmitter Pose Inference in the Upper Mid-Band</a></li>
              <li><strong>IEEE ICRA 2027 · under review</strong><a href="/publications/lei2027-icra-maple-rf/">MAPLE-RF: Efficient Probabilistic RF Source Localization in Partially Explored Environments</a></li>
              <li><strong>IEEE TVT · under review</strong><a href="/publications/lei2025-likelihoodposterior-wirelessloc/">Learning a Measurement-to-Posterior Map for Wireless Localization</a></li>
              <li><strong>IEEE TWC · revision in preparation</strong><a href="/publications/lei2026twc-siteagnostic-posterior/">Site-Agnostic Posterior Inference for Indoor Localization with Ray-Tracing Wireless Digital Twins</a></li>
            </ul>
          </section>
          <section class="publication-column" aria-labelledby="peer-reviewed-heading">
            <p class="publication-group-label" id="peer-reviewed-heading">Selected peer-reviewed work</p>
            <ul>
              <li><strong>IEEE GLOBECOM 2026</strong><a href="/publications/lei2026globecom-locusdt/">LOCUS-DT: Localization via Observation-Conditioned Uncertainty Scoring with Digital Twins</a></li>
              <li><strong>Asilomar 2026</strong><a href="/publications/lei2025-likelihoodposterior-rfloc/">Beyond Point Estimates: Likelihood-Based Full-Posterior Wireless Localization</a></li>
              <li><strong>IEEE OJ-COMS 2025</strong><a href="/publications/lei2025ojcoms-digitaltwin/">Digital Twin-Enhanced Wireless Indoor Navigation</a></li>
              <li><strong>IEEE ICRA 2024</strong><a href="/publications/yin2024zeroshot-icra/">Zero-Shot Wireless Indoor Navigation through Physics-Informed Reinforcement Learning</a></li>
            </ul>
          </section>
        </div>

        <p class="publication-index-link"><a href="/publications/">View the full publication list</a></p>
    design:
      css_class: publications-section
      columns: '1'

  - block: markdown
    id: media
    content:
      title: In the Field
      text: |-
        <article class="featured-media-card">
          <a class="featured-media-visual" href="https://www.youtube.com/watch?v=2_3FGVCxYKY" target="_blank" rel="noopener" aria-label="Watch the Brooklyn 6G Summit 2025 interview">
            <img src="/media/6gsummit-interview.jpg" alt="FR3 robotic localization demonstration at the Brooklyn 6G Summit 2025" loading="lazy" decoding="async">
            <span class="featured-media-play" aria-hidden="true"><span>▶</span> Watch interview</span>
          </a>
          <div class="featured-media-copy">
            <p class="featured-media-kicker">Brooklyn 6G Summit 2025</p>
            <h3>MobiFR3 in a live research demonstration</h3>
            <p>I demonstrated our 10-GHz robotic RF platform and discussed how probabilistic localization can support indoor positioning when visual information is incomplete.</p>
            <div class="media-links" aria-label="Interview and media coverage">
              <a href="https://www.youtube.com/watch?v=2_3FGVCxYKY" target="_blank" rel="noopener">Video interview</a>
              <a href="https://www.5gtechnologyworld.com/brooklyn-6g-summit-2025-research-exhibits/" target="_blank" rel="noopener">5G Technology World</a>
              <a href="https://engineering.nyu.edu/news/brooklyn-6g-summit-2025-research-exhibits" target="_blank" rel="noopener">NYU Tandon</a>
              <a href="/projects/wireless-robotics-platform/">Project details</a>
            </div>
          </div>
        </article>
    design:
      css_class: field-section
      columns: '1'

  - block: markdown
    id: affiliation
    content:
      title: Academic Home
      text: |-
        <div class="academic-home-grid">
          <article class="affiliation-panel">
            <a class="lab-photo-link" href="/uploads/NYU_wireless.pdf" aria-label="Open NYU WIRELESS overview PDF">
              <img src="/media/lab.jpg" alt="NYU WIRELESS group photo" loading="lazy" decoding="async">
            </a>
            <div>
              <p class="panel-kicker">NYU WIRELESS</p>
              <h3>From wireless models to robots in the loop</h3>
              <p>At NYU WIRELESS, I align ray-traced wireless models with measured RF, form calibrated spatial beliefs, and validate them on the MobiFR3 robotic platform.</p>
              <a class="text-link" href="/uploads/NYU_wireless.pdf">Center overview</a>
            </div>
          </article>
          <article class="credentials-panel">
            <p class="panel-kicker">Education</p>
            <h3>Academic Background</h3>
            <dl>
              <div><dt>Ph.D.</dt><dd>New York University<br><span>Expected May 2027</span></dd></div>
              <div><dt>M.S.</dt><dd>Computer Engineering, NYU<br><span>2022</span></dd></div>
              <div><dt>B.E.</dt><dd>Electrical Engineering and Automation, CAU<br><span>2019</span></dd></div>
            </dl>
            <p class="credential-note">2023 Ernst Weber Fellowship · NYU Tandon</p>
          </article>
        </div>
    design:
      css_class: academic-home-section
      columns: '1'

  - block: markdown
    id: contact
    content:
      title: Contact
      text: |-
        <div class="contact-band">
          <div>
            <p class="panel-kicker">Research conversations and collaboration</p>
            <h3>Let’s connect across wireless sensing, localization, and autonomous systems.</h3>
          </div>
          <address>
            <strong>NYU WIRELESS</strong><br>
            9th Floor, 370 Jay Street<br>
            Brooklyn, NY 11201<br>
            <a href="mailto:hl4155@nyu.edu">hl4155@nyu.edu</a>
          </address>
        </div>
    design:
      css_class: contact-section
      columns: '1'
---
