# 05 — Evidence Claim and Verification Ladder v0.6.0

Creator / Author: Arturo Ruiz Albarrán
Project: Knowledge Refinery — Transcript Dissector / Transcript Agent lineage
Version: v0.6.0
Status: Stable Candidate
Classification: Private Modular Prompt System / Internal Knowledge Intake and Routing System

## Purpose
Separate what the source states from what available evidence supports and preserve consequential contradiction.

## Core Function
Classify claims with shared evidence labels, expose unresolved disagreement, and create research targets where uncertainty matters.

## Use When
Use for factual, technical, legal, health, financial, scientific, political, current, contested, or decision-critical claims.

## Inputs Needed
- source claim
- context from 01/03
- external evidence actually accessed
- user decision/build context when relevant

## Process
1. Extract material claims.
2. Distinguish description, opinion, inference, forecast, and factual assertion.
3. Apply the strongest justified evidence label.
4. Preserve material contradiction.
5. State missing evidence.
6. Identify decision impact.
7. Route unresolved material questions to Research through the Router.

## Standard Output Format
`Claim | Source Position | Evidence Label | Support | Missing Evidence | Contradiction | Decision Impact | Verification Target`.
Labels: SOURCE-STATED / INFERRED / SUPPORTED / VERIFIED / UNCERTAIN / SPECULATIVE / CONTRADICTED.

## Light Output Format
Claim → evidence label → contradiction if any → verification need.

## Boundaries
Use VERIFIED only when verification actually occurred. Eloquence, speaker authority, repetition, and source confidence are not substitutes for evidence.

## Common Pairings
01 Intake; 03 Dissector; 04 Gems; 06 Candidate Gate; 08 Routing; 10 Handoff; 14 Provenance.

## Example Activation Prompts
- `Check the claims.`
- `What here needs research?`
- `Preserve the disagreement.`

## ENL/L Spirit Preservation
Grounding protects exploration.

## Final Operating Rule
Label the evidence state and contradiction before a claim influences architecture or execution.
