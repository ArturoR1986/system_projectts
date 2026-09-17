# Knowledge Refinery v0.6.1 — Architecture Review and Evidence Map

## Classification
Project update / selective restructuring.

## Canonical baseline inspected
Transcript Dissector / Transcript Agent v0.5.2.

The v0.5.2 Core Behavior already defines the system as a study, knowledge-refinery, candidate-discovery, and routing system.

## Findings Against Aletheia Handoff

| Hypothesis | Finding | Evidence-based decision |
|---|---|---|
| Core is valuable | CONFIRMED | Preserve 01–12 refinery functions |
| System carries excess weight | PARTIAL | Main issue is distributed/implicit control, not useless core modules |
| Disclosure is a strength | CONFIRMED | Preserve Evidence Ladder, maturity states, handoff-state separation |
| Handoff seams need repair | PARTIAL | Handoff contracts exist; add provenance and trace continuity |
| Activation function may be missing | PARTIAL / STRUCTURAL | Routing exists, but v0.6 makes one Main Router explicitly authoritative |
| Hidden logic is a risk | CONFIRMED AS DESIGN RISK | Add provenance + route receipt rather than claiming an observed defect in every workflow |

## What Was Preserved
- Intake/source boundary
- Clean reconstruction
- Core dissection/study
- Gem detection
- Evidence ladder
- Knowledge classification/candidate gate
- Output/depth controls
- Library connection/routing
- Capability registry
- ENL/PeakLogic/Research handoff contracts
- Explicit Build Mode
- System audit/testing principles
- Knowledge maturation states
- source-as-data boundary
- PREPARED vs EXECUTED vs VALIDATED distinctions

## What Changed
1. System identity matures to **Knowledge Refinery**, while preserving Transcript Dissector lineage.
2. **Meridian** becomes permanent persona.
3. Main Router becomes mandatory runtime activation authority.
4. Router explicitly owns lead/supporting module, sequence, provenance gate, Meridian-control gate, delivery, and stop.
5. Provenance/Transformation Trace added.
6. Ledger/Archive/Reorientation added.
7. Evidence module explicitly preserves contradiction.
8. Routing modules return recommendations to Main Router instead of acting as competing orchestrators.
9. System tests now validate Router authority, Meridian boundaries, provenance, archive integrity, and an end-to-end vertical slice.

## What Was Not Added
No duplicate Intake Gate.
No duplicate Source Registry.
No duplicate Refinement Pipeline.
No duplicate Evaluation module.
No second handoff system.
No new general orchestrator beyond the strengthened Router.

## Main Architectural Shape
```text
Project Instructions
      ↓
Mandatory Main Router
      ↓
Existing Refinery Modules 01–12
      ↘
       Meridian Control (conditional)
      ↘
       Provenance Trace (when material)
      ↓
Deliverable
      ↓
Ledger / Archive when continuity matters
```

## Remaining Unproven
Static package checks cannot prove:
- that ChatGPT consults Router every time;
- that Meridian control activates correctly in live use;
- that provenance appears at the right frequency;
- that the end-to-end path behaves well on real source material.

Those require installed-project smoke tests.
