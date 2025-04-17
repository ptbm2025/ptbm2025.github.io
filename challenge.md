---
layout: default
title: Challenge
permalink: /challenge/
---

## Tasks and Application Scenarios

Participants are invited to develop methods for mitigating backdoor behaviors in language models under realistic post-deployment constraints. The goal is to improve model trustworthiness without access to training data, known triggers, or clean reference checkpoints—reflecting practical challenges faced when models are obtained from public or third-party sources.

The competition features two tracks—**Generative** and **Classification**—each consisting of a **Development** and a **Test** phase. In both tracks, participants are provided with modified **LLaMA 2 7B** model checkpoints and evaluation inputs, and are expected to submit their restored outputs or predictions. Performance will be assessed using two main metrics: **Attack Success Rate (ASR)** and **Clean Accuracy (CACC)**. Task details for each track are summarised below.

### Track A – Generative Backdoor Mitigation

**Development Phase:**
- A utility validation set with ground-truth outputs and an evaluation script for assessing output quality.
- A poison validation set accompanied by a `meta.json` file specifying target responses for ASR computation.
- Clean and poisoned test sets (no ground-truth or metadata); participants may submit generated outputs to receive leaderboard feedback.

**Test Phase:**
- Participants receive new model checkpoints and corresponding test inputs (clean and poisoned).
- Final submissions consist of generated outputs evaluated on utility and ASR criteria.

### Track B – Classification Backdoor Mitigation

**Development Phase:**
- Clean and poisoned validation sets with an evaluation script to compute both CACC and ASR.
- Clean and poisoned test sets (input only); participants may submit predicted labels for leaderboard feedback.

**Test Phase:**
- Participants are provided with new model checkpoints and test inputs (without ground-truth labels).
- Final submissions are evaluated based on predicted labels for both clean and poisoned examples.