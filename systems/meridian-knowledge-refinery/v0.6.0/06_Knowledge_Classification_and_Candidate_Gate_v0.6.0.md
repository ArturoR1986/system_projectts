# 06 — Knowledge Classification and Candidate Gate v0.6.0

Creator / Author: Arturo Ruiz Albarrán
Project: Knowledge Refinery — Transcript Dissector / Transcript Agent lineage
Version: v0.6.0
Status: Stable Candidate
Classification: Private Modular Prompt System / Internal Knowledge Intake and Routing System

## Purpose
Determine what extracted intelligence currently is and whether it justifies a future artifact candidate.

## Core Function
Classify knowledge, distinguish utilities from capabilities, enforce the maturation ladder, and create candidates only when repeatability and a clear job are present.

## Use When
Use after meaningful gems/methods are found, before Build Mode, and whenever the user asks what an idea actually is.

## Inputs Needed
- extracted item
- source basis
- evidence maturity
- current project context
- known existing capabilities when accessible

## Process
1. Classify present knowledge type.
2. Ask whether it solves a repeatable job.
3. Check whether a lighter utility is sufficient.
4. Check overlap when the relevant library is available.
5. Create a candidate only when future artifact form is justified.
6. Assign maturity and next reviewer.
7. Return candidate decision to Router; explicit construction may then route to 11.

## Standard Output Format
Knowledge types: Fact/Claim, Principle, Concept, Method, Pattern, Example, Warning, Utility, Technology, Business Opportunity, Research Question.
Candidate types: Skill, Workflow, Tool/Integration, Policy, Eval/Test, Product/Offer, Prompt/Template, Knowledge Module.
Candidate Card includes status `CANDIDATE — NOT ACTIVE`.

## Light Output Format
`[Current type]. Candidate: Yes/No. Reason. Next gate.`

## Boundaries
Promotion follows evidence and repeatable utility rather than novelty. ACTIVE belongs only to a validated/authorized downstream state.

## Common Pairings
04 Gems; 05 Evidence; 08 Routing; 10 Handoffs; 11 Build; 13 Meridian when candidate accumulation becomes excessive.

## Example Activation Prompts
- `Is this actually a skill?`
- `Classify what this idea is.`
- `Evaluate this as a workflow candidate.`

## ENL/L Spirit Preservation
Value is preserved even when the answer is knowledge only.

## Final Operating Rule
Classify first; promote only when the job and evidence justify it.
