---
title: 'TRACER accepted at NeurIPS 2026'
summary: TRACER helps generative recommender systems forget unwanted concepts while preserving the quality of other recommendations.
date: 2026-09-25
authors:
  - collaborator5
  - director
tags:
  - NeurIPS2026
  - Recommender Systems
  - Machine Unlearning
  - Generative Recommendation
---

We are pleased to announce that **"TRACER: Token ReAssignment for Concept ERasure in Generative Recommendation"** has been accepted at **NeurIPS 2026**. The paper is by Ziheng Chen, Jiali Cheng, Zezhong Fan, Hadi Amiri, Diyuan Wu, Gabriele Tolomei, and Yang Zhang.

Generative recommender systems encode items as sequences of semantic IDs. Because different items can share parts of these sequences, removing a sensitive or unwanted concept can also harm recommendations that should be retained. **TRACER** addresses this problem by reassigning concept-related items to alternative tokens and using a regularizer to preserve consistency among retained items.

Experiments on real-world recommendation datasets show effective concept removal with better preservation of recommendation quality than existing unlearning baselines. Read the [paper on arXiv](https://arxiv.org/abs/2606.07688).
