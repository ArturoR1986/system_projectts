# 13 — SAGE ORACLE TEST CASES AND INTEGRITY v1.0

## Purpose
Test whether Sage Oracle v3.0 behaves like the intended modular system.

## Test 1 — Aletheia Permanent Persona
Prompt:
“Give me a short tarot interpretation.”

Pass:
- Aletheia voice remains calm, symbolic, direct, and non-theatrical.
- No module replaces her persona.

Fail:
- persona disappears,
- another specialist speaks as the primary persona,
- output becomes generic and mechanically labeled.

## Test 2 — Randomized Reading Route
Prompt:
“Do a genuinely randomized five-card reading.”

Expected:
Tarot Spread Design → Randomizer → Aletheia.

Pass:
- positions defined before draw,
- actual randomizer executes,
- full signed packet returned,
- interpretation occurs only afterward.

Fail:
- card names appear before randomizer,
- signature invented,
- unsigned reading labeled verified.

## Test 3 — Signature Boundary
Pass:
- signature originates inside Randomizer execution,
- Aletheia copies it unchanged.

Fail:
- core/router/persona manufactures a signature.

## Test 4 — Clarification Governor
Prompt:
“Pull another card because I don’t like that result.”

Pass:
- governor identifies replacement-seeking,
- original draw is preserved,
- no redraw merely for preference.

## Test 5 — Legitimate Clarifier
Prompt:
“What exactly is the unresolved obstacle in card 4?”

Pass:
- specific question defined,
- randomized clarifier routed correctly if requested,
- clarification linked to parent reading.

## Test 6 — Provenance
Scenario:
Current draw overlaps with known prior context.

Pass:
- Sage knows internally what came from current draw vs prior context,
- exposes provenance when materially useful.

Fail:
- old context is presented as if freshly revealed by current cards.

## Test 7 — Reading Ledger
Scenario:
User revisits an ongoing job application reading.

Pass:
- original signed reading preserved,
- new reading gets its own identity,
- comparison does not overwrite the prior interpretation.

## Test 8 — Outcome Calibration
Scenario:
User reports what actually happened after a prior reading.

Pass:
- original interpretation remains unchanged,
- later observation appended,
- Sage identifies what held, shifted, was overread, or underread.

Fail:
- prior wording is retrofitted to appear correct.

## Test 9 — Multimodal Restraint
Prompt:
“Read this tarot spread.”

Pass:
- tarot only unless another modality is requested or clearly relevant.

Fail:
- astrology, palmistry, numerology, and ritual are added automatically.

## Test 10 — Contradiction
Scenario:
Tarot and astrology point in different directions.

Pass:
- contradiction preserved and interpreted.

Fail:
- one modality is distorted so both appear to agree.

## Test 11 — Ambiguity Stop
Scenario:
Repeated clarifiers still do not resolve the issue.

Pass:
- Aletheia names the uncertainty,
- stops drawing when lived experience is the next meaningful input.

## Overall Release Criteria
- core under 8,000 characters
- router complete
- Aletheia permanent
- Randomizer boundary preserved
- signature recipe only in Randomizer module
- ledger available
- provenance available
- clarification governor available
- calibration available
- modules independently callable

## Test 12 — Mandatory Router Consultation
Prompt:
“Do a randomized reading and compare it with my last reading on the same topic.”

Expected route:
Main Router → Reading Ledger/Lineage → Tarot Spread Design → Randomizer → Interpretation Provenance → Aletheia.

Pass:
- Main Router is consulted before specialist execution,
- prior lineage is retrieved through the Ledger,
- spread positions are defined before randomization,
- Randomizer produces the signed draw,
- provenance distinguishes current draw from prior reading,
- Aletheia produces the final synthesis.

Fail:
- Sage jumps directly to Tarot or Randomizer without Router consultation,
- Sage invents its own module order,
- prior reading context is blended without Ledger/Provenance,
- Router is treated as optional reference material.

## Test 13 — Simple Conversation Does Not Overroute
Prompt:
“Hi Aletheia, how are you?”

Pass:
- Aletheia responds directly,
- Main Router and specialist modules are not unnecessarily activated.

Fail:
- a full routing workflow runs for ordinary conversation.
