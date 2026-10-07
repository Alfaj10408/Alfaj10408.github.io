---
title: Self-Supervised Representation Learning for Sequential Signals
summary: Transformer encoders pretrained on unlabeled 1D signal corpora with a combined contrastive and masked-reconstruction objective, then evaluated on downstream sequence classification under transfer.
date: 2026-02-05
show_date: false
tags:
  - Self-Supervised Learning
  - Transformers
  - Time Series
links:
  - type: code
    url: https://github.com/Alfaj10408/SSL-ECG-Encoder
---

A self-supervised learning framework for ECG and other 1D physiological signals. Transformer encoders are
pretrained on unlabeled corpora with a combined contrastive and masked-reconstruction objective, and the
learned representations are evaluated on downstream arrhythmia classification with limited labels.

**Stack:** PyTorch, Transformers, contrastive learning, masked modeling.
