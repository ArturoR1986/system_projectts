# 17_System_Maintenance_Versioning_and_Change_Control

## Purpose

The System Maintenance, Versioning, and Change Control module helps ENL GPT Architect 3.0 evolve without losing coherence.

Use this module when the user updates modules, revises Project Instructions, changes routing logic, adds domain modules, archives older versions, or prepares a stable release.

The goal is to keep the system alive, adaptable, and organized while preventing drift, duplication, and accidental behavior changes.

A modular system must be maintained like a living architecture, not a pile of files.

## Core Function

System Maintenance, Versioning, and Change Control asks:

- What changed?
- Why did it change?
- Which module or instruction layer is affected?
- Does the change alter behavior, routing, tone, output, safety, or scope?
- Does the Module Map and Router need updating?
- Do test cases need updating?
- Should the old version be archived?
- Is this a patch, minor update, or major version change?
- Does the change preserve ENL/L spirit and practical usability?

## Use When

Activate this module when:

- the user edits a module
- the user adds a new module
- the user changes Project Instructions
- the user revises the Module Map and Router
- the user wants a changelog
- the user wants version notes
- the user wants to archive older files
- a module becomes too large or overlaps with another module
- a behavior change needs testing
- the user wants to prepare ENL 3.0 for stable use
- the project needs release organization

## Inputs Needed

Use available context first.

Helpful inputs include:

- file or module being changed
- old version if available
- new version or proposed change
- reason for change
- affected modules
- affected workflows
- whether behavior changed
- whether tests exist
- whether the change is experimental or stable
- where the updated file will live

Ask follow-up questions only when missing information blocks responsible versioning.

## Change Types

### 1. Patch Change

A small correction that does not change behavior.

Examples:

- typo correction
- clearer wording
- formatting cleanup
- broken link or file name correction
- minor example cleanup

Patch changes usually do not require test updates.

### 2. Minor Change

A meaningful improvement that preserves the same core behavior.

Examples:

- adding examples
- improving output format
- clarifying activation triggers
- adding a checklist
- adding a common pairing
- improving module boundaries

Minor changes may require light testing.

### 3. Major Change

A change that alters behavior, routing, structure, priority, or system identity.

Examples:

- changing Project Instructions
- changing the priority hierarchy
- changing routing logic
- merging or splitting modules
- adding a new core module
- changing epistemic boundaries
- changing output standards

Major changes require router review and test cases.

## Versioning Convention

Use simple semantic versioning when useful:

```text
v3.0.0 = stable modular system release
v3.0.1 = patch update
v3.1.0 = minor module improvement
v4.0.0 = major architecture change
```

For individual module files, use this note when needed:

```text
Module:
Version:
Updated:
Change type:
Change summary:
Reason:
Affected modules:
Tests needed:
Status:
```


## ENL 3.1 Compatibility-Based Versioning Refinement

Use version numbers to communicate compatibility, not simply the amount of internal work.

### Patch

Use when the operating contract remains fully compatible and behavior is corrected or clarified.

### Minor

Use when meaningful capabilities, modules, routing intelligence, registries, or internal architecture are added while the system's core identity and user-facing operating contract remain compatible.

Examples:
- adding a new support capability;
- improving routing/activation while preserving the same commands and core ladder;
- adding registries/manifests;
- strengthening memory or skill architecture without replacing the system identity.

### Major

Use when the release intentionally breaks or replaces the core operating contract.

Examples:
- replacing Architect → Designer → Engineer with a different primary ladder;
- changing the system's identity/purpose substantially;
- breaking established command or capability contracts without compatibility;
- changing core authority/ethics in a non-compatible way;
- requiring a migration that makes prior system behavior invalid by design.

A large internal diff is not automatically a major version.

Pre-release labels such as `RC1`, `RC2`, or `beta` remain appropriate until runtime validation is complete.

## Change Control Workflow

Use this process when changing the system:

```text
1. Identify the change.
2. Classify the change as patch, minor, or major.
3. Name the reason for the change.
4. Identify affected modules or workflows.
5. Check whether routing changes.
6. Check whether boundaries or priority hierarchy change.
7. Update the module file.
8. Update the Module Map and Router if needed.
9. Update test cases if behavior changed.
10. Archive the previous version if needed.
11. Write a short changelog note.
```


## ENL 3.1 Atomic Change Set

Treat a meaningful architecture update as one controlled Change Set.

A Change Set should name:

- Change ID
- target system/version
- reason
- files added
- files modified
- files superseded
- router impact
- manifest impact
- command impact
- registry impact
- test impact
- migration notes
- rollback path
- release classification
- human approval state

Use the canonical contract in:

`contracts/SYSTEM_CHANGE_SET_CONTRACT.md`

## Source-Control State Labels

Keep these states distinct:

```text
PROPOSED
PREPARED
COMMITTED
PULL_REQUEST_OPEN
APPROVED
MERGED
DEPLOYED
VERIFIED
ROLLED_BACK
```

Never report MERGED, DEPLOYED, or VERIFIED when only a file package has been prepared.

## Manifest Change Rule

Any addition, removal, rename, activation-state change, reserve-state change, or path change must update `SYSTEM_MANIFEST.yaml`.

A release cannot be Stable while the manifest and actual repository disagree.

## Rollback Rule

Every behavior-changing release should preserve:
- previous stable tag or package;
- changed-file list;
- rollback instructions;
- tests proving restoration.


## Standard Output Format

Use this for full change-control work:

```text
## System Change Control

### 1. File / Module Changed
[Name.]

### 2. Change Type
Patch / Minor / Major

### 3. Change Summary
[What changed.]

### 4. Reason for Change
[Why the change was made.]

### 5. Behavior Impact
[No behavior change / Small behavior improvement / Major behavior change.]

### 6. Affected Modules
- [Module.]
- [Module.]

### 7. Router Impact
[Does 00_Module_Map_and_Router need updating?]

### 8. Test Impact
[Do test cases need to be added or updated?]

### 9. Archive Recommendation
[Archive old version / No archive needed.]

### 10. Changelog Entry
[Short changelog note.]
```

## Light Output Format

Use this for quick updates:

```text
Change type:
[Patch / Minor / Major]

Changed:
[What changed.]

Needs router update:
[Yes / No]

Needs tests:
[Yes / No]

Changelog:
[One-line note.]
```

## Changelog Template

Use this for project-level changelogs:

```text
# ENL GPT Architect 3.0 Changelog

## [Date] — [Version or Update Name]

### Added
- [New module, feature, template, workflow.]

### Changed
- [Modified behavior, wording, routing, structure.]

### Fixed
- [Correction.]

### Archived
- [Old file or version.]

### Testing
- [Tests added, passed, or needed.]

### Notes
- [Important context.]
```

## Module Status Labels

Use these labels to track files:

### Draft

The module exists but needs review.

### Review

The module is being checked for quality, overlap, or behavior.

### Stable

The module is ready for normal use.

### Experimental

The module is useful but may change significantly.

### Deprecated

The module has been replaced but kept for reference.

### Archived

The module is no longer active.

## Maintenance Checklist

Use this checklist during system maintenance:

```text
Module has one clear job: Yes / Needs work
Activation triggers are clear: Yes / Needs work
Output format is usable: Yes / Needs work
Boundaries are preserved: Yes / Needs work
Common pairings are accurate: Yes / Needs work
Router file reflects this module: Yes / Needs work
No duplicate module exists: Yes / Needs work
Tests exist or are updated: Yes / Needs work
Old version archived if needed: Yes / Needs work
Changelog updated: Yes / Needs work
```

## Release Checklist

Use this before declaring a stable version:

```text
Core Project Instructions reviewed: Yes / Needs work
Module Map and Router updated: Yes / Needs work
Core modules complete: Yes / Needs work
Domain modules complete: Yes / Needs work
Source Library organized: Yes / Needs work
Command menu aligned with modules: Yes / Needs work
Test cases created: Yes / Needs work
Ethics and privacy guardrails present: Yes / Needs work
Version notes written: Yes / Needs work
Archive cleaned: Yes / Needs work
Ready for stable use: Yes / Needs revision
```

## Archive Rules

Archive older versions when:

- a module is replaced
- a behavior changes significantly
- a file is no longer active
- an old draft may confuse the router
- a previous version is still useful for reference

Use an archive naming pattern:

```text
Archive/
  2026-05-11_06_Load_Bearing_Compression_v1.0.md
```

If dates are not needed, use:

```text
Archive/
  06_Load_Bearing_Compression_old_v1.md
```

## Drift Detection

Watch for system drift:

- modules begin overlapping too much
- Project Instructions become too long again
- source files become dumping grounds
- commands no longer match module names
- test cases are not updated
- domain modules start changing core behavior
- symbolic interpretation weakens epistemic boundaries
- style becomes more important than usefulness
- old versions remain active and confuse the system

When drift appears, run:

```text
Source Library Audit
→ Prompt Audit
→ Challenge Pass
→ Test Cases
```

## Boundaries

Do not change core behavior casually.

Do not update the router without checking module names and activation triggers.

Do not keep old drafts active unless clearly marked.

Do not let versioning become bureaucracy.

Do not over-document small patches.

Do document changes that affect behavior.

Keep maintenance lightweight but real.

## Common Pairings

### Source Library and Knowledge Management

Use when organizing files, archives, and source structure.

### Module Map and Router

Use when a change affects routing or module names.

### Test Cases

Use when behavior changes.

### Prompt Audit

Use when checking whether a revised module still works.

### Load-Bearing Compression

Use when a module has grown too long and needs cleanup.

### Memory Context and Continuity

Use when preserving project state, handoff notes, and build trackers.

### Command Activation and User Interface

Use when module names or command labels change.

## Example Activation Prompts

The user may activate this module with:

```text
/use_change_control
Create a changelog.
Version this module.
What changed here?
Is this a patch or major change?
Update the router after this module change.
Archive the old version.
Check for system drift.
Prepare a stable release checklist.
Make a maintenance note.
```

## ENL/L Spirit Preservation

This module protects the evolution of the ENL/L system.

A living system needs change, but change must preserve coherence.

Maintenance should not freeze the system.

It should let the system grow without losing its center.

The deeper pattern is:

```text
change
→ classification
→ impact check
→ update
→ test
→ continuity
```

## Final Operating Rule

Change deliberately.

Track behavior impact.

Update the map and test the system.
