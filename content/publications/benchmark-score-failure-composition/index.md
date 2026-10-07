---
title: 'A Benchmark Score Is Not a Property of a Model: Failure Composition Reorganizes Across Operating Regimes'
authors:
  - me
  - et al.
date: '2026-09-30'
show_date: false
publication_types: ['manuscript']
publication:
  name: 'Under review at ICLR 2027'
  short_name: 'Under review at ICLR 2027'
peer_reviewed: false
abstract: >-
  Benchmark accuracy reports how often a language model succeeds on a multi-step task, not how it fails.
  This work builds an exact-simulator evaluation that separates correct responses from decision errors,
  state errors, token exhaustion, malformed outputs, and noncompliance, and applies it to the Qwen3 family
  across reasoning-on and reasoning-off operating regimes with Clopper–Pearson and clustered uncertainty
  estimates. Failure composition shifts with scale without following a monotonic law: smaller models
  primarily choose incorrect moves, while larger models choose correct moves but misreport the resulting
  state. Interventions redistribute failures rather than removing them. Position labels reduce Qwen3-4B
  state errors from 50.6% to 0.6% while introducing formatting failures; invariant constraints eliminate
  invalid states but leave overall state error unresolved; self-consistency often replaces decision errors
  with state errors rather than correct answers. A preregistered prediction rule identifies regimes where
  reasoning interventions yield larger gains. Replication on Tower of Hanoi and a second model family
  supports the conclusion that evaluations should measure overall correctness alongside failure
  redistribution.
summary: >-
  An exact-simulator evaluation that decomposes LLM failures on long-horizon tasks, showing that failure
  composition reorganizes across model scale and reasoning regimes, and that common interventions
  redistribute failures rather than remove them.
tags:
  - Large Language Models
  - Evaluation
  - Reasoning
featured: true
links: []
projects: []
slides: ''
---

**Status.** Submitted to ICLR 2027 and under review. A public preprint link will be added here when available.

**Role.** Built the exact-simulator evaluation and the harness behind the results: 810 automated tests,
SHA-256-pinned verbatim prompts, parser audits, token-budget controls, and resumable grid runners for
unattended multi-day GPU sweeps. Ran 800-sample reasoning-on/off grids on Qwen3 models served through vLLM
on dual-GPU nodes.
