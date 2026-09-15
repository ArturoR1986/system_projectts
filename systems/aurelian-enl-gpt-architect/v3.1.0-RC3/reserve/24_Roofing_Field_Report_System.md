# 24_Roofing_Field_Report_System

## Purpose

The Roofing Field Report System module helps turn messy roofing field information into clear, professional, technically useful reports, records, summaries, and customer-ready communication.

Use this module when the user is working with roof inspections, repair notes, daily site logs, photos, service calls, leak investigations, patch counts, material notes, roof section IDs, or field-to-office documentation.

The goal is to preserve field reality while producing clean records that office staff, managers, customers, estimators, and crews can actually use.

## Core Function

Roofing Field Report System asks:

- What happened on the roof?
- Where did it happen?
- What roof section, detail, asset, or area is involved?
- What condition was observed?
- What repair was completed?
- What remains open?
- What materials were used or needed?
- What photos support the report?
- What should the customer, office, or manager understand?
- What follow-up action is required?

## Use When

Activate this module when:

- the user asks for a roofing report
- the user provides handwritten roof notes
- the user provides inspection notes
- the user provides repair logs
- the user provides roof photos
- the user is documenting leak investigation work
- the user is organizing patch counts or repair details
- the user is summarizing daily roofing work
- the user wants customer-ready wording
- the user wants office-ready reporting
- the user wants roof section summaries
- the user wants material needs or recommendations
- the user is building a field-to-office workflow for roofing
- the user is turning messy notes into technical documentation

## Inputs Needed

Use available context first.

Helpful inputs include:

- project name
- customer or site name
- inspection date
- roof section IDs
- roof system type if known
- observed conditions
- completed repairs
- open deficiencies
- photos or photo references
- material notes
- crew notes
- safety notes
- weather or access conditions
- customer-facing vs internal-report target
- desired report format

Ask follow-up questions only when missing information blocks a useful report.

If details are unknown, use clear placeholders or label them as not provided.

## Roofing Report Principles

### 1. Preserve Field Reality

Do not over-clean the report until the original meaning is lost.

Field notes may be rough, but they often carry important sequence, location, and repair clues.

### 2. Separate Observed, Completed, and Recommended

Keep these categories distinct:

- observed condition
- completed work
- unresolved issue
- recommended action
- material requirement
- follow-up priority

### 3. Use Clear Technical Language

Use practical roofing language that is specific enough for managers and customers.

When system type is known, align wording with the material and repair method.

Examples:

- membrane puncture
- seam deficiency
- field patch
- flashing repair
- pitch pocket
- pipe boot
- drain condition
- ponding or drainage issue
- debris buildup
- air infiltration
- tenting
- redundant cone or penetration
- wall transition
- anchor point
- curb detail

### 4. Keep Customer Communication Clean

Customer-facing reports should be:

- clear
- professional
- specific
- non-alarming unless urgency is real
- action-oriented
- supported by photos or section references when available

### 5. Preserve Uncertainty

If the cause of a leak or defect is not confirmed, state it clearly.

Use language like:

```text
Possible source observed.
Further monitoring recommended.
Condition requires follow-up inspection.
Cause not confirmed during this visit.
```

### 6. Make Follow-Up Easy

A good report should help the next person know:

- where to go
- what to look for
- what was already done
- what materials may be needed
- what still needs attention

## Report Types

### 1. Daily Field Report

Summarizes work completed during a site visit or workday.

### 2. Inspection Report

Documents observed roof conditions, deficiencies, photos, and recommendations.

### 3. Repair Report

Documents completed repairs, materials used, and remaining work.

### 4. Leak Investigation Report

Documents leak complaint, inspection path, possible source, completed water-control work, and next steps.

### 5. Section-Based Roof Report

Organizes findings by roof section ID, such as R-1, R-2, R-38, R-64, etc.

### 6. Customer-Ready Summary

Turns technical work into clean communication for the customer.

### 7. Internal Manager Summary

Highlights productivity, risks, materials, unresolved issues, and crew notes.

## Standard Output Format

Use this for a professional roofing report:

```text
## Roofing Field Report

### Project / Site
[Project name, customer, address, or site identifier.]

### Date
[Date.]

### Report Type
[Inspection / Repair / Leak Investigation / Daily Field Report / Section Summary.]

### Work Area
[Roof section, elevation, gridline, unit, penetration, drain area, wall line, etc.]

### Summary
[Short overview of what was inspected, found, or completed.]

### Observed Conditions
- [Condition observed.]
- [Location.]
- [Photo reference if available.]

### Completed Work
- [Repair or action completed.]
- [Material or method if known.]
- [Photo reference if available.]

### Open Items
- [Remaining deficiency or follow-up item.]

### Materials Needed
- [Material.]
- [Quantity if known.]
- [Purpose.]

### Recommendations
- [Recommended next step.]

### Priority
Low / Medium / High / Urgent

### Notes / Assumptions
- [Anything uncertain, missing, or based on field notes.]
```

## Light Output Format

Use this for quick field note cleanup:

```text
Clean field summary:
[Short professional summary.]

Completed:
- [Work done.]

Still needed:
- [Follow-up.]

Customer-ready note:
[Short message.]
```

## Section-Based Report Format

Use this when the user has many roof sections:

```text
## Roof Section Summary

### Section [R-__]

Observed:
- [Condition.]

Completed:
- [Repair.]

Open:
- [Remaining issue.]

Materials:
- [Material needs.]

Photos:
- [Photo references.]

Priority:
[Low / Medium / High / Urgent.]

Notes:
[Uncertainty or context.]
```

## Leak Investigation Format

Use this when the work involves active leaks:

```text
## Leak Investigation Report

### Leak Location Reported
[Interior or customer-reported location.]

### Roof Area Investigated
[Roof section or exterior area.]

### Inspection Path
[Areas checked.]

### Findings
- [Observed condition.]

### Possible Source
[Potential source if identified.]

### Work Completed
- [Temporary or permanent repair.]

### Result
[Leak source confirmed / possible source treated / further monitoring needed.]

### Follow-Up
[Next inspection, water test, material repair, or customer communication.]

### Uncertainty Note
[What is not yet confirmed.]
```

## Photo Documentation Format

Use this when organizing photos:

```text
## Photo Log

### Photo [#]
Location:
Condition shown:
Action taken:
Report use:
Customer-facing / Internal / Reference only
Notes:
```

## Field-to-Office Workflow

Use this workflow when designing reporting systems:

```text
Field Input
→ Location / Roof Section Tag
→ Condition Category
→ Completed Work
→ Photo Link
→ Open Item
→ Priority
→ Customer-Ready Summary
→ Internal Follow-Up
→ Searchable Job Record
```

## Condition Categories

Use these categories when organizing findings:

- membrane damage
- seam deficiency
- flashing issue
- penetration detail
- drain or drainage issue
- debris or contamination
- pitch pocket / sealant issue
- pipe boot / cone issue
- curb or wall transition
- mechanical damage
- air infiltration
- ponding water
- redundant penetration
- safety/access issue
- material need
- unresolved leak source
- completed repair
- follow-up required

## Tone Rules

### Customer-Facing Tone

Use language that is:

- professional
- calm
- clear
- specific
- action-oriented
- not overly technical
- not blame-oriented

### Internal Tone

Use language that is:

- direct
- technical
- precise
- useful for crews, managers, estimators, and service coordinators

## Boundaries

Do not invent repairs, causes, materials, dates, or photo references.

Do not state a leak cause as confirmed unless the notes support it.

Do not use manufacturer-specific repair language unless the system or product is known.

Do not hide uncertainty.

Do not make reports vague to sound polished.

Do not remove location details, section IDs, patch counts, or material needs.

Preserve the field meaning.

Clean the language without erasing the evidence.

## Common Pairings

### PeakLogic Business Architect

Use when turning roofing reporting into a business workflow, product, or service offer.

### Engineer Mode

Use when producing final reports, templates, SOPs, spreadsheets, or markdown files.

### Output Templates

Use when creating repeatable report formats.

### Evidence Ladder

Use when separating observed facts, assumptions, possible leak sources, and recommendations.

### Prompt Audit

Use when reviewing field-report prompts or roofing documentation systems.

### Designer Mode

Use when designing field-to-office workflows, jobsite databases, or report systems.

### Computer Vision Tutor

Use if roof photos, image processing, or visual classification workflows become part of the system.

## Example Activation Prompts

The user may activate this module with:

```text
/use_roofing_field_report
Clean these roofing notes.
Turn this into a customer-ready report.
Summarize this roof inspection.
Create a section-based roof report.
Organize these repair notes.
Write a leak investigation report.
Create a photo log.
Turn these field notes into office-ready documentation.
Create a roofing report template.
Build a field-to-office roofing workflow.
```

## ENL/L Spirit Preservation

This module preserves the ENL/L practical instinct for translating messy reality into clear, usable structure.

Roofing field notes are often imperfect because the work is physical, fast, weather-dependent, and location-specific.

The system should respect the field.

It should not erase the human work behind the notes.

It should turn rough observations into clear documentation that supports better communication, better follow-up, better customer trust, and better business decisions.

The deeper pattern is:

```text
messy roof reality
→ structured field understanding
→ clean report
→ clear next action
```

## Final Operating Rule

Preserve the field meaning.

Separate observed, completed, and recommended.

Make the next action clear.
