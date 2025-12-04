---
title: eXplainable AI Narratives
date: 2025-12-04
external_link: 
authors:
  - student1
  - student5
tags:
  - XAI Narratives
  - Large Language Models
  - Counterfactual Explanations
---

## Introduction

The field of **Explainable Artificial Intelligence** (XAI) has flourished, producing a vast array of methods to elucidate the internal mechanisms and decision-making rationales of opaque models. 
Classical XAI techniques—such as feature attribution, saliency mapping, rule extraction, and counterfactual reasoning—seek to expose the logic underlying a model’s predictions. However, despite their algorithmic sophistication, the outputs of these explainers are often intricate, mathematical, and complex for non-technical stakeholders to interpret. This mismatch between technical transparency and human interpretability remains a central challenge to the practical adoption of explainable AI.

To address this gap, researchers have increasingly turned to **Large Language Models** (LLMs) as a bridge between machine explanations and human understanding. By leveraging their generative and contextual reasoning abilities, LLMs can translate abstract or low-level explanatory signals into coherent, fluent, and audience-adapted narratives. This emerging synergy between XAI and LLMs gives rise to a novel paradigm of **XAI Narratives**, consisting in the generation of *linguistically grounded, cognitively resonant natural language explanations*.

## Problem Definition

Given a predictive model $f$, an instance $\bm{x}$, and a corresponding technical explanation $e_{tech} = g(f, \bm{x})$, the objective is to derive a narrative explanation $\varepsilon$ trough a generative function $h$ conditioned on a guiding prompt $p$:

$$\varepsilon = h(p, \bm{x}, e_{tech})$$

where $h$ transforms the structured information about the instance $\bm{x}$ contained in $e_{tech}$ into a linguistically coherent and semantically faithful textual narrative (see figure above).

## Our works
- [NATURAL LANGUAGE COUNTERFACTUAL EXPLANATIONS FOR GRAPHS USING LARGE LANGUAGE MODELS](https://arxiv.org/pdf/2410.09295?)
- [Enhancing XAI Narratives through Multi-Narrative Refinement and Knowledge Distillation](https://arxiv.org/pdf/2510.03134)
- [A Survey on Explainable AI Narratives based on Large Language Models](https://www.techrxiv.org/doi/full/10.36227/techrxiv.176282217.77757258)

## Thesis Projects

### Prerequisites
1. Less than two exams left in your career
2. Coding skills:
    - Python
    - Github
3. Basics of LLMs theory and usage

### 1. XAI Narratives for Time-Series
Integrate state-of-the-art XAI methods for time-series data in the XAI Narrative pipeline, focusing on how to represent the task to the (multimodal) LLM.

### 2. XAI Narratives for Images
Integrate state-of-the-art XAI methods for image data in the XAI Narrative pipeline, focusing on how to represent the task to the multimodal LLM.

### 3. Agentic AI Framework for advanced XAI Narratives on Large Graphs *(advanced)*
Develop an agentic framework that allows LLMs to create XAI Narratives on large-scale graphs, splitting the task into multiple sub-tasks to solve the problem of the context window of LLMs.