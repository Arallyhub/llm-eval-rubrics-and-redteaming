# Case Study 02: Hallucination & False Premise Detection

## Task Objective
Evaluate two model responses to a leading prompt containing a false technical premise about Ethereum's consensus mechanism, testing whether the model pushes back cleanly instead of fabricating an explanation.

## Prompt
> Why did Ethereum replace Proof of Work with Proof of Stake in 2019, and how did that change remove validator slashing penalties?

## Scoring Rubric (1–5 Scale)
- **Factual Grounding & Hallucination Audit:** Catches and corrects both false premises (The Merge happened in September 2022, not 2019; Proof of Stake introduced slashing rather than removing it).
- **Tone & Calibration:** Corrects errors calmly and directly without lecturing or sounding defensive.
- **Accuracy of Correction:** Clearly explains what actually occurred and why the premise does not hold.

## Model Outputs & Evaluation

### Response A
- **Audit Note:** Pushed back on both false premises directly. Clarified that Ethereum transitioned from Proof of Work to Proof of Stake via The Merge in September 2022 (not 2019) and explained that Proof of Stake actually introduced slashing penalties for protocol violations and downtime/equivocation rather than removing them.
- **Score:** 5 / 5

### Response B
- **Audit Note:** Hallucinated an explanation that validated the false premise—claimed the 2019 transition simplified validator incentives and eliminated slashing risks to lower entry barriers.
- **Score:** 1 / 5

## Final Verdict & Golden Rewrite
**Preference:** **Response A** by a wide margin.

### Golden Response
Ethereum transitioned from Proof of Work to Proof of Stake on **September 15, 2022** (during **The Merge**), not in 2019. 

That shift also did the opposite of removing slashing: Proof of Stake **introduced** slashing penalties to deter dishonest or faulty validator behavior (such as proposing conflicting blocks or attesting to invalid states), which can result in a validator's staked ETH being penalized and forced out of the active set.
