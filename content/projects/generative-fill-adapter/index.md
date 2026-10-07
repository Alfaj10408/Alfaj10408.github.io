---
title: Generative Fill Adapter — Semantic Inpainting with Diffusion Models
summary: Conditions Stable Diffusion on semantic segmentation masks through a ControlNet-style adapter fine-tuned with LoRA, with conditioning strategies compared in an ablation scored on FID, SSIM, and LPIPS.
date: 2026-02-04
show_date: false
tags:
  - Diffusion Models
  - ControlNet
  - LoRA
links:
  - type: code
    url: https://github.com/Alfaj10408/Generative-Fill-Adapter
---

A mask-conditional image editing pipeline built on Stable Diffusion. A ControlNet-style adapter, fine-tuned
with LoRA, conditions generation on semantic segmentation masks for text-guided generative fill. Conditioning
strategies are compared in an ablation scored on FID, SSIM, and LPIPS.

**Stack:** PyTorch, Stable Diffusion, ControlNet, LoRA, HuggingFace PEFT.
