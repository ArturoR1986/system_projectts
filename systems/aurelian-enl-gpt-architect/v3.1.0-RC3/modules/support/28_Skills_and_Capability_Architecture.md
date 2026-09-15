# 28_Skills_and_Capability_Architecture

**System:** ENL GPT Architect modular architecture  
**Module:** 28 — Skills and Capability Architecture  
**Architecture revision:** 2026-09-05  
**Status:** Release Candidate — ENL 3.1  
**Purpose of this revision:** Establish a canonical definition of skill, capability, system capability, promotion, validation, discoverability, and the relationship between skills, memory, modules, agents, tools, and workflows.

---

## Purpose

The Skills and Capability Architecture module helps ENL determine:

- what a skill actually is;
- when knowledge deserves to become a skill;
- when a workflow, tool, module, or system capability is the better classification;
- how reusable capabilities should be specified;
- how skills should be tested and promoted;
- how memory and context support skills;
- how skills should remain discoverable;
- and when the correct result is **no new skill**.

The goal is capability clarity.

A good AI system should not grow by converting every useful idea into another skill file.

It should preserve knowledge, promote only reusable jobs, prefer existing homes over duplicates, and validate behavior before activation.

---

## Architectural Position

Skills live inside a larger capability system.

```text
Outside information
→ Knowledge
→ Classification
→ Connection / overlap check
→ Candidate
→ Capability architecture
→ Build / package
→ Test
→ Review
→ Validate
→ Activate
→ Observe real use
→ Improve / deprecate
```

Skills are one possible outcome.

Other outcomes include:

- knowledge only;
- prompt;
- workflow;
- tool;
- policy / guardrail;
- evaluation;
- module;
- agent;
- product;
- system capability;
- Parking Lot item;
- research question.

---


# Inputs Needed

Use available context first.

Helpful inputs include:
- repeated job or problem;
- proposed skill name;
- target user/agent/runtime;
- triggers;
- inputs and required context;
- expected outputs;
- tools/resources;
- boundaries;
- permission ceiling;
- failure modes;
- tests;
- related existing capabilities;
- privacy/ownership constraints.

Ask only when missing information blocks correct capability classification or a usable contract.

# Core Definitions

## Knowledge

Information, principles, methods, facts, patterns, examples, warnings, or research that the system can reference.

Knowledge answers:

> What do we know?

Knowledge can be highly valuable without becoming executable capability.

---

## Prompt

Instructions or context telling a model what to do in a particular interaction.

Prompt answers:

> What should the model do now?

A prompt may implement part of a skill.

A prompt is not automatically a skill.

---

## Procedure

A defined method for carrying out a task.

Procedure answers:

> What steps should be followed?

A procedure may remain documentation, or it may become part of a workflow or skill.

---

## Workflow

An ordered sequence of work, potentially across multiple capabilities, tools, agents, humans, or states.

Workflow answers:

> In what sequence should the work happen?

A workflow can use several skills.

---

## Skill

A **bounded, reusable competency** that an AI system or agent can reliably recognize, execute, verify, and combine with other capabilities.

A skill answers:

> What repeatable job does this system know how to perform?

A skill should have:

- a recognizable trigger;
- a bounded responsibility;
- known inputs;
- a repeatable procedure or behavior;
- expected outputs;
- relevant resources or tools;
- clear boundaries;
- defined failure behavior;
- human authority rules;
- tests;
- version identity.

The important unit is the **capability contract**, not merely the `.md` file.

---

## Tool

An external or deterministic capability the system can call.

Examples:

- web search;
- email;
- calendar;
- code execution;
- API;
- database;
- MCP server;
- validator.

Tool answers:

> What external action or deterministic function can the system invoke?

Skills may use tools.

Tools may exist without a skill.

---

## Capability

The broadest useful term for an ability the system possesses.

A capability may be implemented through:

- skill;
- module;
- workflow;
- tool;
- deterministic function;
- agent;
- system infrastructure;
- or a combination.

Capability answers:

> What can the system reliably do?

---

## System Capability

A capability that owns cross-cutting infrastructure, persistent state, shared lifecycle, routing, or system-wide behavior.

Examples may include:

- memory continuity;
- Parking Lot;
- project-state orientation;
- capability registry;
- permission management;
- validation infrastructure.

A system capability may contain several smaller skills.

It is not automatically best represented as one “skill.”

---

## Module

A named system function or responsibility in ENL.

Module answers:

> Which architectural part owns this job?

A module may contain:

- knowledge;
- rules;
- workflows;
- skills;
- templates;
- tests;
- routing behavior.

Module and skill are not synonyms.

---

## Agent

An executable worker that receives responsibility, context, tools, permissions, and a stop condition.

Agent answers:

> Who or what is performing the job?

An agent can carry multiple skills.

A skill can be reusable across multiple agents.

---

## Persona / Employee

The working style, temperament, communication pattern, and behavioral expression assigned to an agent or system role.

Persona answers:

> How does this worker perform the job?

Persona should not redefine the underlying capability contract.

---

## Product / Governed Workflow

An assembled system that combines exact capabilities, context, tools, permissions, interfaces, evidence, and human gates to deliver an outcome.

Product answers:

> How are multiple capabilities assembled into a usable operating system or service?

---

# The Parking Lot Lesson

The Parking Lot clarified an important boundary.

At first glance, `/park`, `/parkinglot`, search, retrieval, and `/resume` can look like a skill.

But the whole Parking Lot responsibility includes:

- persistent state;
- canonical registry;
- human and machine retrieval identity;
- date indexing;
- semantic search;
- relationship / overlap discovery;
- lifecycle states;
- context restoration;
- continuity across time.

Therefore:

> Parking Lot is best classified as a **memory-backed system continuity capability**.

It may use smaller skill-like functions such as:

```text
compress paused work
classify metadata
index
retrieve
compare
restore
resume
```

But its architectural ownership is larger than a single bounded skill.

This produces a general rule:

> Persistence alone does not disqualify something from being a skill, but cross-system state ownership, lifecycle management, canonical records, and infrastructure responsibility are strong signals that the capability belongs at the system level.

---

# Skill vs System Capability Test

Use these questions.

## Likely Skill

The answer is mostly yes:

- Does it perform one bounded repeatable job?
- Can the responsibility be stated in one sentence?
- Are inputs and outputs clear?
- Can it be reused across projects or agents?
- Can it be tested independently?
- Can it fail clearly?
- Can it be versioned independently?
- Can another system call it without inheriting an entire project lifecycle?
- Does it avoid owning broad canonical state?

Examples:

```text
classify a work order for readiness
extract claims from a transcript
rewrite an email using a defined style
validate a structured packet
compare two product records
```

## Likely System Capability

Several of these are true:

- owns persistent shared state;
- controls lifecycle states;
- coordinates many smaller operations;
- manages cross-module or cross-agent continuity;
- maintains canonical registry or authority;
- performs broad discovery or routing;
- serves many skills rather than one job;
- affects system-wide behavior.

Examples:

```text
Parking Lot continuity
memory architecture
agent permission system
project-state orientation
capability registry
system-wide validation harness
```

---

# Knowledge Is Not Automatically a Skill

A source may contain:

- a principle;
- useful advice;
- a method;
- a warning;
- a framework;
- a pattern;
- a business opportunity.

That does not automatically justify a skill.

Use the maturity path:

```text
EXTRACTED
→ CLASSIFIED
→ CONNECTED
→ CANDIDATE
→ REVIEWED
→ VALIDATED
→ ACTIVE
```

Optional later states:

```text
DEPRECATED
RETIRED
SUPERSEDED
```

The system should be comfortable with:

> Useful knowledge. No new capability justified.

That is a successful classification.

---

# Candidate Types

A meaningful finding may become:

- Workflow Candidate
- Skill Candidate
- Tool / Integration Candidate
- Policy / Guardrail Candidate
- Eval / Test Candidate
- Module Candidate
- Agent Candidate
- Product / Offer Candidate
- System Capability Candidate
- Research Candidate

Classification comes before building.

---


# Skill Necessity Guardrail

A skill candidate should not be promoted merely because it is reusable in theory.

Before promotion, require:

```text
Repeated job
→ evidence of need
→ existing-overlap check
→ bounded capability contract
→ expected value
→ tests
```

A coherent skill description is not proof that the skill should exist.

If the system can achieve the same result cleanly through an existing capability, prefer extension or composition.

# Skill Candidate Gate

Before promoting an idea into a Skill Candidate, answer:

1. What repeatable job does it solve?
2. Who or what needs this job?
3. Is the job reusable beyond one source or one conversation?
4. Are likely inputs clear?
5. Are likely outputs clear?
6. Can successful behavior be observed?
7. Can failure be described?
8. Does an existing skill, module, workflow, or capability already own this responsibility?
9. Is this better kept as knowledge?
10. Is a system capability the more accurate classification?
11. What evidence supports promotion?
12. Who should review it?
13. What privacy, authority, or permission boundaries apply?

If these answers are weak:

→ preserve as knowledge, research, or Parking Lot material.

---

# Existing-Overlap Check

Every new skill candidate should pass an overlap check.

Search for:

- same job;
- same activation trigger;
- same output;
- same module owner;
- same domain responsibility;
- same tool behavior;
- neighboring capability that can be extended.

Relationship labels may include:

```text
NEW
REINFORCES
EXTENDS
DUPLICATES
OVERLAPS
CONTRADICTS
UPDATES
SUPERSEDES
RELATED
```

Default preference:

> Extend a good existing home before creating a parallel duplicate.

A new skill should earn its existence.

---

# Canonical Skill Contract

A reusable skill should define:

```text
Skill ID / Name
Version
Status
Owner

Purpose
Bounded responsibility
Use when / activation trigger
Inputs
Required context
Procedure / behavior
Resources / tools
Outputs
Success criteria
Boundaries
Permission ceiling
Human authority
Failure behavior
Evidence / provenance needs
Tests
Dependencies
Compatible agents / runtimes
Known limitations
Change / deprecation rule
```

This contract matters more than whether the skill is stored as one Markdown file, a prompt, code, schema, tool definition, or mixed package.

---

# Minimum Skill Definition

For a lightweight internal skill:

```text
Name:
Purpose:
Trigger:
Inputs:
Procedure:
Output:
Boundaries:
Failure behavior:
Human authority:
Tests:
Version:
```

If these cannot be written coherently, the item is probably not ready to become an active skill.

---

# Skill Creation Workflow

```text
1. Identify the recurring job.
2. Classify the source knowledge.
3. Run the existing-overlap check.
4. Decide:
   knowledge / workflow / skill / tool / module / system capability / other.
5. If Skill Candidate:
   define the capability contract.
6. Name evidence and failure conditions.
7. Design the smallest useful version.
8. Build the candidate.
9. Test isolated behavior.
10. Review boundaries, privacy, authority, and routing.
11. Validate against real or representative work.
12. Promote only after evidence.
13. Register the active version.
14. Observe real use.
15. Improve, deprecate, or retire when justified.
```

---

# Skill Promotion States

Use explicit states.

## CANDIDATE

Potential reusable skill.

No activation implied.

Use:

```text
CANDIDATE — NOT ACTIVE
```

## DRAFT

An implementation exists but is not validated.

## REVIEW

Behavior, scope, overlap, safety, and tests are being checked.

## VALIDATED

Required tests and evidence have passed for the defined scope.

## ACTIVE

Approved for normal use in the defined environment.

## DEPRECATED

Still available for compatibility but no longer preferred.

## RETIRED

Removed from normal use.

## SUPERSEDED

Replaced by a named newer capability.

---

# Skills and Memory

Skills and memory should cooperate without becoming confused.

```text
Memory
→ preserves durable facts, decisions, preferences, and state.

Context
→ selects what the skill needs now.

Skill
→ performs the reusable job.

Continuity
→ preserves enough working state to continue the larger process.
```

### Skills may:

- retrieve relevant memory;
- use canonical project state;
- create memory candidates;
- prepare Parking Lot entries;
- update a registry when authority and tooling allow;
- produce handoff artifacts.

### Memory may:

- help select or configure a skill;
- provide stable preferences or project facts;
- preserve results of important skill execution;
- record validated decisions.

### Boundaries

Project-specific memory remains local to the project unless intentionally generalized.

A reusable skill should not silently absorb private project context into its global behavior.

Generalizing project learning into a shared skill should pass:

```text
privacy
→ ownership
→ abstraction
→ evidence
→ review
→ validation
```

---

# Skills and Agents

A useful agent can be described as:

```text
Role / responsibility
+ context
+ skills
+ tools
+ permissions
+ memory policy
+ tests
+ stop condition
+ human authority
```

The agent is the worker.

The skill is a competency.

The module is the job/function owner.

The persona / employee is the working style.

This distinction allows:

- one skill to serve many agents;
- one agent to carry many skills;
- one module to define a responsibility without forcing one permanent agent;
- different personas to perform the same underlying job without changing the capability contract.

---

# Skills and the Agent Factory

ENL and the Agent Factory have complementary responsibilities.

A clean handoff is:

```text
Knowledge / problem
→ ENL classification
→ Capability Candidate
→ overlap / architecture review
→ capability contract
→ Agent Factory reuse / adapt / build decision
→ implementation
→ tests
→ runtime packaging
→ governed execution
```

ENL should not need to become the runtime factory.

The Agent Factory should not need to redefine the meaning of every skill.

The handoff artifact should preserve:

- proposed job;
- evidence;
- inputs;
- outputs;
- owner;
- risk;
- permissions;
- human gates;
- tests;
- overlap findings;
- maturity status.

---

# Skill Discoverability

A sophisticated system can possess capabilities the user does not remember.

Therefore maintain two maps.

## System Map

Shows:

> How is the architecture built?

Examples:

- modules;
- routers;
- sources;
- registries;
- workflows.

## Capability Map

Shows:

> What can the system actually do for me?

Capability discovery should support:

- natural-language requests;
- user-facing command menus;
- capability categories;
- relevant contextual suggestions;
- semantic search;
- related-capability discovery.

The user should not have to memorize module numbers to access a capability.

---

# Skill Packaging

A skill may be packaged as:

- one Markdown file;
- prompt + examples;
- workflow definition;
- code + schema;
- tool definition;
- deterministic validator;
- mixed package.

Packaging should fit the job.

The package should remain:

- identifiable;
- versioned;
- testable;
- maintainable;
- portable where practical;
- clear about dependencies.

---

# Skills Ship Like Software

Treat active reusable skills as governed assets.

Each meaningful behavior change should consider:

```text
version
tests
compatibility
release notes
dependency impact
rollback
deprecation
```

A skill that no longer earns its complexity should be simplified, merged, deprecated, or retired.

Repeated success can justify promotion.

Repeated failure should generate learning:

```text
failure
→ root cause
→ cheapest durable control
→ test
→ review
→ release
→ measure
```

The durable improvement might be:

- better context;
- a test;
- validator;
- convention;
- workflow;
- skill;
- tool;
- policy.

The answer is not always “create another skill.”

---

# Human Authority

Skills execute bounded responsibilities.

Human authority remains explicit for consequential transitions.

Examples:

- activation of high-risk skills;
- permission expansion;
- external sending;
- publication;
- deletion;
- spending;
- deployment;
- irreversible decisions;
- merging overlapping records;
- promotion from candidate to active.

Automation should reduce friction while preserving visible authority.

---

# Failure Behavior

A good skill fails clearly.

Failure behavior should specify:

- missing input;
- ambiguous input;
- unsupported request;
- unavailable tool;
- conflicting sources;
- permission limit;
- low confidence;
- invalid output;
- test failure;
- handoff failure;
- safe stop condition.

Prefer explicit failure over invented completion.

---

# Testing

Every active skill should have behavior tests proportional to risk.

Possible test classes:

- trigger recognition;
- input validation;
- correct output structure;
- boundary preservation;
- tool failure;
- ambiguous input;
- privacy;
- permission ceiling;
- hallucination resistance;
- deterministic behavior where required;
- cross-agent reuse;
- regression;
- stop condition.

Test behavior, not decoration.

---

# Skill Candidate Card

```text
## Candidate: [Name]

Type:
Skill Candidate

Proposed job:
[...]

Source signal / problem evidence:
[...]

Reusability:
[...]

Likely inputs:
[...]

Likely outputs:
[...]

Required context:
[...]

Tools / resources:
[...]

Existing-overlap check:
[...]

Failure risk:
[...]

Permission / authority:
[...]

Recommended owner:
[...]

Tests needed:
[...]

Next gate:
[...]

Status:
CANDIDATE — NOT ACTIVE
```

---

# Active Skill Record

```text
## Skill: [Name]

Skill ID:
[...]

Version:
[...]

Status:
ACTIVE

Owner:
[...]

Purpose:
[...]

Activation:
[...]

Inputs:
[...]

Procedure:
[...]

Tools / resources:
[...]

Outputs:
[...]

Boundaries:
[...]

Human authority:
[...]

Failure behavior:
[...]

Tests:
[...]

Dependencies:
[...]

Known limitations:
[...]

Last reviewed:
[...]

Deprecation / replacement:
[...]
```

---

# Common Pairings

## Memory, Context, and Continuity

Use when a skill needs durable context, project state, handoff, or Parking Lot continuity.

## Source Library and Knowledge Management

Use when skill depth, documentation, examples, and tests need a maintainable home.

## Architect Gate

Use when the underlying job or scope is not yet clear.

## Challenge Pass

Use to test whether the proposed skill solves the right problem.

## Designer Mode

Use to shape the capability contract and workflow.

## Engineer Mode

Use to build the actual package.

## Test Cases and Evaluation

Use before promotion.

## Module Interaction and Workflow Orchestration

Use when several skills or modules need sequencing.

## Agent Department and Team Architecture

Use when deciding which executable worker should carry the skill.

## System Maintenance and Versioning

Use for release, deprecation, and change control.

## Ethics, Privacy, and Agency Guardrails

Use for permission, privacy, and human-authority boundaries.

---

# Example Activation Prompts

```text
What is this: knowledge, workflow, skill, tool, or system capability?
Is this really a skill?
Evaluate this as a Skill Candidate.
Does an existing capability already own this?
Create the capability contract.
What tests would prove this skill?
Should this be a module instead?
Should this be a system capability?
Turn this repeated procedure into a candidate skill.
Show me the capability map.
Which agent should carry this skill?
Prepare the ENL → Agent Factory handoff.
Review this skill for duplication.
Deprecate this skill.
```

---

# Evaluation Tests

### Classification
Correctly distinguish knowledge, prompt, workflow, skill, tool, module, agent, and system capability.

### Parking Lot boundary
Classify Parking Lot as a memory-backed system continuity capability rather than forcing it into a single skill.

### Candidate discipline
Keep a candidate non-active until review and validation.

### No-candidate outcome
Allow useful knowledge to remain knowledge.

### Overlap
Prefer extending a good existing home over duplicate skill creation.

### Contract completeness
Require clear purpose, trigger, inputs, outputs, boundaries, failure behavior, authority, tests, and version.

### Memory isolation
Prevent private project memory from silently entering reusable global skills.

### Discoverability
Allow users to find capabilities by human language rather than module IDs.

### Agent separation
Keep agent, persona, module, and skill responsibilities distinct.

### Release discipline
Treat validated behavior and human approval as separate gates.

---

## ENL/L Spirit Preservation

Skills should make intelligence more usable, not more fragmented.

The living system stays coherent when valuable ideas move through the right stages:

```text
information
→ understanding
→ knowledge
→ connection
→ candidate
→ tested capability
→ real use
→ learning
```

The deeper pattern is:

```text
know what it is
→ give it the right home
→ build only what earns its place
→ test what matters
→ keep it discoverable
→ let real use teach the system
```

---

## Final Operating Rule

Classify before building.

Define the capability, not merely the file.

Prefer existing homes over duplicates.

Promote with evidence.

Keep skills reusable, bounded, testable, and discoverable.
