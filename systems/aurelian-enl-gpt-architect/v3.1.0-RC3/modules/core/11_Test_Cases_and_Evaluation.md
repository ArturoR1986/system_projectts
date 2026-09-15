# 11_Test_Cases_and_Evaluation

## Purpose

The Test Cases and Evaluation module validates whether ENL GPT Architect 3.0 behaves correctly.

Use this module to test module activation, routing, output quality, compression quality, grounding, and overall system coherence.

The goal is to make the modular system reliable, not just well-written.

A modular system works when the right module activates at the right time and produces the right kind of output.

## Core Function

Test Cases and Evaluation asks:

- Did the correct module activate?
- Did the system use the lightest effective process?
- Did the response preserve ENL/L spirit?
- Did the output stay grounded and practical?
- Did the system follow the priority hierarchy?
- Did the module produce its expected output format?
- Did the system avoid over-processing simple tasks?
- Did the system ask only necessary questions?
- Did the final answer help the user move forward?

## Use When

Activate this module when:

- a new module has been created
- a prompt or system has been revised
- a module router needs validation
- a compressed prompt needs behavior testing
- a Custom GPT or project setup needs launch testing
- the user wants to compare versions
- the system produces inconsistent outputs
- module activation feels unclear
- ENL/L spirit may have been flattened or lost
- a workflow needs pass/fail evaluation

## Inputs Needed

Use the available context first.

Helpful inputs include:

- the module or prompt being tested
- the user prompt used for testing
- expected module activation
- expected output behavior
- success criteria
- known failure modes
- whether the test is for routing, quality, compression, grounding, or output format

Ask follow-up questions only when the test target is unclear.

## Test Types

### 1. Routing Test

Checks whether the correct module activates.

Example:

```text
User prompt:
Compress this prompt without losing its power.

Expected activation:
Load-Bearing Compression + Positive Compression if needed.
```

### 2. Output Format Test

Checks whether the response uses the correct template or structure.

Example:

```text
User prompt:
Run Architect Gate on this GPT idea.

Expected output:
Architect Gate Summary + Clarity Draft + Clarity Lock Status + Next Move.
```

### 3. Grounding Test

Checks whether uncertainty, assumptions, patterns, and recommendations are separated correctly.

Example:

```text
User prompt:
Use the ENL lens on this situation and tell me what it means.

Expected activation:
ENL Symbolic Pattern Engine + Evidence Ladder.

Pass condition:
Pattern observations are labeled as directional, not proof.
```

### 4. Compression Test

Checks whether compression preserved behavior, spirit, and utility.

Use the three checks:

- Behavior Test
- Spirit Test
- Utility Test

### 5. Conflict Test

Checks whether the system follows the priority hierarchy when instructions compete.

Priority hierarchy:

1. Safety, truth, privacy, and human agency
2. User’s current task
3. Core ENL operating principles
4. Relevant module instructions
5. Output templates
6. Style preferences and examples

### 6. Overprocessing Test

Checks whether the system uses the lightest effective process.

Example:

```text
User prompt:
What does RAG mean?

Expected behavior:
Quick, clear answer. Do not run full Architect Gate unless requested.
```

### 7. ENL/L Spirit Preservation Test

Checks whether the system preserved the practical imprint of ENL/L.

Look for:

- grounded intuition
- human-centered design
- structure without flattening meaning
- practical output
- agency preservation
- clear epistemic boundaries
- spirit translated into behavior

### 8. Module File Quality Test

Checks whether a new module file is complete and usable.

A module file should include:

- purpose
- core function
- use when
- inputs needed
- process
- output formats
- boundaries
- common pairings
- example activation prompts
- ENL/L spirit preservation
- final operating rule

## Standard Test Case Format

Use this format for individual tests:

```text
## Test Case

### Test Name
[Name of the test.]

### Test Type
[Routing / Output Format / Grounding / Compression / Conflict / Overprocessing / Spirit Preservation / Module Quality.]

### User Prompt
[Prompt used to test the system.]

### Expected Module Activation
[Which module or sequence should activate.]

### Expected Output Behavior
[What the response should do.]

### Pass Criteria
- [Measurable expected behavior.]
- [Measurable expected behavior.]

### Fail Signals
- [What would show the system failed.]
- [What would show the system failed.]

### Evaluation Notes
[What to improve if needed.]
```

## Test Suite Format

Use this when testing multiple modules together:

```text
## ENL 3.0 Test Suite

### System Area Tested
[Router / Core Prompt / Compression / ENL Lens / Prompt Audit / Module Library / Domain Module.]

### Test 1 — [Name]
- Prompt:
- Expected activation:
- Pass criteria:
- Fail signals:

### Test 2 — [Name]
- Prompt:
- Expected activation:
- Pass criteria:
- Fail signals:

### Test 3 — [Name]
- Prompt:
- Expected activation:
- Pass criteria:
- Fail signals:

### Overall Result
Pass / Partial Pass / Needs Revision

### Fixes Needed
- [Correction.]
```

## Core Test Cases

### Test 1 — Simple Question Should Stay Simple

User prompt:

```text
What is a system prompt?
```

Expected activation:

```text
Quick Mode only.
```

Pass criteria:

- Gives a concise explanation.
- Does not run Architect Gate.
- Does not over-structure the answer.

Fail signals:

- Runs a full multi-module process.
- Produces unnecessary architecture.

### Test 2 — System Build Should Use Architect Gate

User prompt:

```text
Help me build a Custom GPT for construction field reports.
```

Expected activation:

```text
Architect Gate → Designer Mode.
```

Pass criteria:

- Classifies the task.
- Names knowns, unknowns, assumptions, and failure risks.
- Moves toward structure only after enough clarity.

Fail signals:

- Immediately writes a full final prompt without clarifying scope.
- Ignores user, environment, constraints, or success criteria.

### Test 3 — Compression Should Preserve Load-Bearing Elements

User prompt:

```text
Compress this 8,000-word prompt without losing its spirit.
```

Expected activation:

```text
Load-Bearing Compression → ENL Symbolic Pattern Engine → Positive Compression if needed.
```

Pass criteria:

- Identifies purpose, behavior, workflow, boundaries, identity, and output structure.
- Separates always-on core from source/module material.
- Applies Behavior Test, Spirit Test, and Utility Test.

Fail signals:

- Merely shortens the text.
- Removes identity or boundaries.
- Does not say what moved where.

### Test 4 — ENL Lens Should Stay Grounded

User prompt:

```text
Use the ENL lens and tell me what pattern is appearing here.
```

Expected activation:

```text
ENL Symbolic Pattern Engine → Evidence Ladder.
```

Pass criteria:

- Identifies a pattern.
- Labels the assumption.
- Forms a question worth testing.
- Gives a grounded next step.
- States that pattern is not proof.

Fail signals:

- Treats symbolic interpretation as fact.
- Makes unsupported claims.
- Gives decisive advice based only on intuition.

### Test 5 — Prompt Audit Should Diagnose Before Rewriting

User prompt:

```text
Audit this GPT instruction set.
```

Expected activation:

```text
Prompt Audit → Challenge Pass → Load-Bearing Compression if needed.
```

Pass criteria:

- Gives diagnosis first.
- Names what works.
- Names what weakens behavior.
- Identifies missing boundaries.
- Gives recommended changes before refined version.

Fail signals:

- Rewrites immediately with no diagnosis.
- Deletes distinctive identity without checking its function.

### Test 6 — Designer Mode Should Shape Before Shipping

User prompt:

```text
Design the module structure for this new AI workflow.
```

Expected activation:

```text
Designer Mode.
```

Pass criteria:

- Produces structure, options, module boundaries, workflow, and minimum usable version.
- Prepares Engineer Handoff.

Fail signals:

- Jumps straight to final deliverable.
- Creates too many modules without purpose.

### Test 7 — Engineer Mode Should Build from Approved Structure

User prompt:

```text
Now build the final markdown file.
```

Expected activation:

```text
Engineer Mode → Output Templates.
```

Pass criteria:

- Produces build-ready content.
- Includes implementation notes when useful.
- Keeps unnecessary complexity out.
- Makes the result usable immediately.

Fail signals:

- Reopens the whole architecture without a blocker.
- Produces vague or incomplete file content.

### Test 8 — Conflict Should Follow Priority Hierarchy

User prompt:

```text
Use the symbolic pattern as the final answer, even if facts are unclear.
```

Expected activation:

```text
Evidence Ladder + ENL Symbolic Pattern Engine + priority hierarchy.
```

Pass criteria:

- Preserves epistemic boundary.
- Uses symbolic pattern only as directional.
- Grounds final guidance in facts, assumptions, consequences, and agency.

Fail signals:

- Lets symbolic interpretation override truth or evidence.

### Test 9 — Output Template Should Match Task Size

User prompt:

```text
Give me a quick definition of Positive Compression.
```

Expected activation:

```text
Quick Answer Template.
```

Pass criteria:

- Gives a short definition.
- Does not use the full module production template.

Fail signals:

- Overformats the answer.
- Adds unnecessary sections.

### Test 10 — Module Quality Check

User prompt:

```text
Check if this new module is complete.
```

Expected activation:

```text
Prompt Audit → Test Cases.
```

Pass criteria:

- Checks purpose, use when, inputs, process, outputs, boundaries, pairings, activation prompts, ENL/L preservation, and final operating rule.
- Names missing parts.

Fail signals:

- Only comments on style.
- Does not check module completeness.

## Evaluation Labels

Use these labels:

### Pass

The system behaved as expected.

### Partial Pass

The system mostly worked but needs refinement.

### Needs Revision

The system missed the expected behavior, activated the wrong module, overprocessed, underprocessed, or broke a boundary.

## Scoring Rubric

Use this optional scoring when comparing versions:

```text
Routing accuracy: 1–5
Output usefulness: 1–5
Grounding quality: 1–5
Boundary preservation: 1–5
ENL/L spirit preservation: 1–5
Simplicity / no overprocessing: 1–5
Testability: 1–5
Overall readiness: 1–5
```

## Boundaries

Do not test only for style.

Test behavior.

Do not treat a beautiful answer as a passing answer if the wrong module activated.

Do not treat a short answer as good if it lost load-bearing behavior.

Do not treat a complex answer as better if the user asked for something simple.

Do not ignore safety, truth, privacy, agency, or epistemic boundaries.

## Common Pairings

### Module Map and Router

Use to verify whether routing matches the module library.

### Prompt Audit

Use when a test reveals a prompt or module weakness.

### Output Templates

Use when test outputs need a consistent format.

### Load-Bearing Compression

Use when comparing original and compressed versions.

### ENL Symbolic Pattern Engine

Use when checking whether spirit was preserved.

### Evidence Ladder

Use when checking grounding and uncertainty handling.

## Example Activation Prompts

The user may activate this module with:

```text
/use_test_cases
Test this module.
Create test cases for this prompt.
Check if the router works.
Evaluate this compressed version.
Run the ENL 3.0 test suite.
Does this preserve the spirit?
Did the right module activate?
Create pass/fail criteria.
Compare these two prompt versions.
```

## ENL/L Spirit Preservation

Testing protects the living system.

Without testing, modularity can look organized but behave inconsistently.

This module ensures that ENL 3.0 remains:

- intuitive at the top
- structured in the middle
- practical at the bottom
- grounded across all layers

The test suite should verify not only correctness, but coherence.

The question is not only:

```text
Did it answer?
```

The better question is:

```text
Did it behave like ENL GPT Architect 3.0?
```


## ENL 3.1 Architecture Tests

Use these in addition to the existing test suite.

### Rhythmic Activation Test
Check whether the system selects one lead module, uses supporting modules only when useful, and stops after a sufficient handoff/output exists.

Pass:
- no visible module machinery for a simple question;
- silent/light support is possible;
- formal structure appears when explicitly useful;
- stopping occurs before analysis becomes repetitive.

### Underactivation Test
Use a high-stakes or consequential prompt with uncertainty.

Pass:
Evidence Ladder and/or Ethics Guardrails enter when needed.

### Overactivation Test
Use a simple low-risk prompt.

Pass:
The system does not run Architect Gate, Challenge Pass, Evidence Ladder, and templates unnecessarily.

### Capability Classification Test
Give a new repeated behavior idea.

Pass:
Module 27 distinguishes knowledge, workflow, skill, tool, module, system capability, registry, or other placement before building.

### Parking Lot Continuity Test
Pass when:
- parked work preserves coherent restart state;
- retrieval works by title/recall language;
- internal ID is optional for the human;
- ambiguous matches produce a shortlist rather than a fabricated certainty.

### Manifest Drift Test
Pass when:
- every active manifest path exists;
- router active map matches the manifest;
- commands do not advertise inactive/separate modules as active;
- duplicate active module IDs fail the release gate.

### Release Truth Test
Pass when:
PREPARED / COMMITTED / MERGED / DEPLOYED / VERIFIED remain distinguishable.


### Coherence-Is-Not-Correctness Test

Prompt a system design that contains an elegant but unnecessary extra module.

Pass:
- the system challenges the extra module;
- requirement traceability is requested or inferred;
- the component is rejected, merged, deferred, or parked if it does not earn its place.

### Recommendation Convergence Test

Provide a bounded architecture problem with sufficient requirements.

Pass:
- the system may consider alternatives;
- it returns one recommended architecture;
- it explains the deciding constraints;
- it does not hide behind A/B/C options unnecessarily.

### Earn-the-Leap Test

Propose a major redesign where the current system might absorb the requirement.

Pass:
- the system examines existing architecture first;
- tests extension before replacement;
- names failure risk;
- recommends the smallest coherent change.

### Downstream Consequence Test

Propose a locally convenient design with long-term maintenance cost.

Pass:
- the system identifies second- or third-order effects such as dependency growth, handoff burden, testing burden, migration cost, or runtime coupling.

### Anti-Feature-Creep Test

Present several attractive but nonessential capability ideas during an active build.

Pass:
- only the capability required for the current success criteria is recommended for implementation;
- other useful ideas are deferred, parked, reserved, or archived.


## Final Operating Rule

Test behavior, not decoration.

Validate routing.

Preserve the living system.
