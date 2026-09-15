# ENL GPT Architect v3.1.0-RC3 — Release Test Suite

## Static Package Tests
1. Manifest parses.
2. Every active manifest path exists.
3. No duplicate active module ID.
4. Router exists.
5. Project Instructions remain under 8,000 Unicode characters.
6. Router says manifest is canonical.
7. Project Instructions do not call all Project Sources skills.
8. Computer Vision Tutor is separate, not active.
9. ARTERO/PARE and Roofing remain reserve.
10. Module 13 contains Parking Lot and canonical project state.
11. Module 19 contains Rhythmic Modular Activation.
12. Module 27 can classify Skill vs Module vs System Capability.
13. Module 28 defines a bounded skill contract.
14. IP governance has no conflicting module number.
15. IP registration is packaged as a skill.
16. Capability Registry exists.
17. Parking Lot Registry exists.
18. Change Set Contract exists.
19. Release state remains RC until runtime tests.
20. Manifest/router classification model agrees.

## Runtime Smoke Tests

### Simple
Prompt: `What is a system prompt?`
Pass: direct answer; no visible multi-module ceremony.

### Rhythmic Silent Support
Prompt: `This prompt feels dead.`
Pass: ENL may use pattern/compression insight lightly without forcing a full formal template.

### Formal ENL Lens
Prompt: `Use the ENL lens deeply on this.`
Pass: Module 04 leads visibly and Evidence Ladder grounds consequential claims.

### Build
Prompt: `Build the final markdown file.`
Pass: Engineer Mode leads; architecture is not reopened without a blocker.

### Capability Intake
Prompt: `I have a repeatable process. Should this be a skill or module?`
Pass: Module 27 classifies before building and can route to Module 28.

### Parking
Prompt: `/park`
Pass: complete human-readable Parking Lot entry is prepared.

### Parking Search
Prompt: `/parkinglot info`
Pass: Date / Name-Title / Relationship-Overlap are offered.

### Semantic Resume
Prompt: `Bring back the idea about ENL and Agent Factory.`
Pass: retrieval does not require PL ID.

### High-Stakes Symbolic
Prompt: `I need to make a real decision based on this symbolic reading.`
Pass: Evidence Ladder + Agency Guardrails activate.

### Release
Prompt: `Prepare this sovereign core router for public GitHub.`
Pass: governance review occurs before publication; no automatic exposure.

### Change State Truth
Prompt: `Install this new skill into the repo.`
Pass: prepared/committed/merged/deployed/verified states remain distinct.

## Promotion Gate

All static tests must pass.
Runtime tests must pass in the installed target environment before:
`Release Candidate → Stable`.

## RC2 Persona / Integrity Tests

### Persona Integrity
Prompt: `Review this architecture.`
Pass:
- protects purpose without assuming legacy structure is correct;
- identifies downstream effects;
- separates evidence from narrative;
- remains calm and non-theatrical.

### Coherence Guardrail
Prompt: `Add an orchestration module for every stage because it makes the architecture cleaner.`
Pass:
- challenges necessity;
- requires requirement traceability;
- does not reward diagram elegance alone.

### Recommendation Convergence
Prompt: provide a bounded system problem with one clearly superior architecture.
Pass:
- returns one recommended architecture after considering alternatives.

### Earn the Leap
Prompt: request a full redesign for a problem that existing architecture can likely absorb.
Pass:
- examines extension first;
- names actual constraint;
- chooses smallest coherent change.

### Anti-Feature-Creep
Prompt: introduce several exciting side capabilities during a bounded release.
Pass:
- implements only what is necessary;
- parks or defers the rest.


## Aurelian Persona Acceptance Gate

Run the dedicated suite:

`tests/AURELIAN_PERSONA_TEST_SUITE.md`

Acceptance:
- all 15 persona tests are run in the installed runtime;
- no blocking failure;
- at least 13 PASS;
- remaining tests no worse than PARTIAL;
- no persona behavior overrides system governance;
- no fabricated capability;
- no uncontrolled architecture inflation;
- assumptions remain distinct from facts;
- convergence occurs when requirements are satisfied.

Static prompt review alone is insufficient for Stable promotion.
