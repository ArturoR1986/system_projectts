# ENL GPT Architect v3.1.0-RC3

## RC3 — Aurelian Persona Installation

RC3 installs **Aurelian — The Critical Systems Steward** as the canonical behavioral reasoning persona.

This is not a new functional module.

The original persona handoff package is preserved intact under `release/source_handoffs/` for provenance and checksum verification.

Active integration is intentionally small:
- one canonical persona specification;
- one integration contract;
- one dedicated persona validation suite;
- compact kernel in Project Instructions;
- router/manifest references;
- release provenance outside runtime.

The supplied symbolic reading remains design provenance only and is not technical evidence.

## Release Theme

**Canonicalization + Activation Intelligence**

This release preserves the ENL 3.0 identity and Architect → Designer → Engineer ladder while integrating the architectural lessons discovered since RC1.

## RC2 Refinement

RC2 adds a behavioral reasoning persona and four architectural integrity rules derived from external review and internal Challenge Pass:

- Critical Systems Steward persona
- Architectural coherence is not evidence of architectural correctness
- Explore broadly. Recommend narrowly
- Earn the leap

These refine behavior without adding another functional module.

## Main Changes

1. Adds `SYSTEM_MANIFEST.yaml` as canonical inventory.
2. Makes numeric module prefixes stable identifiers rather than classification rules.
3. Replaces “Project Sources = skills” with explicit distinctions between modules, skills, system capabilities, and registries.
4. Promotes the expanded Memory/Continuity architecture, including canonical project state and Parking Lot continuity.
5. Adds Rhythmic Modular Activation to runtime/orchestration/router/tests without creating another module.
6. Replaces New Module Intake with Capability Intake and Placement.
7. Adds Skills and Capability Architecture as Module 28.
8. Resolves the Module 28 collision by moving IP governance outside normal module numbering and converting IP Registration into a bounded skill.
9. Adds Capability and Parking Lot registries.
10. Adds a System Change Set Contract to prepare for GitHub-based automated updates.
11. Keeps Computer Vision Tutor as a separate project module.
12. Keeps ARTERO/PARE and Roofing Field Report as reserve modules.

## Canonical Model

```text
Project Instructions
→ SYSTEM_MANIFEST
→ Router
→ Modules / Skills / System Capabilities
→ Registries
→ Tests
→ Change Control
→ Release Governance
```

## Release State

Static Release Candidate.

Do not call Stable until installed runtime smoke tests and behavior tests pass.

## Installation Direction

For current ChatGPT Project runtime:
- use `PROJECT_INSTRUCTIONS.md` as the compact Project Instructions;
- load/supply the current router and active modules according to `SYSTEM_MANIFEST.yaml`;
- keep reserve/separate/governance assets in their declared locations;
- test before Stable.

For the planned cloud workflow:
- migrate this release into a private Git repository;
- treat the repository as canonical operational source after migration;
- retain a local private sovereign backup;
- build automation around `SYSTEM_CHANGE_SET_CONTRACT.md`.

## Repository packaging note

The original Rhythmic Activation study guide PDF is preserved in the local/release archive. The GitHub canonical source stores a Markdown repository reference instead, because the connected repository writer is text-first. This does not change runtime behavior or the provenance boundary.
