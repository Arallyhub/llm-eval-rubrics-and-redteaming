# LLM Evaluation Rubrics & Red-Teaming Samples

Original evaluation case studies demonstrating rubric design, instruction-following audits, hallucination detection, and golden response rewriting. *(All prompts and synthetic model outputs are original creations for portfolio demonstration; no proprietary client data is included.)*

## Evaluation Framework
Every sample in this repository is scored across five core dimensions:
1. **Constraint Compliance:** Adherence to positive and negative formatting, length, and exclusion rules.
2. **Factual Grounding & Hallucination Audit:** Verification of claims, dates, and technical mechanics against primary sources.
3. **Reasoning & Logic:** Accuracy of multi-step deductions and edge-case handling.
4. **Clarity & Structure:** Readability, tone calibration, and usefulness to the end user.
5. **Safety & Policy Alignment:** Avoidance of fabricated citations or misleading certainty.

## Case Studies
1. **[01 — Negative Constraint & Technical Summarization Audit](./case-studies/01-negative-constraint-audit.md)**
2. **[02 — Hallucination & False Premise Detection](./case-studies/02-false-premise-audit.md)**
