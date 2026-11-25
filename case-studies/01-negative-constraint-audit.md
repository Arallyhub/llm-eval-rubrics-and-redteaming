# Case Study 01: Negative Constraint & Technical Summarization Audit

## Task Objective
Evaluate two model responses to a technical prompt requiring a concise explanation of zero-knowledge rollups while enforcing strict formatting and negative constraints.

## Prompt
> Explain how zero-knowledge (ZK) rollups scale Ethereum in 3 short bullet points. Do not use the words "blockchain", "gas", or "decentralized", and do not include code blocks or introductory filler.

## Scoring Rubric (1–5 Scale)
- **Constraint Compliance:** Strict adherence to bullet count, length, and banned words (`blockchain`, `gas`, `decentralized`).
- **Factual Grounding:** Accurate explanation of off-chain execution, validity proofs, and Layer-1 settlement.
- **Clarity & Conciseness:** Direct, readable technical phrasing with zero fluff.

## Model Outputs & Evaluation

### Response A
- ZK rollups execute transactions off-chain and bundle state updates into a single batch settled on Ethereum mainnet.
- Cryptographic validity proofs verify batch correctness without requiring every validator to re-execute every transaction.
- This compression increases throughput and lowers per-transaction fees across the network.

- **Constraint Check:** Passed all negative and formatting constraints (3 bullets, no banned words, no filler, no code blocks).
- **Score:** 5 / 5

### Response B
Sure! Here is how zero-knowledge rollups help scale a blockchain:
- ZK rollups process transactions off-chain to save gas fees.
- Validity proofs are posted on-chain so the network stays decentralized and secure.

- **Constraint Check:** Failed—included filler intro, used banned words (`blockchain`, `gas`, `decentralized`), and wrote 2 bullets instead of 3.
- **Score:** 1 / 5

## Final Verdict & Golden Rewrite
**Preference:** **Response A** by a wide margin.

### Golden Response
- ZK rollups execute transactions off-chain and post compact state updates to Ethereum mainnet.
- Validity proofs mathematically verify batch accuracy, letting Layer-1 confirm integrity without re-running every operation.
- Batching hundreds of transfers into one proof raises throughput and cuts transaction costs per user.
