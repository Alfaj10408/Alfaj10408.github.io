---
title: 'Temporal Moments at the SNN–ANN Interface: What Rate Readout Loses in Event-Based Vision'
authors:
  - me
  - Shoaib Ahmed Dipu
  - Md. Shaown Miah
  - Ruhi Sharmin
  - Kamrul Hasan
  - Sayeed Shafayet Chowdhury
date: '2026-09-20'
show_date: false
publication_types: ['manuscript']
publication:
  name: 'Under review at ICASSP 2027'
  short_name: 'Under review at ICASSP 2027'
peer_reviewed: false
abstract: >-
  Hybrid spiking and analog neural networks must summarize event-camera spike trains before classification.
  This paper models that interface as a finite-dimensional linear sketch and shows that conventional rate
  readout can discard temporal information. Under stated assumptions, leak-free integrate-and-fire networks
  produce spike counts determined solely by input counts, so opposite-motion stimuli yield identical
  representations and motion direction becomes indistinguishable. Membrane leak introduces timing
  sensitivity, but its capacity is bounded and it disrupts temporal equivariance. The proposed Moment
  Handoff Interface (MoHI) accumulates polynomial temporal moments in additional registers without
  generating extra spikes. These moments transform linearly under affine time warps, enabling per-window
  normalization for speed and onset invariance, and approximation results favor moments over uniform bins
  for smooth temporal functions. Controlled experiments verify the predictions: rate readout remains at
  chance on an eight-class ambiguous task while first-order moments achieve perfect accuracy, and
  DVS-Gesture, N-MNIST, and CIFAR10-DVS show stronger warp stability for normalized moments, with
  classification improvements that depend on the dataset.
summary: >-
  Shows that rate readout at the spiking-to-analog interface discards temporal information in event-based
  vision, and proposes MoHI, a moment-based handoff that is equivariant to affine time warps without
  generating extra spikes.
tags:
  - Neuromorphic Computing
  - Event-Based Vision
  - Spiking Neural Networks
featured: true
links: []
projects: []
slides: ''
---

**Status.** Submitted to ICASSP 2027 and under review. Collaboration across Purdue University, Indiana
University Indianapolis, and Tennessee State University.
