---
title: "ViPoser: Sparse-IMU Based Human Pose Estimation with Distilled Vision Foundation Priors"
collection: publications
category: conferences
permalink: /publication/2026-viposer
excerpt: 'A lightweight framework that distills human-structure priors from a vision foundation model (Sapiens) into a compact IMU-based pose estimator — achieving 10–30% lower error and near-zero anatomically implausible poses under sparse 1–3 IMU input.'
date: 2026-11-01
venue: 'ACM International Conference on Mobile Computing and Networking (MobiCom 2026)'
paperurl: 'http://fridge23.github.io/files/ViPoser.pdf'
citation: 'Hanyu Zeng, et al. (2026). &quot;ViPoser: Sparse-IMU Based Human Pose Estimation with Distilled Vision Foundation Priors.&quot; <i>ACM MobiCom 2026</i>.'
---

Estimating full-body pose from only one to three consumer-grade IMUs is highly under-constrained, and prior methods often produce physically implausible configurations. ViPoser analyzes the human-centric vision model **Sapiens** to locate the layers richest in biomechanical and skeletal knowledge (blocks 18–21), distills them into a compact 64-dim student Transformer, and integrates the distilled priors into a three-stage pipeline (local joint estimation → masked whole-body completion → global translation).

**Highlights**
- 10–30% lower pose error than IMUPoser and MobilePoser across DIP-IMU, TotalCapture, and the IMUPoser dataset (e.g., 13.94 cm MPJVE on DIP-IMU).
- Introduces the **Joint Violation Rate (JVR)** metric based on AAOS clinical range-of-motion limits; ViPoser reaches near-zero JVR (0.03%), an order of magnitude below baselines.
- Runs at ~9,200 FPS on a consumer RTX 3070 — ~7.7× faster than MobilePoser — suitable for real-time edge deployment.

[Download the paper here](http://fridge23.github.io/files/ViPoser.pdf)
