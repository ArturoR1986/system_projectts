# SKILL-IP-001 — IP Registration and Provenance

Version: 1.0-RC1
Status: Candidate Skill
Owner: Asset Sovereignty and IP Governance

## Purpose

Stamp a finished or release-candidate asset with clear ownership/provenance metadata and prepare its registry record.

## Trigger

Use when an owned asset reaches:
- stable candidate;
- handoff;
- release;
- archive;
- GitHub/Codex preparation;
- client review;
- publication preparation.

## Inputs

- asset title;
- asset type;
- owner/author;
- version;
- date;
- classification;
- status;
- repository/project;
- storage location;
- license/rights if applicable;
- commit/timestamp if available;
- related assets.

Use placeholders for non-blocking missing metadata.

## Procedure

1. Identify the asset.
2. Confirm ownership is appropriate.
3. Assign/confirm Asset ID.
4. Apply ownership/provenance notice.
5. Create registry entry.
6. Create provenance note.
7. Record storage recommendation.
8. Flag whether Sovereignty release review is still required.

## Output

```text
Asset:
Asset ID:
Owner:
Version:
Date:
Classification:
Status:
Rights / License:
Storage:
Commit / Timestamp:
Related Assets:
Ownership / Provenance Notice:
Registry Entry:
Release Review Required:
```

## Boundaries

- This skill does not decide whether an asset should be released.
- This skill does not provide legal advice.
- This skill does not claim ownership of work the user does not own.
- If ownership is unclear, stop and flag review.
- Governance classification controls public exposure.

## Failure Behavior

Stop or return `NEEDS REVIEW` when:
- ownership is unclear;
- asset identity is ambiguous;
- classification conflicts with intended release;
- required provenance cannot be established.

## Human Authority

Human approval remains required for consequential release, licensing, publication, or disclosure decisions.

## Tests

Pass when:
- metadata is complete or honestly marked;
- ownership notice matches classification;
- release decision is not fabricated;
- provenance record is reusable;
- skill remains bounded to registration rather than full governance.

## Final Operating Rule

Register the asset clearly; leave the release decision to governance.
