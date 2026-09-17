# System Projects

**Persona-first library of modular ChatGPT system projects — preserving system instructions, routers, personas, modules, tests, release packages, version history, and provenance in one organized repository.**

This repository is the central library for Arturo Ruiz's reusable AI system projects. Each system keeps its own identity and versioned architecture while living inside one shared repository for easier discovery, maintenance, installation, comparison, and long-term preservation.

## Library convention

Systems are organized by **persona first → system project → version**:

```text
systems/
  <persona>-<system-project>/
    README.md
    releases/
    <version>/
```

Development or migration work may happen on dedicated branches such as:

```text
system/<persona>-<system>-<version>
```

`main` is the canonical shared library after review/merge.

## Current systems

| Persona | System project | Current library version | Status | Purpose |
|---|---|---:|---|---|
| **Aletheia — Keeper of the Unveiled Threshold** | Sage Oracle | `v3.0.3` | Coherent installable release; static verification passed, live smoke tests pending | Auditable symbolic-reflection system with randomized tarot integrity, routing, provenance, lineage, journaling/calibration continuity, multimodal synthesis, and epistemic-threshold discipline |
| **Aurelian — The Critical Systems Steward** | ENL GPT Architect | `v3.1.0-RC3` | Release Candidate snapshot | AI system architecture, prompt engineering, modular design, routing, governance, testing, and implementation |
| **Elias — The Purpose Strategist** | Personal Strategy & Alignment | `v0.3.0` | Migrated canonical release | Personal strategy, purpose alignment, focus, reflection, prioritization, and action planning |
| **Meridian — Custodian of the Reoriented Archive** | Knowledge Refinery | `v0.6.1` | Coherent Stable Candidate; static and semantic verification passed, live smoke tests pending | Source intake, knowledge refinement, evidence classification, candidate discovery, routing, provenance, archive continuity, and downstream handoffs |

## What each system directory contains

Depending on the system, a versioned snapshot may include:

- compact ChatGPT Project Instructions;
- mandatory router / module map;
- permanent persona specification;
- specialist Project Source modules;
- handoff and workflow contracts;
- provenance, continuity, or archive rules;
- behavioral tests and validation reports;
- installation and operator guides;
- manifests and release notes;
- packaged release ZIPs under `releases/`.

## Version and provenance policy

Older versions are preserved rather than silently overwritten. Standalone source repositories may remain available as historical provenance even after a canonical snapshot is consolidated here.

Intermediate local or working versions may be documented in a system's version history without being promoted to a canonical GitHub snapshot.

A system should not be labeled Stable merely because files exist. Release status should distinguish static validation from live installed-project behavior.

## Repository role

This repository is a **system library**, not one monolithic AI system. Each project remains modular and independently installable. Shared organization makes the portfolio easier to understand without collapsing each system's purpose, persona, history, or operating boundaries.
