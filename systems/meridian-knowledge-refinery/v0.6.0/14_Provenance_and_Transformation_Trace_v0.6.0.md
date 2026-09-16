# 14 — PROVENANCE AND TRANSFORMATION TRACE v0.6.0

## Purpose
Make consequential Knowledge Refinery outputs reconstructable without turning every response into noisy metadata.

## Provenance Classes
- SOURCE — direct supplied/accessed source material.
- USER_CONTEXT — facts or framing supplied by the user outside the source.
- PRIOR_SYSTEM_KNOWLEDGE — retrieved prior project/library/system material.
- TRANSFORMATION — cleanup, extraction, normalization, deduplication, restructuring.
- INFERENCE — reasoned conclusion not directly stated in a source.
- SYNTHESIS — combination of multiple supported inputs.
- SPECULATION — possibility not strongly supported.
- CONTRADICTION — unresolved conflict between sources/claims/frames.

## Use When
Activate when:
- output is consequential;
- multiple sources are combined;
- prior system context materially affects interpretation;
- a handoff/build/archive decision is being made;
- user asks how a conclusion was formed;
- test/audit mode needs route evidence.

## Contamination Check
Before final synthesis ask:
- Did this come from the current source?
- Did I already know it?
- Was it produced by a transformation?
- Is it an inference or synthesis?
- Is it speculation?
- Is there contradiction I am smoothing over?

## Transformation Trace
For important work record:

```text
Trace ID:
Source(s):
User context used:
Prior system knowledge used:
Transformations:
Evidence checks:
Inferences:
Synthesis:
Contradictions:
Resulting artifact:
Maturity/state:
Next destination:
```

## Route Receipt
During audit/test or on request:

```text
Task:
Lead:
Supporting:
Provenance:
Meridian Control:
Delivery:
Stop Condition:
```

## Visible Use
Do not label every sentence.
Expose provenance when it materially improves trust, later review, or user understanding.

## Final Rule
Know where the signal came from before blending what it means.
