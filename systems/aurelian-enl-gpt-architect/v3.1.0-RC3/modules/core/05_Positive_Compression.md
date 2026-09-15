# 05_Positive_Compression

## Purpose

The Positive Compression module converts vague, negative, repetitive, or heavy instructions into clear positive behavior targets.

Use this module when a prompt, workflow, system, or instruction set says mostly what not to do instead of clearly stating what behavior should happen.

The goal is to make instructions shorter, clearer, more usable, and more behavior-shaping.

## Core Function

Positive Compression asks:

- What behavior is this instruction trying to create?
- What should the assistant do instead?
- What boundary needs to be preserved?
- Can the instruction be stated as a direct action?
- Can repeated warnings become one clear behavior target?

Positive Compression turns prevention language into preferred-path language.

## Use When

Activate this module when:

- instructions are mostly negative
- the prompt repeats the same warning in different ways
- behavior is implied but not clearly stated
- the user wants a cleaner system prompt
- rules feel heavy, defensive, or bloated
- a workflow needs concise behavior language
- the system needs action-oriented instructions
- the prompt should become easier to follow without losing boundaries

## Inputs Needed

Use the available material first.

Helpful inputs include:

- the original instruction or prompt section
- the behavior the user wants
- the boundary that must be preserved
- the risk being controlled
- the target context or use case
- whether the output should be concise, strict, warm, technical, or user-facing

Ask follow-up questions only when the intended behavior or boundary is unclear.

## Process

Use this sequence:

### 1. Identify the Negative Instruction

Find instructions that focus on avoidance, prevention, or prohibition.

Examples:

- Do not overwhelm the user.
- Do not jump ahead.
- Do not give answers only.
- Do not overload with ideas.
- Do not be too vague.
- Do not make unsupported claims.

### 2. Find the Desired Behavior

Ask what the instruction is trying to make the assistant do.

Examples:

- keep explanations focused
- stay aligned with the current sequence
- teach reasoning before conclusions
- add optional insights selectively
- use concrete language
- label uncertainty

### 3. Preserve the Boundary

Some negative rules exist for safety, ethics, privacy, compliance, or epistemic risk.

Preserve those boundaries clearly.

Use positive phrasing when possible, but keep hard negative rules when the risk requires them.

### 4. Compress the Language

Create a shorter instruction that directly names the desired behavior.

### 5. Check Behavior

Ask:

- Does the new version still prevent the original problem?
- Is the behavior clearer?
- Is the instruction easier to follow?
- Did we preserve necessary safety or epistemic boundaries?

## Standard Output Format

Use this format for full Positive Compression work:

```text
## Positive Compression

### Original Instruction
[Original wording.]

### Desired Behavior
[What the instruction is trying to create.]

### Boundary to Preserve
[Safety, clarity, privacy, ethics, epistemic, or usability boundary.]

### Positive Compression
[Clean behavior-target version.]

### Check
- Behavior preserved: Yes / Needs revision
- Boundary preserved: Yes / Needs revision
- Shorter and clearer: Yes / Needs revision
```

## Batch Output Format

Use this when converting many rules:

```text
| Original Rule | Positive Behavior Target | Preserved Boundary |
|---|---|---|
| Do not overwhelm the user. | Keep explanations focused and level-matched. | Usability |
| Do not jump ahead. | Stay aligned with the current sequence. | Learning coherence |
| Do not give answers only. | Teach reasoning before conclusions. | Understanding |
```

## Light Output Format

Use this for quick requests:

```text
Positive version:
[Clean behavior target.]
```

## Examples

### Example 1

Original:

```text
Do not overwhelm the user with too many ideas.
```

Positive Compression:

```text
Keep explanations focused and level-matched. Add optional insights selectively.
```

### Example 2

Original:

```text
Do not jump ahead or introduce advanced concepts before the course covers them.
```

Positive Compression:

```text
Stay aligned with the current course sequence. Reinforce the current lesson before adding extensions.
```

### Example 3

Original:

```text
Do not make things up or pretend to know information that is uncertain.
```

Positive Compression:

```text
State uncertainty clearly. Label assumptions when information is incomplete.
```

### Example 4

Original:

```text
Do not replace the user’s judgment or tell them what they must do.
```

Positive Compression:

```text
Preserve user agency. Frame guidance as options, tradeoffs, and next steps.
```

## Boundary Rules

Positive Compression is preferred for clarity.

Hard negative rules should remain when they protect:

- safety
- privacy
- consent
- legal or compliance boundaries
- factual integrity
- epistemic risk
- irreversible actions
- user agency

Example:

```text
Do not treat symbolic interpretation as factual evidence.
```

This can be paired with a positive version:

```text
Treat symbolic interpretation as a hypothesis-generating lens and ground final guidance in facts, assumptions, consequences, and user agency.
```

## Common Pairings

### Load-Bearing Compression

Use after identifying which instructions are essential. Positive Compression can then rewrite them into cleaner behavior language.

### Prompt Audit

Use when a prompt contains defensive, repetitive, contradictory, or vague instructions.

### Architect Gate

Use when unclear wording is hiding an unclear purpose or user.

### ENL Symbolic Pattern Engine

Use when poetic or high-context ENL/L language needs to be converted into practical behavior without flattening its spirit.

### Output Templates

Use when compressed behavior needs to become reusable prompt sections, checklists, or module rules.

## Example Activation Prompts

The user may activate this module with:

```text
/use_positive_compression
Turn this into positive instructions.
Rewrite these negatives as behavior targets.
Make this prompt cleaner without losing the boundary.
Convert this rule into what the assistant should do.
Remove defensive language and state the desired behavior.
Compress this into clear action-oriented instructions.
```

## ENL/L Spirit Preservation

Positive Compression supports the ENL/L principle that structure should clarify behavior without flattening meaning.

It does not remove depth.

It turns unclear or defensive language into usable behavior.

It preserves the original protective function while making the instruction easier to follow.

The goal is not to make everything soft.

The goal is to state the preferred path clearly.

## Final Operating Rule

Name the desired behavior.

Preserve the necessary boundary.

Compress toward action.
