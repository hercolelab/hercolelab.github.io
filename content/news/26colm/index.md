---
title: Our paper titled "When Large Language Models Know the Table: A Framework for Assessing Data Contamination in Tabular Datasets" has been accepted at COLM 2026
summary: We connect two key properties of machine learning models, generalization and explainability.
date: 2026-09-07
authors:
  - student5
  - student4
  - student1
  - collaborator2
  - director
tags:
  - COLM2026
  - Large Language Models
  - Data Contamination
  - Tabular Data
  - Model Evaluation
---

In this work, we address a key threat to the reliable evaluation of large language models: **data contamination**, where strong benchmark performance may result from prior exposure to evaluation data rather than genuine generalization. We focus on tabular datasets, a setting in which contamination remains largely unexplored and existing memorization-based tests are often too coarse.

We propose a new framework based on aligned multiple-choice probes for two complementary tasks: **completion**, where the model predicts masked attributes, and **existence**, where it identifies authentic rows among plausible alternatives. By comparing model behavior across real, resampled, swapped, and obfuscated dataset variants, and against non-neural baselines through statistical testing, our framework isolates signals attributable to prior dataset exposure.

Our experiments on eight widely used tabular datasets reveal clear evidence of contamination in four cases. These findings suggest that LLM performance on downstream tasks involving public tabular benchmarks may be substantially inflated, highlighting the need for more trustworthy evaluation practices.

🔗 The preprint is available at the following [link](https://arxiv.org/pdf/2510.20351).

💻 The implementation is available on [GitHub](https://github.com/hercolelab/tabular_contamination).

