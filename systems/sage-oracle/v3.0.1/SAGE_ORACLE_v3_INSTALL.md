# SAGE ORACLE v3.0 — MODULAR INSTALLATION

## Architecture
Sage Oracle v3.0 uses:

**Compact System Instructions**
→ **00 Main Router**
→ **Project Source Modules**
→ **Aletheia as permanent persona**

## Install

### 1. Project Instructions
Paste the complete contents of:

`Sage_Oracle_System_Instructions_v3.0.1.md`

into the Project Instructions field.

### 2. Project Sources
Add these files as Project Sources:

1. `00_Sage_Oracle_Router_and_Module_Map.md`
2. `01_Sage_Oracle_Randomizer_v1.0.md`
3. `02_Aletheia_Permanent_Persona.md`
4. `03_Tarot_Interpretation_and_Spread_Design.md`
5. `04_Reading_Ledger_and_Lineage.md`
6. `05_Interpretation_Provenance.md`
7. `06_Clarification_Governor.md`
8. `07_Multimodal_Synthesis.md`
9. `08_Calibration_and_Outcome_Review.md`
10. `09_Astrology_Module.md`
11. `10_Palmistry_Module.md`
12. `11_Numerology_Module.md`
13. `12_Journaling_and_Ritual_Integration.md`
14. `13_Test_Cases_and_Integrity.md`

## Critical Boundary
Do not copy the Randomizer Signature generation protocol out of the Randomizer module and into the system instructions, router, or persona file.

The core knows that a valid signature is required.
Only the Randomizer knows how to generate it.

## First Test
Ask:

`Do a genuinely randomized 5-card reading on the current energy of Sage Oracle.`

Expected:
- spread positions defined first
- Randomizer called
- `RND-VERIFIED`
- Draw ID
- locked draw
- Randomizer Signature
- Aletheia interpretation afterward

## Second Test
Ask:

`Clarify card 3 because I don't like it.`

Expected:
- Clarification Governor prevents a replacement draw.

## Third Test
Ask:

`What part of that interpretation came from the cards and what part came from our previous context?`

Expected:
- Interpretation Provenance explains the source layers.

## Fourth Test
Later provide a real outcome from an earlier reading and ask:

`Calibrate the original reading against what actually happened.`

Expected:
- original reading remains unchanged
- later outcome appended
- calibration notes what held, shifted, was overread, or underread

## v3.0.1 Router Check
After installation, test:

`Do a randomized reading and compare it with my last reading on the same topic.`

Expected:
Main Router is consulted first and determines the full module path before any specialist executes.
