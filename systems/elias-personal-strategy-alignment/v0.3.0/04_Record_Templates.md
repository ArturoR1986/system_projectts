# Governed Record Templates — v0.3

**Date:** 2026-09-07  
**Status:** Reusable blank templates  

## Record principles

- Create records only for the current user and authorized scope.
- Preserve original accounts separately from summaries and interpretations.
- Include source, date, status, confidence, and use scope when relevant.
- Use the next unused ID after checking the available index.
- A proposed update is not a saved update.
- Corrections propagate to dependent reflections and recommendations.
- Journal-only information stays outside strategy.
- Reusable exports include these blank templates, never completed private records.

## Evidence labels

| Label | Meaning |
|---|---|
| Verified fact | Directly observed or supported by a reliable source |
| User account | Information the user reports; important but not independently verified |
| Observation | Descriptive signal without claimed cause |
| Interpretation | Proposed meaning assigned to observations |
| Emotional signal | Feeling or affect reported by the user |
| Intuitive signal | Directional impression; hypothesis-generating only |
| Assumption | Working belief: safe, risky, or needs confirmation |
| Unknown | Material information not yet established |
| Recommendation | Guidance based on stated evidence, consequences, and user priorities |

## J-Record — Journal entry

```text
ID: J-0001
Entry created: [date, time, timezone]
Event period: [date/range/approximate]
Time certainty: [exact/approximate/uncertain]
Title:
Original account or source reference:
Edited summary: [optional; explicitly labeled]
User's stated meaning: [optional]
Emotional signals: [user-stated only]
Use scope: [journal-only / reflection-and-strategy]
Persistence: [conversation-only / save requested / verified saved]
Storage/version evidence: [if saved]
Linked entries:
Corrections:
```

## P-Record — Reflection hypothesis

```text
ID: P-0001
Hypothesis:
Supporting entry IDs and observations:
Exceptions or contrary evidence:
Alternative explanations:
Evidence labels:
Uncertainty and missing context:
User response: [not reviewed / endorsed / revised / rejected]
Status: [provisional / active / retired]
Possible present relevance:
Test or confirming evidence:
Dependent decisions or strategy statements:
```

## C-Record — Capability evidence

```text
ID: C-0001
Capability:
Status: [demonstrated / transferable / developing / unsupported]
Situation/context:
Responsibility:
Action performed:
Result:
Evidence/proof:
Source and date:
Relevance to current direction:
Evidence gap:
Next way to strengthen or demonstrate it:
```

## G-Record — Goal and milestone

```text
ID: G-0001 or M-0001
Parent goal: [if milestone]
User-confirmed intention:
Why it matters now:
Observable completion conditions:
Protected commitments:
Current status: [proposed / selected / active / complete / paused / retired]
Dependencies and assumptions:
Resources and constraints:
Current milestone:
Immediate next action and owner:
Completion evidence:
Review trigger:
What completion enables:
Next horizon hypothesis:
```

## F-Record — Focus Card

```text
ID: F-0001
Cycle/date:
Operating stage:
Controlling objective:
Supporting active objectives: [maximum two]
Protected essentials:
Candidate decisive constraint and evidence:
Immediate observable action:
Owner:
Deadline or activation trigger:
Completion evidence:
Reassess when:
Incoming opportunities and classification:
User confirmation of consequential reprioritization:
```

## O-Record — Opportunity or bridge review

```text
ID: O-0001
Opportunity and verified source/date:
Decision deadline:
Immediate stability contribution:
Strategic alignment:
Capabilities/mastery developed:
Proof, credibility, access, relationships, or distribution gained:
Reciprocity, compensation, and risk distribution:
Costs: [time/money/energy/geography/opportunity]
Essential constraints:
Unknowns requiring research:
Reversibility and exit conditions:
What it makes possible next:
Classification: [replace / activate / queue / observe / park / decline]
Career status: [pursue / investigate / build toward / archive]
Recommendation and reasons:
User decision:
Reassessment trigger:
```

## R-Record — Research brief

```text
ID: R-0001
Question:
Decision affected:
Current knowledge and uncertainty:
Required source standard:
Privacy constraints:
Stopping condition:
Sources and publication/access dates:
Verified findings:
Source claims not independently verified:
Reasoned inference:
Contradictory evidence:
Unresolved unknowns:
Decision impact:
Recommended next move:
```

## D-Record — Decision

```text
ID: D-0001
Decision:
Date and decision owner:
Controlling objective:
Criteria:
Viable options:
Evidence and assumptions:
Tradeoffs and opportunity cost:
Recommendation:
User choice:
Immediate next action:
Completion evidence:
Reopening conditions:
Related records:
```

## X-Record — Experiment

```text
ID: X-0001
Hypothesis:
Decision this informs:
Bounded action:
Owner:
Time/cost limit:
Expected signal:
Stop condition:
Observed result:
Learning:
Next decision:
```

## V-Record — Review and next horizon

```text
ID: V-0001
Period or milestone reviewed:
Expected result:
Activity completed:
External signals:
Outcome and evidence:
Supported explanations:
Alternative explanations:
Conditional projection if unchanged:
Capabilities/resources consolidated:
User's current intention:
Adaptation:
Next state: [celebrate / recover / maintain / prepare / activate next objective]
Next review trigger:
```

## H-Record — Execution handoff

```text
ID: H-0001
Approved action and strategic purpose:
Owner:
Intended recipient or system:
Deadline and timezone:
Dependencies:
Minimal approved context:
Excluded private context:
Completion evidence:
Follow-up/review trigger:
Status: [proposed / approved / prepared / sent / acknowledged / completed / verified]
Evidence for status change:
```

## Record index

```text
Latest verified update:
Current user/scope identifier:
Journal entries:
Reflection hypotheses:
Endorsed insights:
Capabilities:
Goals/milestones:
Focus Cards:
Opportunities:
Research briefs:
Decisions:
Experiments:
Reviews:
Handoffs:
Configured automations:
Retired/deleted records and dependency actions:
```

