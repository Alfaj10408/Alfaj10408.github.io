---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2026-10-07
type: landing

sections:
  - block: resume-biography-3
    content:
      username: me
      text: ''
      button:
        text: Download CV
        url: uploads/alfaj-uddin-ahmed-cv.pdf
      headings:
        about: About
        education: Education
        interests: Research Interests
    design:
      background:
        gradient_mesh:
          enable: true
      name:
        size: md
      avatar:
        size: large
        shape: circle

  - block: focus-areas
    id: research
    content:
      title: Research
      subtitle: Four directions, one question
      text: |-
        How do learned systems fail, and how should we train and evaluate them so that those failures become
        measurable and fixable? Each direction below pairs a precise failure characterization with a method
        that targets it.
      items:
        - name: Failure Composition in Long-Horizon LLM Execution
          description: |-
            Benchmark accuracy hides *how* language models fail on multi-step tasks. An exact-simulator
            evaluation separates decision errors, state errors, token exhaustion, malformed outputs, and
            noncompliance. On the Qwen3 family, failure composition shifts with scale without a monotonic
            law: smaller models choose wrong moves, larger models choose correct moves but misreport the
            resulting state. Interventions redistribute failures rather than removing them. Under review at ICLR 2027.
          icon: hero/cpu-chip
          gradient: from-indigo-500 to-blue-500
          status: active
          topics:
            - LLM evaluation
            - Reasoning
            - Qwen3 · vLLM
          cta:
            text: Read the summary
            url: /publications/benchmark-score-failure-composition/
        - name: Evidence-Grounded Vision-Language Models
          description: |-
            Vision-language models answer confidently from blank or unrelated images, a failure we call
            *mirage*. TIDE pairs each question with its correct image, a blank image requiring refusal,
            and a same-domain wrong image requiring refusal, with a population-level guarantee that
            image-blind predictors are suboptimal. Across six VLMs, blank-image mirage drops to zero and
            out-of-domain variation narrows from 0.473 to 0.042. Manuscript in final preparation for CVPR 2027.
          icon: hero/eye
          gradient: from-teal-500 to-emerald-500
          status: active
          topics:
            - VLM grounding
            - Abstention
            - QLoRA at 2B–32B
          cta:
            text: Read the summary
            url: /publications/mirage-tide/
        - name: Temporal Information at the Spiking–Analog Interface
          description: |-
            Hybrid spiking–analog networks summarize event-camera spike trains before classification.
            Modeling that interface as a linear sketch shows rate readout from leak-free spiking
            front-ends cannot distinguish opposite-motion stimuli. MoHI accumulates polynomial temporal
            moments in extra registers, without extra spikes, and transforms linearly under affine time
            warps, enabling speed- and onset-invariant readout. Under review at ICASSP 2027.
          icon: hero/bolt
          gradient: from-amber-500 to-orange-500
          status: active
          topics:
            - Event cameras
            - Spiking networks
            - DVS-Gesture · N-MNIST · CIFAR10-DVS
          cta:
            text: Read the summary
            url: /publications/temporal-moments-snn-ann-interface/
        - name: Generative Augmentation for Pediatric Fracture Detection
          description: |-
            Dissertation work on ML for pediatric fracture and non-accidental trauma detection from
            radiographs, where a center may see only a handful of confirmed cases per year. The pipeline
            couples a mask-conditional latent diffusion model in a VQ-VAE latent space, with
            ControlNet-style conditioning on radiologist-delineated lesion masks, to transformer detection
            and few-shot classification. A multi-view fusion pilot (manuscript in preparation) established
            that cross-view max-fusion recovers recall but inflates false positives at the score level.
            IRB-approved data collection with pediatric radiology collaborators at Riley Hospital for Children.
          icon: hero/beaker
          gradient: from-rose-500 to-pink-500
          status: active
          topics:
            - Latent diffusion
            - Rare-event detection
            - Pediatric radiology
    design:
      layout: cards
      columns: 2

  - block: markdown
    content:
      title: How I work
      text: |-
        **Pre-registered decision gates.** Kill criteria are written before GPU budget is committed; seven
        research directions have been retired this way. **Evaluation as infrastructure.** The LLM results
        rest on a harness with 810 automated tests, SHA-256-pinned prompts, parser audits, token-budget
        controls, and resumable grid runners for multi-day unattended sweeps. **Null results are reported.**
        An apparent scale-dependent trend across the Qwen3-VL ladder was traced to a projector co-scaling
        artifact and documented as such.
    design:
      columns: '1'

  - block: collection
    id: publications
    content:
      title: Publications & Manuscripts
      text: Status labels are exact. Under-review and in-preparation work is listed as such until accepted.
      count: 0
      filters:
        folders:
          - publications
    design:
      view: citation

  - block: collection
    id: projects
    content:
      title: Selected Open-Source Projects
      text: Code on [GitHub](https://github.com/Alfaj10408).
      count: 6
      filters:
        folders:
          - projects
    design:
      view: article-grid
      columns: 3
      show_date: false
      show_read_time: false
      show_read_more: false

  - block: contact-info
    id: contact
    content:
      title: Contact
      subtitle: Open to research collaborations and Summer 2027 research internships.
      visit_title: Where I am
      connect_title: Reach me
      address:
        lines:
          - Weldon School of Biomedical Engineering
          - Purdue University
          - West Lafayette, IN, USA
      email: ahmed436@purdue.edu
      social:
        - icon: brands/github
          url: https://github.com/Alfaj10408
        - icon: brands/linkedin
          url: https://www.linkedin.com/in/alfaj-uddin-ahmed-0a5ab514a/
        - icon: academicons/google-scholar
          url: https://scholar.google.com/citations?user=mGQcwU4AAAAJ&hl=en
        - icon: academicons/orcid
          url: https://orcid.org/0009-0004-4991-6551
        - icon: brands/x
          url: https://x.com/AlfajUddin10408
      show_form: false
---
