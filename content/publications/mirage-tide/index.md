---
title: 'Why Models See Mirages: An Evidence-Starvation Theory of Ungrounded Multimodal Reasoning, and TIDE, a Training Objective That Provably Removes It'
authors:
  - me
  - et al.
date: '2026-09-10'
show_date: false
publication_types: ['manuscript']
publication:
  name: 'Manuscript in final preparation for CVPR 2027'
  short_name: 'Manuscript in final preparation for CVPR 2027'
peer_reviewed: false
abstract: >-
  Vision-language models often answer questions despite receiving blank or unrelated images, a failure we
  call mirage. Standard cross-entropy training permits this behavior: answers predictable from the question
  alone provide little incentive to use visual evidence, and unsupported inputs never reward abstention.
  TIDE pairs each question with its correct image and answer, a blank image requiring refusal, and an
  incorrect image from the same domain requiring refusal. Under stated assumptions, the population
  objective makes image-blind predictors suboptimal by at least log 3 nats and preserves optimal behavior
  on valid inputs; these guarantees concern the theoretical optimum rather than finite trained models.
  Experiments evaluate six models spanning multiple architectures, including cross-attention, using LoRA
  training and an image-aware judge. TIDE reduces blank-image mirage to zero across all models, increases
  valid-image answering rates, and narrows between-model variation on unseen out-of-domain images from
  0.473 to 0.042. In-domain wrong-image mirage remains at 27.8–34.8%, and representation-level grounding
  alone does not reduce blank-image mirage on converged models.
summary: >-
  Characterizes the "mirage" failure in which VLMs answer from blank or unrelated images, explains it as
  evidence starvation under cross-entropy training, and introduces TIDE, a training objective that
  drives blank-image mirage to zero across six models.
tags:
  - Vision-Language Models
  - Grounding
  - Hallucination
featured: true
links: []
projects: []
slides: ''
---

**Status.** Manuscript in final preparation for CVPR 2027; an OpenReview preprint is forthcoming and will
be linked here.

**Role.** Fine-tuned Qwen3-VL at 2B, 4B, 8B, and 32B with 4-bit QLoRA, traced an apparent scale-dependent
trend across the model ladder to a projector co-scaling artifact (reported as a documented null result),
and showed that representation-level grounding alone does not reduce blank-image mirage on converged models.
