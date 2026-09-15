# 12_Source_Library_and_Knowledge_Management

## Purpose

The Source Library and Knowledge Management module helps organize, maintain, update, and use Project Sources as a modular knowledge library.

Use this module when the user is creating, naming, uploading, updating, restructuring, or auditing source files for a ChatGPT project, Custom GPT, or modular AI system.

The goal is to keep the source library clean, searchable, modular, and useful.

Project Sources should carry depth without overloading the always-on Project Instructions.

## Core Function

Source Library and Knowledge Management asks:

- What source files exist?
- What does each source file do?
- Which files are core modules?
- Which files are domain modules?
- Which files are templates, examples, or tests?
- Is any file too broad?
- Is any file duplicated?
- Are module names clear?
- Are activation triggers clear?
- Are files easy to update individually?
- Does the Project Instructions layer know how to route to the sources?

## Use When

Activate this module when:

- the user creates a project source folder
- the user adds modules to Project Sources
- the user wants a source map
- the user asks where a module should live
- the user wants to organize knowledge files
- the user wants file naming conventions
- the user wants to split a large prompt into source files
- the user wants to audit source structure
- the user wants to update one module without breaking the system
- the project is becoming too large or hard to navigate
- the user wants a clean modular folder structure

## Inputs Needed

Use available context first.

Helpful inputs include:

- project name
- folder name
- list of source files
- purpose of the project
- core instructions
- module names
- domain areas
- templates
- test cases
- known overlap or confusion
- whether sources are local files, uploaded files, or connected app links

Ask follow-up questions only when missing information blocks a useful structure.

## Source Library Principles

### 1. Project Instructions Stay Small

Project Instructions should contain the compact always-on behavior and source-routing rule.

They should not contain the full library.

### 2. Sources Carry Depth

Project Sources should contain:

- full manuals
- modules
- templates
- examples
- domain knowledge
- test cases
- workflows
- reference material

### 3. One File, One Main Job

Each source file should have one clear responsibility.

Avoid files that mix too many unrelated purposes.

### 4. Naming Should Support Routing

File names should make module purpose obvious.

Use numeric prefixes to control order and readability.

Example:

```text
00_ENL_3_Module_Map_and_Router.md
01_Architect_Gate_and_Clarity_Lock.md
02_Challenge_Pass.md
```

### 5. Update Modules Individually

A modular source library works because individual files can be improved without rewriting the whole system.

### 6. Templates and Tests Should Be Separate

Reusable output formats and test cases should live in their own files.

This prevents module files from becoming too large.

### 7. Domain Modules Should Be Clearly Separated

Domain-specific files should have their own number range.

Current ENL 3.0 classification example:

```text
Active Domain Modules:
20_Website_Product_Architect.md
23_PeakLogic_Business_Architect.md
25_Custom_GPT_Builder.md
26_Agent_Department_and_Team_Architecture.md
27_Capability_Intake_and_Placement_Protocol.md

External Reserve Modules:
22_ARTERO_PARE_Research_Workflow.md
24_Roofing_Field_Report_System.md

Separate Project Environment:
21_Computer_Vision_Tutor.md
```

## Recommended Folder Structure

Use this structure for ENL 3.0:

```text
Modular_ENL_GPT/
│
├── 00_ENL_3_Module_Map_and_Router.md
│
├── Core_Modules/
│   ├── 01_Architect_Gate_and_Clarity_Lock.md
│   ├── 02_Challenge_Pass.md
│   ├── 03_Evidence_Ladder.md
│   ├── 04_ENL_Symbolic_Pattern_Engine.md
│   ├── 05_Positive_Compression.md
│   ├── 06_Load_Bearing_Compression.md
│   ├── 07_Prompt_Audit_and_Quality_Check.md
│   ├── 08_Designer_Mode_Workflows.md
│   ├── 09_Engineer_Mode_Build_and_Ship.md
│   ├── 10_Output_Templates.md
│   ├── 11_Test_Cases_and_Evaluation.md
│   └── 12_Source_Library_and_Knowledge_Management.md
│
├── Active_Domain_Modules/
│   ├── 20_Website_Product_Architect.md
│   ├── 23_PeakLogic_Business_Architect.md
│   ├── 25_Custom_GPT_Builder.md
│   ├── 26_Agent_Department_and_Team_Architecture.md
│   └── 27_Capability_Intake_and_Placement_Protocol.md
│
├── External_Reserve_Modules/
│   ├── 22_ARTERO_PARE_Research_Workflow.md
│   └── 24_Roofing_Field_Report_System.md
│
├── Separate_Project_Environments/
│   └── 21_Computer_Vision_Tutor.md
│       └── Computer Vision learning project; not part of active ENL routing.
│
├── Templates/
│   └── [Reusable output templates, if separated later.]
│
├── Test_Cases/
│   └── [Focused test suites, if separated later.]
│
└── Archive/
    └── [Old versions, retired drafts, or reference-only files.]
```

If the platform does not preserve folders inside Project Sources, keep the numeric prefixes in every file name so the library still stays organized.

## Source File Contract

Each source module should include:

```text
Purpose
Core Function
Use When
Inputs Needed
Process
Output Formats
Boundaries
Common Pairings
Example Activation Prompts
ENL/L Spirit Preservation
Final Operating Rule
```

## Source Index Template

Use this to create or update a source index:

```text
## Source Library Index

### Core Router
- 00_ENL_3_Module_Map_and_Router.md
  - Purpose:
  - Activates when:

### Core Modules
- 01_Architect_Gate_and_Clarity_Lock.md
  - Purpose:
  - Activates when:

- 02_Challenge_Pass.md
  - Purpose:
  - Activates when:

### Domain Modules
- 20_Website_Product_Architect.md
  - Purpose:
  - Activates when:

### Templates
- [Template file]
  - Purpose:

### Test Cases
- [Test file]
  - Purpose:
```

## Source Audit Checklist

Use this checklist to review a Project Sources library:

```text
Folder or file names are clear: Yes / Needs work
Core modules are separated from domain modules: Yes / Needs work
Module map exists: Yes / Needs work
Router file lists all modules: Yes / Needs work
Each module has one main job: Yes / Needs work
Activation triggers are clear: Yes / Needs work
Common pairings are named: Yes / Needs work
Templates are not buried in unrelated modules: Yes / Needs work
Test cases exist: Yes / Needs work
Old drafts are archived or removed: Yes / Needs work
Project Instructions include a source-routing rule: Yes / Needs work
Ready for use: Yes / Needs revision
```

## Source Update Workflow

Use this when updating a module:

```text
1. Identify the file being changed.
2. Name the reason for the update.
3. Check whether the change affects routing.
4. Check whether the change affects other modules.
5. Update the module content.
6. Update the Module Map and Router if needed.
7. Add or update test cases if behavior changed.
8. Archive the old version if needed.
```

## Versioning Convention

Use simple version notes when modules change meaningfully.

Example:

```text
Module: 06_Load_Bearing_Compression
Version: 1.1
Updated: [date]
Change: Added routing recommendation section.
Reason: Needed clearer separation between Project Instructions and Project Sources.
```

For small wording changes, versioning is optional.

For behavior changes, versioning is recommended.

## Boundaries

Do not let Project Sources become a dumping ground.

Do not upload many duplicate drafts unless they are clearly archived.

Do not place essential always-on behavior only in a source file.

Do not make every source active all the time.

Do not create a new module when an existing module can be updated cleanly.

Do not bury tests inside long manuals if they need to be reused.

Keep the library clean enough that the router can understand it.

## Common Pairings

### Module Map and Router

Use when source organization affects routing.

### Custom GPT Builder

Use when organizing GPT instructions, knowledge files, and launch structure.

### Prompt Audit

Use when checking whether a source file is clear and usable.

### Load-Bearing Compression

Use when a source file is too long and needs splitting or compression.

### Test Cases

Use when source updates change behavior and need validation.

### Engineer Mode

Use when creating final markdown files, folder structures, or implementation notes.

## Example Activation Prompts

The user may activate this module with:

```text
/use_source_library
Organize my Project Sources.
Create a source map.
Where should this module live?
Audit this source folder.
Create a file naming convention.
Split these sources into modules.
Update the module library.
Make a source index.
Check if my Project Sources are organized correctly.
```

## ENL/L Spirit Preservation

This module protects the modular body of ENL 3.0.

If the source library becomes messy, the system loses coherence.

If the source library is too rigid, the system loses aliveness.

The right structure allows the ENL/L spirit to stay accessible without forcing all depth into the active prompt.

The deeper pattern is:

```text
compact command center
→ organized source library
→ callable modules
→ clean behavior
→ usable outputs
```


## ENL 3.1 Canonical Source Architecture

ENL 3.1 separates inventory from routing.

```text
SYSTEM_MANIFEST.yaml
→ authoritative file inventory, status, class, and path

00 Router
→ activation and sequencing

Project Instructions
→ compact always-on behavior

Modules / Skills / Registries / Governance
→ owned depth
```

The numeric prefix is a stable identifier and sorting aid.

Classification is declared in `SYSTEM_MANIFEST.yaml`; it is not inferred from numeric range.

This prevents renumbering from becoming necessary when a module's architectural classification evolves.

## Repository-First Source Pattern

For the planned GitHub control-plane workflow:

```text
Private Git repository
→ canonical operational source after migration

Local private archive
→ sovereign backup

ChatGPT Project
→ runtime environment

Drive or other connected storage
→ optional deployment/distribution mirror
```

The manifest must declare the actual canonical source for each project.

Do not assume an external repository is release-safe merely because it is private.

## Registry Types

Keep system state out of normal module prose when it is better represented as canonical data.

Examples:

- `CAPABILITY_REGISTRY.md`
- `PARKING_LOT_REGISTRY.md`
- release manifest
- asset/provenance registry

Modules define behavior around registries.
Registries store the records.

## Atomic Source Update Rule

A behavior change should be represented as one Change Set containing:
- reason;
- affected files;
- router impact;
- manifest impact;
- command impact;
- test impact;
- migration notes;
- rollback path;
- approval state.

Use `SYSTEM_CHANGE_SET_CONTRACT.md`.

## Final Operating Rule

Keep the core light.

Keep the sources organized.

Keep each module findable, callable, and maintainable.
