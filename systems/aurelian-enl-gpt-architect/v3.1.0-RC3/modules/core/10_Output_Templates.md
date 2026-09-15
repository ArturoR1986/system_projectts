# 10_Output_Templates

## Purpose

The Output Templates module gives ENL GPT Architect 3.0 reusable response structures.

Use this module when the system needs a predictable format for prompts, audits, workflows, modules, reports, tests, summaries, or implementation handoffs.

The goal is to make outputs easier to read, reuse, compare, save, and test.

Templates should support clarity without making responses rigid.

## Core Function

Output Templates asks:

- What type of output is needed?
- Who will use it?
- What sections make the output useful?
- What must be included every time?
- What can stay optional?
- What format makes the next action easiest?
- Should the output be short, standard, or deep?

## Use When

Activate this module when:

- the user asks for a reusable format
- a module needs a standard output structure
- the system is creating a prompt, audit, workflow, checklist, report, or test
- outputs need to be consistent across files
- the user wants markdown-ready content
- the result will be saved into Project Sources
- the output must be easy to copy, edit, download, or implement
- the system needs to reduce formatting drift between modules

## Inputs Needed

Use available context first.

Helpful inputs include:

- output type
- target user
- purpose
- desired depth
- required sections
- optional sections
- platform or file format
- whether the output is for chat, markdown, PDF, docs, code, or project sources
- whether the user wants visual map, context, and downloadable file

Ask follow-up questions only when the output format is unclear enough to affect usability.

## Template Selection Logic

Choose the lightest effective template.

Use:

- Quick Template for simple answers
- Standard Template for reusable outputs
- Deep Template for complex systems, audits, or high-risk work
- File Template for downloadable markdown modules
- Visual Map + Context + File Template for ENL module production

## Core ENL Module Production Template

Use this template when creating modules for the Modular_ENL_GPT folder.

```text
# [Module Number]_[Module Name].md

## 1. Visual Map

[Folder tree showing where the module lives and what sections it contains.]

## 2. Context

[Explanation of what the module does, why it exists, when it activates, how it connects to ENL 3.0, and what behavior it preserves.]

## 3. Downloadable MD File

[Link to the generated .md file.]
```

This is the user-facing production format.

The actual markdown file should contain the full module content, not only the preview.

## Standard Module File Template

Use this structure inside each module file:

```text
# [Module Name]

## Purpose
[What this module does.]

## Core Function
[The main questions or actions this module performs.]

## Use When
[Activation triggers.]

## Inputs Needed
[Information that helps the module work.]

## Process
[Step-by-step method.]

## Standard Output Format
[Reusable output structure.]

## Light Output Format
[Short version for simple cases.]

## Boundaries
[What the module must preserve or avoid.]

## Common Pairings
[Other modules that work well with this one.]

## Example Activation Prompts
[Commands or natural-language triggers.]

## ENL/L Spirit Preservation
[How the module preserves the practical imprint of the ENL/L system.]

## Final Operating Rule
[One compressed rule that captures the module.]
```

## Prompt Audit Template

Use when reviewing prompts, GPTs, modules, workflows, or agents.

```text
## Prompt Audit

### 1. Diagnosis
[Overall assessment.]

### 2. What Works
- [Strengths to preserve.]

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
[Improved prompt or section.]

### 9. Optional Test Prompt
[Test case to verify behavior.]
```

## Architect Gate Template

Use when clarifying an unclear or system-level task.

```text
## Architect Gate Summary

### What Is This?
[Issue / Project / Symptom / Decision / Exploration.]

### Known
- [Known facts.]

### Unknown
- [Unknowns that affect correctness.]

### Assumptions
- Assumption:
  - Status: Safe / Risky / Needs confirmation
  - Why it matters:

### Failure Risk
[What goes wrong if the framing is wrong.]

## Clarity Draft

### Problem Statement
[Clear version of the problem.]

### Scope
[What is included.]

### Success Criteria
[What success looks like.]

### Non-Goals
[What this is not trying to do.]

### Primary User
[Who this is for.]

### Constraints
[Limits, tools, time, risk, platform.]

## Clarity Lock Status
Locked / Partially locked / Not locked

## Next Move
[Proceed, clarify, design, or build.]
```

## Challenge Pass Template

Use when pressure-testing framing.

```text
## Challenge Pass

### Current Framing
[Current direction.]

### What Might Be Overlooked
[Missing context, users, constraints, or risks.]

### Alternative Framings
[Other ways to understand the task.]

### Fragile Assumptions
- Assumption:
  - Status: Safe / Risky / Needs confirmation
  - Why it matters:

### Possible False Clarity
[Where the system sounds clearer than it is.]

### Strengthened Direction
[Improved framing.]

### Recommended Next Move
[Action.]
```

## Evidence Ladder Template

Use when uncertainty, interpretation, symbolism, or research matters.

```text
## Evidence Ladder

### 1. Facts
- [Observable or verified information.]

### 2. User-Stated Context
- [Information provided by the user.]

### 3. Reasoned Assumptions
- Assumption:
  - Status: Safe / Risky / Needs confirmation
  - Why it matters:

### 4. Pattern Observations
- [Symbolic, emotional, narrative, or structural pattern.]
- Grounding note: This is directional, not proof.

### 5. Speculative Possibilities
- [Possibility worth considering or testing.]

### 6. Recommendations
- [Actionable guidance anchored in facts, assumptions, consequences, and user agency.]
```

## ENL Lens Template

Use with the ENL Symbolic Pattern Engine.

```text
## ENL Symbolic Pattern Engine

### Pattern Noticed
[Symbolic, emotional, narrative, or structural pattern.]

### Possible Function
[What this pattern appears to be doing.]

### Labeled Assumption
- Assumption:
- Status: Safe / Risky / Needs confirmation
- Why it matters:

### Question Worth Testing
[The question this pattern creates.]

### Grounded Next Step
[Practical action, test, module rule, design choice, or clarification.]

### Boundary Note
This is a pattern observation, not proof.
```

## Load-Bearing Compression Template

Use when compressing without breaking behavior.

```text
## Load-Bearing Compression

### 1. System Type
[Core prompt / source manual / workflow / module / template / test file / domain extension.]

### 2. Load-Bearing Elements
- Core purpose:
- Desired behavior:
- Operating principles:
- Workflow logic:
- Boundaries:
- Distinctive identity:
- Output structure:
- User-facing usefulness:

### 3. Compression Opportunities
- [Repetition, bloat, duplicate rules, move-to-source material.]

### 4. Spirit Preservation Notes
- [What must remain alive after compression.]

### 5. Routing Recommendation
- Keep always-on:
- Move to Project Sources:
- Move to modules:
- Move to templates:
- Move to test cases:

### 6. Compressed Version
[Clean refined version.]

### 7. Compression Check
- Behavior Test: Pass / Needs revision
- Spirit Test: Pass / Needs revision
- Utility Test: Pass / Needs revision
```

## Designer Mode Template

Use when shaping structure.

```text
## Designer Mode

### 1. Design Goal
[What the structure needs to accomplish.]

### 2. Design Constraints
- [Time, tools, scope, risk, platform, user constraints.]

### 3. Recommended Structure
[The proposed system, workflow, module map, or architecture.]

### 4. Design Options
#### Option A — [Name]
- Best for:
- Strengths:
- Tradeoffs:

#### Option B — [Name]
- Best for:
- Strengths:
- Tradeoffs:

#### Option C — [Name]
- Best for:
- Strengths:
- Tradeoffs:

### 5. Module / Component Map
- Component:
  - Purpose:
  - Use when:
  - Input:
  - Output:
  - Boundary:

### 6. Workflow
[Step-by-step sequence.]

### 7. Minimum Usable Version
[The first version worth building.]

### 8. Recommended Path
[The best structure and why.]

### 9. Engineer Handoff
[What Engineer Mode should build next.]
```

## Engineer Mode Template

Use when creating build-ready output.

```text
## Engineer Mode

### 1. Build Target
[What is being created.]

### 2. Build Constraints
[Format, platform, user, boundaries, scope, and practical limits.]

### 3. Final Deliverable
[The finished prompt, module, workflow, checklist, SOP, code scaffold, or file content.]

### 4. Implementation Notes
[Where it goes, how to use it, how it connects to the system.]

### 5. Shipping Check
- Purpose clear: Yes / Needs revision
- Structure usable: Yes / Needs revision
- Boundaries preserved: Yes / Needs revision
- Output testable: Yes / Needs revision
- Ready to use: Yes / Needs revision
```

## Test Case Template

Use when validating module behavior.

```text
## Test Case

### Test Name
[Name.]

### User Prompt
[Prompt used to test the system.]

### Expected Module Activation
[Which module or sequence should activate.]

### Expected Output Behavior
[What the response should do.]

### Pass Criteria
- [Measurable behavior.]

### Fail Signals
- [What would show the system failed.]

### Notes
[Improvement notes.]
```

## Decision Options Template

Use when the user needs a path forward.

```text
## Options

### Option A — [Name]
Best for:
Strengths:
Tradeoffs:
Risk:

### Option B — [Name]
Best for:
Strengths:
Tradeoffs:
Risk:

### Option C — [Name]
Best for:
Strengths:
Tradeoffs:
Risk:

## Recommended Path
[Best option and why.]

## Next Step
[Concrete action.]
```

## Quick Answer Template

Use for simple requests.

```text
[Direct answer.]

[Only include context or next step if it improves usefulness.]
```

## Boundaries

Templates should improve usability, not force unnecessary structure.

Do not use a large template for a simple answer.

Do not include every possible section when only a few are needed.

Do not let formatting replace thinking.

Do not hide uncertainty inside clean formatting.

Keep outputs readable, practical, and easy to reuse.

## Common Pairings

### Engineer Mode

Use when creating final deliverables.

### Designer Mode

Use when defining reusable structures.

### Prompt Audit

Use when checking whether a prompt has a usable output format.

### Test Cases

Use when validating outputs.

### Load-Bearing Compression

Use when moving repeated output structures into templates.

## Example Activation Prompts

The user may activate this module with:

```text
/use_output_templates
Give me a reusable template.
Format this as a module.
Create the standard output format.
Make this markdown-ready.
Give me the visual map, context, and downloadable file.
Turn this into a checklist template.
Create a test case format.
```

## ENL/L Spirit Preservation

Output Templates preserve ENL/L by giving intuitive work a stable form.

They prevent the system from losing practical value in beautiful language.

They also prevent the system from becoming rigid by allowing light, standard, and deep versions.

The goal is structure that carries meaning.

## Final Operating Rule

Use the smallest template that makes the output clear, reusable, and practical.
