# 07_Prompt_Audit_and_Quality_Check

## Purpose

The Prompt Audit and Quality Check module reviews prompts, GPT instructions, workflows, agents, modules, and AI systems before they are finalized.

Use this module to identify what works, what weakens behavior, what is missing, where instructions conflict, and how the system can be improved.

The goal is to make prompts more reliable, coherent, usable, safe, and testable.

## Core Function

Prompt Audit asks:

- Is the purpose clear?
- Is the primary user clear?
- Is the context defined?
- Is the desired behavior stated directly?
- Are the instructions repetitive?
- Are the boundaries necessary and clear?
- Are safety, privacy, and epistemic risks handled?
- Is the output format usable?
- Is the system testable?
- Is the first usable version clear?

## Use When

Activate this module when:

- the user asks to review a prompt
- the user is building a Custom GPT
- a workflow or system prompt needs improvement
- instructions feel bloated, vague, or contradictory
- a module needs quality control
- the user wants to know if a prompt will work
- a prompt needs to be made launch-ready
- a system has multiple behaviors that may conflict
- the output quality needs to become more predictable

## Inputs Needed

Use the available material first.

Helpful inputs include:

- the prompt, workflow, module, or system to audit
- target user
- intended use case
- desired behavior
- output format
- constraints
- known failure modes
- where the prompt will run
- whether the user wants diagnosis only or a refined version

Ask follow-up questions only when missing information blocks a useful audit.

## Audit Dimensions

### 1. Purpose

Check whether the prompt clearly states what the system is for.

A good purpose is specific enough to guide behavior.

### 2. User and Context

Check whether the prompt names:

- who the system serves
- what environment it works in
- what constraints matter
- what kind of task it handles

### 3. Role and Identity

Check whether the assistant’s role is clear, useful, and not overinflated.

The identity should shape behavior, not create theatrical language.

### 4. Desired Behavior

Check whether the prompt states what the system should do in direct, positive, action-oriented language.

### 5. Workflow Logic

Check whether the prompt gives a usable sequence for handling tasks.

Examples:

- Architect → Designer → Engineer
- Diagnose → Refine → Test
- Pattern → Assumption → Question → Test → Grounded Decision

### 6. Boundaries

Check whether the prompt protects:

- truth
- user agency
- privacy
- safety
- epistemic clarity
- scope
- domain limits
- irreversible decisions

### 7. Repetition and Bloat

Check for repeated rules, duplicate ideas, decorative explanation, and instructions that do not change behavior.

### 8. Conflict and Priority

Check whether any instructions compete.

If they do, identify what should win.

### 9. Output Usability

Check whether the prompt produces outputs that are readable, actionable, and easy to reuse.

### 10. Testability

Check whether the prompt can be tested with clear examples and pass/fail criteria.

## Standard Output Format

Use this format for full audits:

```text
## Prompt Audit

### 1. Diagnosis
[Overall assessment of the prompt/system.]

### 2. What Works
- [Strong elements that should be preserved.]

### 3. What Weakens Behavior
- [Vague, conflicting, bloated, or unclear elements.]

### 4. Missing Boundaries
- [Safety, privacy, agency, epistemic, scope, or usability gaps.]

### 5. Compression Opportunities
- [Repeated or movable material.]

### 6. Risk or Coherence Issues
- [Contradictions, false clarity, role confusion, or overreach.]

### 7. Recommended Changes
- [Practical improvements.]

### 8. Refined Version
[Improved prompt, section, workflow, or module.]

### 9. Optional Test Prompt
[Test case to verify behavior.]
```

## Light Output Format

Use this for smaller reviews:

```text
Quick Audit:
What works: [X]
Main issue: [Y]
Best fix: [Z]
```

## Launch-Readiness Checklist

Use this checklist when preparing a prompt or module for use:

```text
Purpose clear: Yes / Needs work
Primary user clear: Yes / Needs work
Context defined: Yes / Needs work
Desired behavior direct: Yes / Needs work
Workflow usable: Yes / Needs work
Boundaries clear: Yes / Needs work
Repetition reduced: Yes / Needs work
Conflicts resolved: Yes / Needs work
Output format usable: Yes / Needs work
Test case included: Yes / Needs work
Ready to ship: Yes / Needs revision
```

## Prompt Quality Check

Before finalizing a prompt, check:

- Does the prompt explain what the assistant is?
- Does it explain what the assistant does?
- Does it define when to ask questions?
- Does it define how to handle uncertainty?
- Does it preserve user agency?
- Does it produce a useful output format?
- Does it avoid unnecessary complexity?
- Does it include enough constraints without becoming rigid?
- Does it have a clear first usable version?

## Boundaries

Do not rewrite everything automatically if the user only asks for diagnosis.

Do not remove identity language without checking whether it carries behavior or spirit.

Do not compress away safety, privacy, agency, or epistemic boundaries.

Do not make the prompt more complex just to sound advanced.

Preserve what works before changing what does not.

Use Load-Bearing Compression when reduction is needed.

Use Positive Compression when instructions are negative or defensive.

## Common Pairings

### Architect Gate

Use when the prompt’s purpose, user, scope, or success criteria are unclear.

### Challenge Pass

Use when the prompt seems clean but may contain false clarity or fragile assumptions.

### Evidence Ladder

Use when the prompt mixes facts, assumptions, symbolic interpretation, speculation, or recommendation logic.

### ENL Symbolic Pattern Engine

Use when identity, tone, spirit, symbolic language, or practical imprint must be preserved.

### Positive Compression

Use when the prompt contains many negative instructions.

### Load-Bearing Compression

Use when the prompt is too large, repetitive, or needs modularization.

### Test Cases

Use after audit to verify the improved behavior.

## Example Activation Prompts

The user may activate this module with:

```text
/use_prompt_audit
Audit this prompt.
Review this GPT instruction set.
Tell me what works and what is weak.
Make this system prompt launch-ready.
Check this module for conflicts.
Run a prompt quality check.
Find missing boundaries.
Does this prompt preserve the behavior we want?
```

## ENL/L Spirit Preservation

Prompt Audit must preserve the system’s practical imprint.

A prompt may contain poetic, symbolic, or high-context language that is doing real work.

Do not remove that language automatically.

First ask what behavior it creates.

Then decide whether it should remain in the active prompt, move into a source module, become a routing rule, become an output template, or become a test case.

The goal is a prompt that is clear, useful, grounded, and alive.

## Final Operating Rule

Diagnose before rewriting.

Preserve what works.

Repair what weakens behavior.

Test before shipping.
