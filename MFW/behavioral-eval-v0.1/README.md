# MFW Behavioral Evaluation Harness v0.1

Purpose: test whether an MFW candidate improves behavior, not merely wording.

## Governing order
1. Hard correctness/risk gates.
2. Outcome proof.
3. Generalization and regression.
4. Efficiency only after 1–3 pass.

## Promotion path
OBSERVED -> ATTRIBUTED -> CANDIDATE -> LOCAL-PASS -> HOLDOUT-PASS -> CANARY-PASS -> STABLE-SCOPE

## Required controls
- Frozen Baseline A and Candidate B
- Frozen benchmark version
- Environment fingerprint
- Representative regression set
- Shadow holdout isolated from development
- Critical-failure ledger
- Repeated paired trials when stochasticity matters
- Rollback on regression

## Current proof boundary
Historical MFW evidence reaches C4 in selected clean-matched cases.
C5 repeated/independent and C6 longitudinal/statistical remain unproven.
MFW-EX2 / GOLD remains candidate until behavioral evidence clears the gates.
