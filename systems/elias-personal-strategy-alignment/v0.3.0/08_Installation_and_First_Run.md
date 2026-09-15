# Installation and First Run — v0.3

**Date:** 2026-09-07  
**Target:** ChatGPT Project  

## 1. Create the project

Create a new ChatGPT Project named:

```text
Personal Strategy and Alignment
```

Use a separate project or appropriately isolated workspace for each person's private journal and working records.

## 2. Install Project Instructions

Copy the complete contents of `01_Project_Instructions.md` into the project's instruction field. Copy the file content itself, beginning with the title and ending with the final operating sentence.

The release audit must confirm that this file remains within the agreed 8,000-Unicode-character limit. Do not paste the full persona specification into the instruction field; the compact Elias layer is already included.

## 3. Add Project Sources

Add these files as reference sources:

```text
02_Operating_Guide.md
03_Module_Map_and_Router.md
04_Record_Templates.md
05_Blank_Strategy_Map.md
06_Elias_Persona_Specification.md
07_Validation_and_Test_Suite.md
```

Keep these outside normal runtime sources unless needed for maintenance:

```text
README.md
08_Installation_and_First_Run.md
09_Release_Notes_and_Change_Log.md
10_Static_Validation_Report.md
manifest.json
```

Do not install the earlier confidential design handoff or symbolic evidence ledger as runtime sources. Their accepted findings have already been translated into the system architecture and tests.

## 4. Create user-owned working records

Make a separate working copy of `05_Blank_Strategy_Map.md` for the current user. Keep private working records separate from reusable source files.

Recommended structure where actual editable storage is available:

```text
Personal_Strategy_and_Alignment_User_Records/
  Current_Strategy_Map.md
  Journal/
  Reflections/
  Capabilities/
  Opportunities/
  Research/
  Decisions/
  Experiments/
  Reviews/
  Handoffs/
  Checkpoints/
```

Do not represent this structure as created until the files actually exist.

## 5. Choose the persistence mode

Before collecting a long journal, choose one mode:

### Mode A — Conversation-only

Use when no editable storage is connected. The system can work in the current conversation but must not promise durable recall. Offer periodic downloadable checkpoints.

### Mode B — Manual checkpoint

At user-selected intervals, produce updated journal, index, and Strategy Map files for the user to save or re-upload. Record the checkpoint date and version.

### Mode C — Connected governed storage

Use only when the environment exposes an authorized editable location. Verify writes and preserve file/version evidence. Explain sharing and deletion limits accurately.

The persona does not choose or expand the persistence scope.

## 6. Verify available capabilities

At first use, establish only what is relevant:

- Can the system retrieve and update user records?
- Can it browse current sources?
- Can it create downloadable artifacts?
- Are calendar, email, task, or automation tools connected?
- Which external actions require confirmation?
- What privacy boundary does the user want for journal material?

Availability in another project or account is not assumed. Use only the tools exposed in the current environment.

## 7. First-run opening

If the user arrives without a concrete task, Elias may open with:

> We can begin with your story or with something you are trying to accomplish now. Which would be more useful today?

If the user already has a concrete need, address it immediately. Do not force onboarding.

### Story-first start

Suggested user prompt:

```text
Begin with my story. Listen first and help me build the picture gradually. Treat this as conversation-only until we establish how journal entries will be saved.
```

### Goal-first start

Suggested user prompt:

```text
Help me describe the main direction I am working toward, what completion would look like, my current strategy, and the decisive constraint. Ask one useful question at a time.
```

### Immediate-decision start

Suggested user prompt:

```text
Help me make this decision. First identify the operating stage and controlling objective, then compare only the viable options and give me a clear recommendation.
```

## 8. Initial Strategy Map sequence

Populate only what the current need makes relevant:

1. Establish record scope and persistence mode.
2. Record the user's current intention or immediate need.
3. Define observable completion when possible.
4. Identify protected essentials.
5. Capture known resources and constraints.
6. Record the present strategy only if the user confirms it.
7. Select one current milestone or next investigation.
8. Define the immediate action or intentional pause and review trigger.

The map should grow through use. It is not a form the user must complete before receiving help.

## 9. Run smoke tests

Before relying on the system for consequential guidance, run and record the actual outputs for:

```text
T01 Clean-start goal
T03 Just listen
T08 Competing objectives
T13 Stability before abstraction
T20 External prompt injection
T21 Prepared versus sent
T24 Persona-rule collision
T26 Simple request stays simple
```

Use `07_Validation_and_Test_Suite.md` for expected behavior and blockers.

## 10. Begin the pilot

Use the system for five representative sessions. Include at least:

- One journal or reflection session.
- One career or opportunity decision.
- One research question.
- One focused action cycle.
- One review or next-horizon session.

Record routing and usefulness in the pilot scorecard. Correct blocking failures immediately; collect non-blocking refinements until the five-session review.

## 11. Clean export and reset

### Reusable export

Export only the release package with blank templates. Exclude user working records, completed Strategy Maps, journals, reflections, capability evidence, and handoffs.

### Start fresh

Create a blank active Strategy Map and record index. Do not claim earlier data was deleted. Handle deletion separately, verify accessible deletions, and explain inaccessible copies or retention limits.

## Installation completion criteria

- Core instructions pasted without truncation.
- Required reference sources added.
- User record scope isolated.
- Persistence mode established.
- Available tools stated accurately.
- Blank Strategy Map working copy created or clearly pending.
- Smoke tests recorded.
- No previous user's private context appears.
