---
schema_version: 1
id: "rca-636229"
document_type: "root_cause_analysis"
title: "Ticket 636229 - Reported visibility of non-sales conversations in Neosapien Mobile App"
version: "1.0"
created_date: "2026-09-18"
review_date: "2026-09-11"
created_by: "Mageswari K"
approved_by: "Soumyo Dey"
ticket:
  system: "ServiceHub"
  id: "636229"
priority: "Low"
product: "Neosapien Mobile App"
components:
  - "Sales-memory display filter"
  - "Sales-only visibility controls"
region: "West Zone"
incident:
  first_occurrence_date: "2026-09-08"
  start_date: "2026-09-08"
  resolution_date: "2026-09-11"
  resolution_time: "12:33"
  timezone: null
  repeat_problem: false
  caused_by_change: false
problem_record:
  number: "1"
  created_date: "2026-09-08"
  assigned_team: "Neosapien Support / Engineering"
  assigned_to: "Mohammed Khalid"
  assigned_role: "L1 agent"
rca:
  completed_date: "2026-09-11"
  completed_by: "Sundharesan"
  completed_by_role: "L3 agent"
reported_by:
  name: "Roshan Mishra"
  role: "Regional Coordinator, West Zone"
affected_user:
  name: "Rajendra Yadav"
  role: "DSR"
  id: "73292"
tags:
  - "non-sales-conversations"
  - "conversation-visibility"
  - "sales-filter"
  - "classifier-hardening"
sources:
  primary_file: "RCA - Ticket 636229.docx"
  equivalent_file: "RCA - Ticket 636229.pdf"
markdown_created_date: "2026-09-22"
markdown_updated_date: "2026-09-22"
---

# Root Cause Analysis

## Ticket 636229 — Reported visibility of non-sales conversations in Neosapien Mobile App

The DSR reported temporary visibility of non-sales conversations in the Neosapien app. The classifier needed to be hardened to ensure non-sales conversations do not appear in the sales flow. The enhancement was completed and communicated on 11 September 2026.

## Document control

| Field | Details |
| --- | --- |
| Version | 1.0 |
| Created date | 18 September 2026 |
| Review date | 11 September 2026 |
| Created by | Mageswari K |
| Approved by | Soumyo Dey |

## Reported problem

| Field | Details |
| --- | --- |
| Problem | Reported temporary visibility of non-sales conversations in Neosapien |
| ServiceHub ticket | 636229 |
| Reported by | Roshan Mishra, Regional Coordinator, West Zone |
| Date and time of first occurrence | 8 September 2026; time not recorded |
| Problem recognition source | The DSR reported the issue through the Regional Coordinator |

## Problem record

| Field | Details |
| --- | --- |
| Problem record number | 1 |
| Assigned team | Neosapien Support / Engineering |
| Assigned to | Mohammed Khalid, L1 agent |
| RCA completed by | Sundharesan, L3 agent |
| Related incident number | 636229 |
| Incident start | 8 September 2026; time not recorded |
| Incident resolution | 11 September 2026, 12:33 |
| Incident priority | Low |
| Problem record created | 8 September 2026; time not recorded |
| RCA completed date | 11 September 2026 |
| Repeat problem | No |
| Caused by a change | No |
| Change number | No, as recorded in the source |

## Impact

### Technical impact

Non-sales conversations were temporarily visible in the Neosapien app.

### Business impact

- **Affected user:** Rajendra Yadav, DSR 73292.
- **Affected processes and functions:** Non-sales conversations were showing up with sales conversations. The classifier needs to be hardened to prevent non-sales conversations from being displayed.

## RCA executive summary

The classifier needed to be hardened to ensure non-sales conversations do not appear in the sales flow.

The enhancement was completed and communicated on 11 September 2026.

| Field | Details |
| --- | --- |
| RCA duration | Updates: 9–11 September 2026 |
| Related incident | 636229 |
| Vendor ticket | Not recorded |
| Capacity-related issue | No capacity issue reported |
| Event trigger | User reported |

### Incident summary

- **Symptoms:** The DSR reported that personal conversations appeared temporarily in the app.
- **Location:** West Zone.
- **System / CI:** Neosapien app and sales-memory display filter.
- **Users impacted:** Rajendra Yadav, DSR 73292. Wider impact not quantified.
- **Investigation outcome:** The sales-only visibility controls were reviewed and hardened to ensure that only eligible sales conversations are surfaced.

## Event monitoring information

| Field | Details |
| --- | --- |
| Was any alert triggered in monitoring? | Not recorded |
| Date and time of alert | Not recorded |
| Was the alert acknowledged? | Not recorded |
| Alert acknowledgement ticket | Not recorded |
| If no alert was triggered, can it be configured? | This needs to be reported by the user |

## Incident timeline

Times use the 24-hour clock. The source does not specify a timezone.

| Date | Time | Event | Details |
| --- | --- | --- | --- |
| 2026-09-09 | 13:39 | Received | We acknowledged the issue and began our investigation. |
| 2026-09-09 | 15:23 | Initial closure | We could not reach the DSR. Roshan shared the TSE contact details. We contacted the TSE, who confirmed the resolution, and communicated ticket closure. |
| 2026-09-10 | 12:01 | Follow-up | G M Gurunathan informed us that non-sales memories were visible despite the filter and disappeared by the next day. |
| 2026-09-10 | 12:38 | RCA ongoing | We informed them that the RCA was ongoing and that an update would be shared once completed. |
| 2026-09-11 | 12:33 | Update shared | We communicated the investigation outcome and the hardening of the sales-only visibility controls. |
| 2026-09-11 | 14:55 | Forwarded | G M Gurunathan forwarded the update to Roshan Mishra. |

## Root cause analysis

**Problem statement:** The DSR reported that non-sales conversations appeared alongside sales conversations in the Neosapien app.

### Why 1 — Why did we investigate?

The DSR reported temporary visibility of non-sales conversations, prompting a review of the reported behaviour.

### Why 2 — What control governs this visibility?

The Neosapien app uses sales-only visibility controls to determine which conversations are surfaced.

### Why 3 — What was identified during the review?

The visibility controls and associated filtering logic were reviewed to ensure that only eligible sales conversations surfaced.

### Why 4 — What corrective action was taken?

The sales-only visibility controls were hardened to provide an additional layer of protection against unintended visibility.

### Why 5 — How can we improve future investigation?

Enhanced diagnostic logging and a screenshot of the affected memory, if the behaviour recurs, will support further investigation.

## Corrective and preventive actions

### Corrective actions

| No. | Action | Owner | Status | Related follow-up | Target completion date |
| --- | --- | --- | --- | --- | --- |
| 1 | Reviewed and hardened the controls to ensure that only eligible sales conversations surfaced in the application. | Neosapien Engineering | Closed | Ticket 636229 | 2026-09-11 |
| 2 | We contacted the TSE regarding the reported behaviour and communicated the investigation update. | Mohammed Khalid, L1 agent | Closed | TSE follow-up 9 September; update shared 11 September | 2026-09-11 |

### Preventive actions

| No. | Action | Owner | Status | Related follow-up | Target completion date |
| --- | --- | --- | --- | --- | --- |
| 1 | Capture a screenshot if the issue occurs again. | Support; reporting user | Ongoing on recurrence | Instruction issued in ticket 636229 | As needed |
| 2 | We performed regression checks across application views and improved logging. | Engineering / QA | Closed | Regression checks completed | 2026-09-11 |

## Lessons learned

| No. | Lesson learned | KEDB updated |
| --- | --- | --- |
| 1 | Maintain consistent sales-only visibility controls across all app views as part of ongoing quality assurance. | Yes |
| 2 | Capture supporting screenshots promptly when a concern is reported to support timely validation and investigation. | Yes |
| 3 | Include sales-only visibility scenarios in regression validation for relevant application changes. | Yes |
