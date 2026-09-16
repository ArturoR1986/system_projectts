# Aletheia — Sage Oracle v3.0.3 — Local Installation

## 1. Project Instructions

Copy the complete contents of:

`01_PROJECT_INSTRUCTIONS/Sage_Oracle_System_Instructions_v3.0.3.md`

into the ChatGPT Project Instructions field.

## 2. Project Sources

Add every Markdown file inside:

`02_PROJECT_SOURCES/`

as Project Sources.

The runtime source set is modules 00 through 14.

## 3. Workspace Reference

`03_WORKSPACE_REFERENCE/README_Sage_Oracle_Workspace.md`

documents the intended continuity structure:

- 00 — System Modules
- 01 — Reading Ledger
- 02 — Journal
- 03 — Calibration & Outcomes
- 04 — History & Archive
- 05 — Handoffs & Work Orders

This workspace reference is **not** a runtime Project Source.

## 4. Critical Boundaries

- Main Router is mandatory for non-trivial Sage Oracle work.
- Aletheia remains the permanent user-facing persona.
- Randomizer alone owns randomized card selection, Draw IDs, locked draws, and Randomizer Signatures.
- Reading Ledger preserves the immutable reading record.
- Journal preserves reflection and lived integration; it does not rewrite the Reading Ledger.
- Calibration appends later review; it does not retrofit the original reading.
- Interpretation Provenance tracks where a claim came from.
- Module 14 governs epistemic status when scientific, philosophical, metaphysical, occult, symbolic, or experiential claims cross a real threshold.
- Module 14 is not another divination modality.
- Journals, ledger entries, calibration records, history, and handoffs are continuity artifacts, not runtime Project Sources by default.

## 5. Recommended Smoke Tests

Run the tests defined in `13_Test_Cases_and_Integrity.md`.

System version: **v3.0.3**.
