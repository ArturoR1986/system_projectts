# 27_Capability_Intake_and_Placement_Protocol
Version: v3.1.0-RC1
Status: Release Candidate

## Purpose

The Capability Intake and Placement Protocol helps ENL decide what a new idea should become before anything is built.

It replaces the narrower assumption that every reusable idea should become a new module.

Core rule:

> Classify before building.

## Core Function

Ask:

- What repeated problem or job is appearing?
- What evidence shows the need is real?
- Does an existing module/capability already own it?
- Is this knowledge, workflow, skill, tool, policy, eval, module, agent, product, system capability, registry, Parking Lot item, or archive material?
- What is the smallest correct home?
- What behavior would prove value?
- What routing, command, manifest, registry, and test changes would follow?

## Use When

Activate when:

- the user proposes a new module or skill;
- a repeated task does not fit cleanly;
- a source yields a capability candidate;
- a module is becoming too broad;
- a new command is proposed;
- a workflow may deserve packaging;
- a system capability or registry may be needed;
- an agent role or department is proposed;
- the user asks where something should live.

## Inputs Needed

Use available context first.

Helpful inputs:
- proposed job/problem;
- target user;
- repeated use case;
- current related modules/capabilities;
- desired output;
- triggers;
- constraints;
- tools;
- authority/permissions;
- evidence;
- failure modes.

## Placement Classes

### Knowledge
Reference material worth preserving.

### Workflow
Ordered sequence across responsibilities.

### Skill
Bounded reusable competency.

### Tool / Integration
External or deterministic callable capability.

### Policy / Guardrail
Constraint or decision rule.

### Eval / Test
Reusable validation behavior.

### Module
System function owner.

### Agent / Role
Executable worker or responsibility carrier.

### Product
Assembled capabilities delivering an outcome.

### System Capability
Shared infrastructure, persistent state, lifecycle, routing, registry, or cross-module behavior.

### Registry
Canonical structured system data.

### Parking Lot
Coherent paused work state.

### Archive
Historical/reference material not active by default.

## Existing-Home Check

Before creating something new, search for:
- same job;
- same trigger;
- same output;
- same owner;
- same domain;
- same tool behavior;
- neighboring capability that can be extended.

Use relationship labels:

```text
NEW
REINFORCES
EXTENDS
OVERLAPS
DUPLICATES
CONTRADICTS
UPDATES
SUPERSEDES
RELATED
```

Default preference:

> Extend a good existing home before creating a parallel one.


## Architectural Integrity Check

Before recommending `Create`, ask:

```text
What real requirement creates the need?
What existing home comes closest?
Why is extension insufficient?
What new capability or boundary is gained?
What downstream complexity is introduced?
What test would prove the new object earns its place?
```

Core guardrails:

> Architectural coherence is not evidence of architectural correctness.

> Explore broadly. Commit narrowly.

> Earn the leap.


## Decision Workflow

```text
1. Intake the idea.
2. Name the repeated job/problem.
3. Check evidence.
4. Search existing homes.
5. Classify the object.
6. Define ownership boundary.
7. Define activation trigger and output.
8. Define tests and failure behavior.
9. Identify router/command/manifest/registry impact.
10. Recommend Create / Extend / Merge / Defer / Park / Archive.
```

## Skill Candidate Route

If classification = Skill:

→ Module 28 Skills and Capability Architecture.

Do not mark ACTIVE until the capability contract, tests, review, and approval are complete.

## Module Candidate Route

If classification = Module:

A module should:
- own one clear system function;
- need a distinct activation boundary;
- produce a distinct class of artifact;
- improve coherence by existing separately.

Then update router, manifest, commands if needed, tests, and change control.

## System Capability Route

Use when responsibility owns shared state, lifecycle, or cross-module infrastructure.

Examples:
- Parking Lot continuity;
- Rhythmic Modular Activation;
- Asset Sovereignty governance.

A system capability may span modules and may contain skills.

## Standard Output Format

```text
## Capability Intake

### Proposed Need
[...]

### Evidence / Repeated Job
[...]

### Existing-Home Check
- Closest owner:
- Relationship:
- Gap:

### Classification
Knowledge / Workflow / Skill / Tool / Policy / Eval / Module / Agent / Product / System Capability / Registry / Parking Lot / Archive

### Ownership Boundary
Owns:
Does not own:

### Trigger
[...]

### Expected Output
[...]

### Failure Behavior
[...]

### Router / Command / Manifest / Registry Impact
[...]

### Tests Needed
[...]

### Recommendation
Create / Extend / Merge / Defer / Park / Archive

### Next Gate
[...]
```

## Boundaries

- Newness is not evidence of value.
- Interesting knowledge does not automatically become executable capability.
- Avoid duplicate containers.
- Preserve human authority for consequential activation and release.
- Keep private context out of reusable global capabilities unless intentionally abstracted and reviewed.

## Common Pairings

- 12 Source Library
- 13 Memory and Continuity
- 15 Orchestration
- 17 Maintenance
- 28 Skills and Capability Architecture
- 11 Test Cases
- 26 Agent Department Architecture

## Example Activation Prompts

```text
/use_capability_intake
Should this be a new module?
Is this really a skill?
Where should this live?
Does an existing capability already own this?
Evaluate this as a system capability.
Create the placement decision.
```

## ENL/L Spirit Preservation

Growth should increase coherence, not file count.

## Final Operating Rule

Give the idea the right home before giving it a new file.
