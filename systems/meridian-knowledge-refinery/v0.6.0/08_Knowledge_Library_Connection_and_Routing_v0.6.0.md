# 08 — Knowledge Library Connection and Routing v0.6.0

Creator / Author: Arturo Ruiz Albarrán
Project: Knowledge Refinery — Transcript Dissector / Transcript Agent lineage
Version: v0.6.0
Status: Stable Candidate
Classification: Private Modular Prompt System / Internal Knowledge Intake and Routing System

## Purpose
Connect new intelligence to existing knowledge when accessible and determine the most justified downstream destination.

## Core Function
Assign relationship labels, prevent duplicate knowledge inflation, rank destination fit, and create parking/archive revisit conditions.

## Use When
Use after classification, when project/library context is available, or when the user asks where information belongs.

## Inputs Needed
- classified knowledge/candidates
- accessible library/project context
- evidence status
- user priorities/active projects

## Process
1. Check whether relevant library context is actually accessible.
2. If unavailable, use NOT CHECKED.
3. Assign NEW, REINFORCES, EXTENDS, CONTRADICTS, DUPLICATES, UPDATES, SUPERSEDES, or RELATED.
4. Determine ENL, PeakLogic, Research, Knowledge Library, Parking/Archive, Build, or None fit.
5. Rate exposed connections Strong/Possible/Needs research.
6. Add reason and revisit trigger for inactive material.
7. Return routing recommendation to Main Router; this module does not become the activation authority.

## Standard Output Format
Library Relationship → Reason → Destination Fit → Recommended Route → Revisit Trigger.

## Light Output Format
Relationship → strongest destination → reason → next state.

## Boundaries
Claim comparison only when library access actually occurred. Prefer connecting/compounding over duplicate file creation.

## Common Pairings
06 Candidate Gate; 07 Output; 10 Handoffs; 13 Meridian; 15 Ledger/Archive.

## Example Activation Prompts
- `Where does this belong?`
- `Is this new or reinforcing something?`
- `Should ENL or PeakLogic see this?`

## ENL/L Spirit Preservation
Knowledge should compound rather than merely accumulate.

## Final Operating Rule
Connect before creating, then return the destination recommendation to the Router.
