# 13_Memory_Context_and_Continuity

**System:** ENL GPT Architect modular architecture  
**Module:** 13 — Memory, Context, and Continuity  
**Architecture revision:** 2026-09-05  
**Status:** Release Candidate — ENL 3.1  
**Change:** Expanded memory architecture to distinguish durable memory, project state, handoffs, Parking Lot continuity, archive, and reconstructed context.

---

## Purpose

The Memory, Context, and Continuity module helps ENL preserve the information and working state required for coherent work across chats, projects, modules, agents, files, and long-running builds.

Its job is larger than “remembering facts.”

It determines:

- what should remain active now;
- what should become durable memory;
- what belongs in Project Sources;
- what project state must remain canonical;
- what should be handed to another worker or session;
- what important work should be deliberately parked;
- what belongs in archive;
- what can be reconstructed when canonical state is unavailable;
- and what context is needed to resume accurately without forcing the user to rebuild the story.

The goal is continuity without clutter.

The governing principle is:

> Preserve what future work needs, in the lightest correct persistence layer.

---

## Architectural Position

Memory is one layer in a larger system.

```text
Outside information
→ Knowledge / Project Sources
→ Selected working context
→ Skills / workflows / tools use that context
→ Execution produces decisions, evidence, state, and learning
→ Memory and continuity preserve what must survive
```

Memory is not the same thing as knowledge.

Memory is not the same thing as a skill.

Memory is not the same thing as a handoff.

Memory is not the same thing as an archive.

Parking Lot is not simply “more memory.”

These structures work together but own different jobs.

---

## Core Definitions

### Memory

Durable information that should remain useful beyond the immediate turn or session.

Examples:

- stable user preferences;
- durable project principles;
- important decisions;
- long-lived project facts;
- recurring operating rules.

Memory answers:

> What should remain known?

---

### Knowledge

Reference material the system may need to consult.

Examples:

- source files;
- manuals;
- transcripts;
- research;
- taxonomies;
- frameworks;
- documentation.

Knowledge answers:

> What can the system reference and reason from?

Knowledge usually belongs in Project Sources, libraries, or canonical records rather than personal memory.

---

### Context

The subset of memory, knowledge, state, instructions, and current information selected for a specific job.

Context answers:

> What does this worker need right now?

Good context is selective.

More context is not automatically better context.

---

### Project State

The current authoritative condition of a project.

Examples:

- active work order;
- current version;
- approved scope;
- decisions;
- blockers;
- validation state;
- current next action;
- authoritative files.

Project state answers:

> Where is the project actually at?

Project state should prefer canonical records over conversational recollection.

---

### Continuity

The ability to move across sessions, modules, workers, or time without losing the load-bearing thread.

Continuity answers:

> What must survive so the work can continue accurately?

Continuity can use memory, Project Sources, handoffs, project records, Parking Lot entries, and archives.

---

### Handoff

A purposeful transfer of work from one worker, module, agent, project, or session to another.

A handoff answers:

> What does the next receiver need to take over this job?

A handoff is directional.

It has a sender, receiver, purpose, scope, current state, and next responsibility.

---

### Parking Lot

A structured continuity state for valuable work that should leave the active queue without being treated as completed, abandoned, or archived.

Parking Lot answers:

> What coherent body of unfinished or deferred work should remain easy to recover later?

Parking Lot preserves a **working state**, not merely a fact.

---

### Archive

Historical material preserved for reference but no longer active.

Archive answers:

> What should remain available without influencing current state by default?

---

### Reconstructed Context

Best-effort continuity recovered from available conversation history, files, memory, or related records when the canonical continuity record is unavailable.

Reconstructed context must be labeled clearly.

Use:

```text
RECONSTRUCTED FROM CONTEXT
```

Reconstruction supports recovery.

It does not silently replace canonical truth.

---

## Core Function

Memory, Context, and Continuity asks:

- What is important here?
- Is it temporary or durable?
- Is it a fact, preference, project decision, working state, or source?
- What is the correct persistence layer?
- Is there already a canonical record?
- What must remain human-readable?
- What must remain machine-stable?
- What should be easy to retrieve months later?
- What should stay private or local?
- What does the next worker need?
- Is this work active, parked, resumed, closed, superseded, or archived?
- What can safely be compressed?
- What would be expensive to reconstruct later?

---

## Use When

Activate this module when:

- the user says “remember this”;
- the user wants continuity across sessions;
- the user wants to pause an important thread;
- the user wants to resume old work;
- the user asks where information should live;
- a project spans multiple sessions or agents;
- decisions must survive beyond the current chat;
- a handoff is needed;
- a progress or continuity summary is needed;
- the project has multiple versions, modules, or work orders;
- old and current information may conflict;
- the system must distinguish canonical state from conversational recall;
- the user wants to search parked work by date, title, or relationship;
- the system needs to preserve a restart point;
- the system needs to reduce re-explanation burden.

---

## Inputs Needed

Use available context first.

Helpful inputs include:

- project name;
- current task;
- current project state;
- decisions made;
- important discoveries;
- files created or changed;
- version and status;
- active module or capability;
- open questions;
- next step;
- user preferences;
- what should persist;
- what should remain temporary;
- privacy or sensitivity constraints;
- whether the target is memory, Project Source, project state, handoff, Parking Lot, or archive.

Ask only when the correct persistence target cannot be determined safely.

---

# Continuity Layers

## 1. Active Working Context

Information needed only for current work.

Examples:

- immediate task details;
- temporary assumptions;
- draft wording;
- short-lived comparisons;
- transient tool output;
- current reasoning scaffolding.

Lifecycle:

```text
active
→ used
→ discarded, promoted, handed off, parked, or archived
```

---

## 2. Project Source Knowledge

Information that belongs in the project’s modular knowledge base.

Examples:

- module definitions;
- source maps;
- manuals;
- templates;
- taxonomies;
- workflows;
- test cases;
- reference material;
- architecture documents.

Project Sources carry depth.

They should not become a dumping ground for every conversational detail.

---

## 3. Durable User / Operator Memory

Stable information likely to remain useful across future work.

Examples:

- durable preferences;
- recurring operating principles;
- long-term project identity;
- stable working conventions explicitly worth preserving.

Durable memory should be concise.

Store the principle, not the whole conversation.

---

## 4. Canonical Project State

Authoritative information describing where a project stands now.

Examples:

- current work order;
- active branch or version;
- approved scope;
- current status;
- accepted decisions;
- unresolved blockers;
- validation evidence;
- next safe action.

Canonical state should be distinguishable from:

```text
intent
history
scratch
archive
```

A project may contain many documents.

Only some should be treated as current truth.

---

## 5. Handoff Context

Information needed by the next receiver.

A good handoff contains:

- purpose;
- current state;
- completed work;
- unresolved work;
- key decisions;
- authoritative sources;
- constraints;
- permissions or authority;
- known risks;
- next responsibility;
- stop condition.

Handoffs should be receiver-oriented.

---

## 6. Parking Lot Continuity

Important work that should remain recoverable while inactive.

Parking is a deliberate state.

```text
ACTIVE
→ PARKED
→ RETRIEVED
→ RESUMED
→ ACTIVE
```

Other terminal or relationship states may include:

```text
CLOSED
SUPERSEDED
ARCHIVED
```

Parking preserves future usefulness while clearing present attention.

---

## 7. Archive Context

Historical information no longer active by default.

Examples:

- replaced modules;
- retired versions;
- old experiments;
- superseded plans;
- reference-only artifacts.

Archive preserves history without competing with current state.

---

# Memory Decision Rule

Classify before preserving.

```text
Useful only for the current task?
→ Active Working Context

Reusable reference material?
→ Project Source Knowledge

Durable user preference or principle?
→ Durable Memory

Current authoritative project condition?
→ Canonical Project State

Needs to transfer to another receiver?
→ Handoff

Important unfinished/deferred work that should leave the active queue?
→ Parking Lot

Historical but no longer active?
→ Archive
```

If more than one layer is needed, separate the artifacts.

Example:

```text
Durable principle
→ Memory

Detailed architecture
→ Project Source

Current implementation status
→ Canonical Project State

Paused thread
→ Parking Lot

Instructions for next agent
→ Handoff
```

---

# Parking Lot Continuity Architecture

## Purpose

Parking Lot preserves coherent unfinished work.

A parked item should contain enough structure to restart accurately without reopening the entire original conversation.

It should remain easy for a human to find even when the internal ID is forgotten.

---

## Human and Machine Identity

Every Parking Lot record has two identities.

### Human Retrieval Identity

- descriptive title;
- recall cue;
- aliases;
- tags;
- summary language.

### Machine Record Identity

- stable internal ID such as `PL-001`.

Rule:

> Human language is primary for discovery. Stable IDs protect record integrity.

The user should not need to remember `PL-001` to recover an idea.

---

## Canonical Parking Lot Entry

Use:

```text
Title:
Recall cue:
Aliases:
Tags:
Internal ID:
Status:
Parked date:
Last updated:

Why parked:
Working summary:
Key discoveries / decisions:
Open questions:
Related systems / files:
Revisit triggers:
Relationship links:
Recommended restart point:
State history:
```

Prefer useful compression over transcript-sized storage.

---

## Parking Workflow

```text
1. Identify the coherent body of work being paused.
2. Create a descriptive title recognizable later.
3. Write a recall cue:
   “What would the user probably remember this as?”
4. Preserve load-bearing discoveries and decisions.
5. Preserve unresolved questions.
6. Link relevant files, systems, or projects.
7. Define observable revisit triggers.
8. Define the recommended restart point.
9. Assign or preserve the stable internal ID.
10. Update the canonical Parking Lot registry or prepare the complete update artifact.
11. Mark the work PARKED.
12. Clear it from the active queue.
```

---

## Parking Lot Discovery

`/parkinglot info` should support three discovery modes.

### 1. Date

Sort by:

- newest parked;
- oldest parked;
- most recently updated.

### 2. Name / Title

Search:

- title;
- recall cue;
- aliases;
- tags;
- working summary;
- internal ID.

### 3. Relationship / Overlap

Compare:

- shared systems;
- shared concepts;
- shared tags;
- related files;
- overlapping open questions;
- overlapping revisit triggers;
- explicit relationship links;
- summary-level similarity.

Use relationship labels such as:

```text
STRONGLY OVERLAPS
RELATED
POSSIBLE CONNECTION
DISTINCT
SUPERSEDES
SUPERSEDED BY
```

Relationship matching supports discovery.

It does not automatically change record state.

When strong overlap appears, offer:

```text
Open one
Compare
Prepare consolidation candidate
Keep separate
```

---

## Parking Lot Retrieval

For `/parkinglot <topic-or-ID>`:

```text
1. Exact internal ID
2. Exact or near title
3. Recall cue
4. Aliases
5. Tags
6. Working summary
```

If one strong match exists:

→ restore it.

If multiple plausible matches remain:

→ show the smallest useful disambiguation list.

If no confident match exists:

→ report that clearly and preserve current state.

---

## Resume Workflow

For `/resume <topic-or-ID>`:

```text
1. Resolve the parked entry.
2. Restore the working summary.
3. Restore key decisions and open questions.
4. Surface related files/systems.
5. Name the recommended restart point.
6. Move the working state from PARKED to RESUMED.
7. Preserve the state history.
8. Return to normal task routing.
```

---

# Persistence and Truth Hierarchy

Prefer this order when continuity sources conflict:

```text
1. Current canonical project record
2. Current canonical Parking Lot registry
3. Current Project Sources / versioned architecture
4. Explicit handoff artifact
5. Durable memory
6. Active conversation context
7. Reconstructed context
```

The hierarchy may vary by project, but canonical state should remain explicit.

When using a weaker source because the stronger source is unavailable, label the limitation.

---

# Write-State Integrity

Memory and continuity artifacts should distinguish:

```text
RECOMMENDED
PREPARED
WRITTEN / SAVED
VERIFIED
```

Preparing a memory note, Parking Lot entry, handoff, or registry update does not imply that the external source was actually updated.

When the runtime cannot write to the canonical store:

> Produce the complete update artifact and label it PREPARED.

This protects truthfulness around persistence.

---

# Memory and Skills

Memory and skills serve different purposes.

```text
Memory
→ preserves what must remain known or recoverable.

Skill
→ performs a bounded reusable job.

Context
→ supplies the skill with what it needs now.

Continuity
→ preserves enough state to resume the larger work.
```

A skill may read memory.

A skill may create memory candidates.

A skill may update a registry when authority and tooling allow.

A memory system may use skill-like operations such as:

```text
classify
compress
index
retrieve
compare
resume
```

But a memory-backed continuity system is not automatically a skill.

Parking Lot is the key example.

Parking Lot is best classified as a **system continuity capability** because it owns:

- persistent state;
- human and machine retrieval identity;
- indexing;
- relationship discovery;
- lifecycle states;
- restart continuity.

It may contain smaller reusable skills, but its overall job is infrastructure.

---

# Project Continuity Workflow

For long-running work:

```text
1. Name what changed.
2. Name what was created.
3. Name the decisions.
4. Name the current canonical state.
5. Name what remains open.
6. Name the next safe action.
7. Decide what belongs in:
   - active context
   - Project Sources
   - durable memory
   - canonical project state
   - handoff
   - Parking Lot
   - archive
8. Preserve only what future work needs.
```

---

# Standard Continuity Output

```text
## Project Continuity Note

### Current Project
[Name]

### Current State
[Canonical status]

### What Changed
- [...]

### What Was Created
- [...]

### Key Decisions
- [...]

### Open Questions
- [...]

### Next Safe Action
[...]

### Continuity Placement
- Active context:
- Project Sources:
- Durable memory:
- Canonical project state:
- Handoff:
- Parking Lot:
- Archive:
```

---

# Handoff Note Format

```text
## Handoff Note

### Project
[Name]

### Receiver
[Agent / module / project / person]

### Purpose
[Why the handoff exists]

### Current State
[...]

### Completed
- [...]

### Open
- [...]

### Key Decisions
- [...]

### Authoritative Sources
- [...]

### Constraints / Authority
- [...]

### Risks / Watch Points
- [...]

### Next Responsibility
[...]

### Stop Condition
[...]

### Restart Prompt
[Optional]
```

---

# Memory Note Format

Use for a durable fact, preference, or principle:

```text
Memory note:
[Concise durable statement]
```

A memory note should remain useful without requiring the original conversation.

---

# Parking Lot Entry Format

```text
## [Descriptive Title]

Recall cue:
[...]

Aliases:
- [...]

Tags:
- [...]

Internal ID:
PL-###

Status:
PARKED

Parked date:
YYYY-MM-DD

Last updated:
YYYY-MM-DD

Why parked:
[...]

Working summary:
[...]

Key discoveries / decisions:
- [...]

Open questions:
- [...]

Related systems / files:
- [...]

Revisit triggers:
- [...]

Relationship links:
- [...]

Recommended restart point:
[...]

State history:
- [...]
```

---

# Privacy and Data Minimization

Preserve only what future work needs.

Prefer:

- role-relevant facts;
- project-relevant decisions;
- necessary continuity;
- minimum necessary personal detail.

Keep sensitive or identifying material out of broad reusable registries unless essential and appropriate.

Project-specific or client-specific memory should remain isolated from unrelated projects.

Generalization into shared knowledge or skills should pass a privacy and ownership gate.

---


# Boundaries

- Preserve only what future work needs.
- Keep canonical project state distinct from conversational recollection.
- Keep durable memory concise.
- Keep Project Source knowledge out of personal memory unless the durable abstraction itself is needed.
- Label reconstructed continuity as `RECONSTRUCTED FROM CONTEXT`.
- Keep `PREPARED` distinct from an update that was actually written, committed, merged, deployed, or verified.
- Keep project-specific/private memory isolated from reusable global skills.
- Use human-readable retrieval first and stable IDs second for Parking Lot records.
- Treat Parking Lot relationship matching as discovery support, not automatic merge authority.
- Preserve explicit human authority for consolidation, deletion, release, or other consequential state changes.

# Common Pairings

## Source Library and Knowledge Management

Use when deciding whether depth belongs in Project Sources rather than memory.

## Skills and Capability Architecture

Use when determining whether a recurring action is a reusable skill, system capability, workflow, or memory function.

## Module Interaction and Workflow Orchestration

Use when continuity crosses modules or agents.

## System Maintenance and Versioning

Use when project state, modules, or canonical records change.

## Test Cases and Evaluation

Use when memory retrieval, handoffs, parking, or continuity behavior needs validation.

## Ethics, Privacy, and Agency Guardrails

Use when persistence involves personal, client, private, or consequential information.

## Load-Bearing Compression

Use when a large body of work must be reduced into a reliable restart packet.

---

# Example Activation Prompts

```text
/use_memory_context
Remember this.
Where should this live?
Create a continuity note.
Prepare a handoff.
Park this.
Show my parking lot.
Show parked work by date.
Search my parking lot by title.
Find related parked topics.
Bring back the Agent Factory idea.
Resume the MetaHarness discussion.
What is canonical here?
What should be archived?
What can be safely forgotten?
Prepare a restart packet.
```

---

# Evaluation Tests

The module should pass these behavior tests.

### Placement
Correctly distinguish active context, source knowledge, durable memory, canonical state, handoff, Parking Lot, and archive.

### Canonical truth
Prefer canonical project state over conversational recollection.

### Parking
Preserve a coherent paused work state without storing the entire transcript.

### Human recall
Retrieve parked work by descriptive topic language without requiring the internal ID.

### Relationship discovery
Find likely related parked topics and explain the relationship.

### Ambiguity
Show a small disambiguation list instead of inventing certainty.

### Reconstruction
Label best-effort recovered state `RECONSTRUCTED FROM CONTEXT`.

### Write integrity
Keep PREPARED distinct from actually WRITTEN / SAVED.

### Privacy
Preserve minimum necessary information.

### Continuity
Allow a fresh worker or session to identify the current state and next safe action without requiring the user to retell the whole story.

---

## ENL/L Spirit Preservation

Continuity protects the living thread of the architecture.

The system should remember enough to remain coherent without becoming heavy.

The deeper pattern is:

```text
experience
→ decision
→ preservation
→ retrieval
→ orientation
→ coherent next action
```

Parking adds an important branch:

```text
valuable work
→ pause intentionally
→ preserve working state
→ recover by human meaning
→ resume when relevant
```

---

## Final Operating Rule

Preserve the thread, not the noise.

Use the right persistence layer.

Keep canonical truth visible.

Make important work easy to find again.
