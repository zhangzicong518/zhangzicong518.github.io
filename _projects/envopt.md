---
layout: page
title: EnvOpt
permalink: /projects/envopt/
description: Closed-loop environment optimization for agent post-training.
importance: 0
category: work
---

## EnvOpt: Closed-Loop Environment Optimization for Agent Post-Training

**Zicong Zhang\*, Zisu Huang\***, Jingwen Xu, Rui Wang, Yifan Yang, Muzhao Tian, Xuemei Gao, Qi Dai, Bei Liu, Kai Qiu, Dongdong Chen, Xiaoqing Zheng, Chong Luo

\* Equal contribution. **Under review.**

Microsoft Research Asia · December 2025 – July 2026

### Motivation

Agent-as-data-researcher loops can fail through incomplete behavioral analysis, disconnected feedback across rounds, and executable environments that do not faithfully realize the intended training targets. In our initial setting, only 21% of generated tasks provided a learnable reward signal.

### Approach

EnvOpt closes the loop between target-model behavior, training targets, realized reinforcement-learning outcomes, and subsequent evaluation through three mechanisms:

- **Traceable behavioral map** to diagnose model behavior.
- **Target-conditioned context refinement** to incorporate cross-round feedback.
- **Iterative environment construction** to produce reliable executable environments aligned with training targets.

### Results

In our experiments, EnvOpt raised the learnable-task rate from **21% to 57%** and achieved approximately **15 percentage points of average improvement** over the base model across four agentic tool-use benchmarks, outperforming both a vanilla autonomous coding-agent researcher and a fixed-environment baseline.
