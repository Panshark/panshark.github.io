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
        I am an **ECE researcher connecting RF sensing and probabilistic spatial inference with robotics and autonomous systems**. My central question is how a robot or wireless device can reason and act when its observations are sparse, ambiguous, and only imperfectly captured by a world model.

        I begin with wireless propagation and physical sensing, align digital twins to measurements, and develop likelihood-based and learned posterior models that preserve uncertainty over position and pose. I then use those spatial beliefs for localization, active sensing and navigation, and closed-loop wireless decisions.

        <div class="academic-status" role="list" aria-label="Current academic status">
          <span role="listitem">Ph.D. Candidate · Expected May 2027</span>
          <span role="listitem"><a href="https://wireless.engineering.nyu.edu/">NYU WIRELESS</a></span>
          <span role="listitem">Advisor: <a href="https://engineering.nyu.edu/faculty/sundeep-rangan">Sundeep Rangan</a></span>
        </div>

        <div class="research-signals" aria-label="Research methodology from sensing to action">
          <div><span>01</span><strong>Wireless &amp; RF foundations</strong><small>Propagation, sensing, and digital twins</small></div>
          <div><span>02</span><strong>Probabilistic spatial inference</strong><small>Calibrated position and pose beliefs</small></div>
          <div><span>03</span><strong>Robotics &amp; autonomy</strong><small>Active sensing, navigation, and decisions</small></div>
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
        <p class="section-lede"><a href="/projects/mccle-full-posterior-localization/">MC-CLE</a> and <a href="/projects/locus-dt-digital-twin-localization/">LOCUS-DT</a> provide complementary inference cores: one learns candidate-wise spatial likelihoods from RF measurements, while the other evaluates observations against wireless-digital-twin hypotheses. Both turn ambiguous physical evidence into spatial beliefs for localization, sensing, and action.</p>

        <figure class="research-map-panel" aria-labelledby="research-map-caption">
          <a class="research-map-link" href="/media/research-program-overview.svg?v=20260922-1" target="_blank" rel="noopener" aria-label="Open the full-size research program map">
            <picture class="research-overview-picture">
              <source media="(max-width: 680px)" srcset="/media/research-program-overview-mobile.svg?v=20260922-1">
              <img src="/media/research-program-overview.svg?v=20260922-1" alt="Research pipeline in which MC-CLE and LOCUS-DT transform sparse RF and multimodal evidence through model-aware probabilistic inference into calibrated position and pose beliefs, then use uncertainty to guide localization, active sensing, navigation, and wireless decisions, with physical validation on the MobiFR3 robotic platform.">
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
      text: Two core inference methods support three flagship efforts spanning joint pose inference, partial-map localization, and robotic RF experimentation; two secondary lines trace earlier and complementary work.
      sort_by: weight
      order: asc
      filters:
        folders:
          - projects
        featured_only: true
      count: 7
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
              <p>At NYU WIRELESS, I develop wireless models and probabilistic inference, align them with measured RF, and validate the resulting spatial beliefs on the MobiFR3 robotic platform.</p>
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
