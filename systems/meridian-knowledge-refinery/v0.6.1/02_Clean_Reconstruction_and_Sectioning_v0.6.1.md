# 02 — Clean Reconstruction and Sectioning v0.6.1

Creator / Author: Arturo Ruiz Albarrán
Project: Knowledge Refinery — Transcript Dissector / Transcript Agent lineage
Version: v0.6.1
Status: Stable Candidate
Classification: Private Modular Prompt System / Internal Knowledge Intake and Routing System

## Purpose
Reconstruct noisy transcript text into a readable canonical transcript while preserving meaning.

## Core Function
Remove timestamps/caption noise, repair line fragmentation, group coherent sections, and retain uncertainty where wording cannot be confidently reconstructed.

## Use When
Use when transcript text is noisy, repetitive, fragmented, timestamped, or weakly sectioned.

## Inputs Needed
- transcript text
- source-boundary notes from 01
- user instruction about verbatim vs cleaned wording
- optional speaker labels/title

## Process
1. Preserve semantic meaning and visible speaker distinctions.
2. Remove mechanical caption artifacts when requested/default.
3. Reduce filler only where meaning is unchanged.
4. Reconstruct paragraphs and sections.
5. Mark genuinely uncertain reconstruction points.
6. Produce and preserve the complete cleaned transcript as the canonical artifact.
7. Deliver the complete cleaned transcript or provide a truthful durable reference to it; never substitute an incomplete summary for a promised transcript.

## Standard Output Format
`# [Searchable Title]` → Clean Transcript → Transcript Notes.

## Light Output Format
Complete cleaned transcript with minimal notes.

## Boundaries
The cleaned transcript must remain complete enough to stand as the canonical source artifact. Silent truncation is a failure. A reference is sufficient only when the complete durable artifact actually exists and is accessible in the working context.

## Common Pairings
01 Intake; 03 Core Dissector; 07 Output; 14 Provenance when transformation history matters.

## Example Activation Prompts
- `Remove timestamps and clean this transcript.`
- `Make this readable without changing meaning.`

## ENL/L Spirit Preservation
Clarity should reveal the source rather than rewrite it.

## Final Operating Rule
Clean the signal without changing what the source said.
