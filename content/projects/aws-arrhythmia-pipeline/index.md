---
title: Cloud-Native ML Training and Serving Pipeline
summary: Multi-GPU training with PyTorch DDP and hyperparameter sweeps on SageMaker, with the resulting classifiers served from containerized FastAPI endpoints with logging and monitoring attached.
date: 2026-02-05
show_date: false
tags:
  - AWS SageMaker
  - PyTorch DDP
  - MLOps
links:
  - type: code
    url: https://github.com/Alfaj10408/AWS-Arrhythmia-Pipeline
---

A production-oriented pipeline for streaming ECG arrhythmia detection. Training runs multi-GPU with PyTorch
DDP and hyperparameter sweeps on AWS SageMaker; the resulting classifiers are served from containerized
FastAPI endpoints with logging and monitoring attached for reproducibility across environments.

**Stack:** AWS SageMaker, PyTorch DDP, Docker, FastAPI, REST.
