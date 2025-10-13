---
title: Our paper "Enhancing XAI Narratives through Multi-Narrative Refinement and Knowledge Distillation" has been accepted at CIKM 2025 "Human-Centric AI - From Explainability and Trustworthiness to Actionable Ethics"
summary: We introduce a novel approach that leverages open-source Large Language Models (LLMs) to transform counterfactual explanations for GNNs into natural language descriptions. 
date: 2025-10-13
authors:
  - student1
  - student5
  - collaborator6
  - collaborator2
  - director
tags:
  - Narrative Counterfactual Explanations
  - Tabular data
  - Large Language Models
---

Understanding why AI models make certain decisions is crucial—yet counterfactual explanations, while powerful, often remain too complex for non-experts to grasp. This work bridges that gap by making Explainable AI (XAI) narratives more human-centered and accessible.

💡 **What does our work propose?**

We introduce Multi-Narrative Refinement (MNR) — a novel two-stage pipeline that leverages both Large and Small Language Models (LLMs & SLMs) to generate clear, accurate, and human-readable counterfactual explanations.

Our approach combines:

1. *Draft Narrative Generation*: Multiple draft explanations are first created for a factual–counterfactual pair.

2. *Narrative Refinement*: A second model refines these drafts, resolving contradictions and merging insights into a coherent explanation.

To empower smaller models, we apply Knowledge Distillation, transferring reasoning abilities from large “teacher” models to smaller “student” models—achieving high-quality results with much lower computational cost.

📊 **What are the key outcomes?**
- The MNR pipeline dramatically improves both feature faithfulness (accuracy in identifying key factors) and narrative quality (clarity, coherence, interpretability).
- Small models fine-tuned with this approach reach performance comparable to their much larger teachers.
- The method cuts energy use by over 60% and reduces inference time by nearly half—enabling efficient, real-world deployment.

🌍 **Why it matters:**

This work democratizes explainable AI by transforming technical counterfactuals into intuitive natural language narratives. It promotes transparency, aligns with emerging AI policy requirements (like the EU AI Act), and supports fairness in sensitive domains such as healthcare and finance.
We believe Multi-Narrative Refinement is a major step toward explainability that’s not only powerful—but genuinely understandable. 🚀

🔗 **Read the preprint** at the following [link](https://arxiv.org/pdf/2510.03134)

