# Care rules and data exchanges

## From a report to follow-up

A clinician reviews a synthetic result and approves the plan version. The patient sees the approved instructions and accepts that version. Each reminder points back to its source. A corrected lab may make an earlier explanation stale. A verified stopped order cancels the affected future reminders while preserving history.

| Noor’s fictional example | Time in Asia/Dubai |
| --- | --- |
| Reported first dose | 09:20 |
| Check-in becomes due | 09:50 |
| Patient records the first dose | 10:00 |
| Next dose in the approved 12-hour interval | 21:20 |

The plan explicitly permits the first-dose anchor. At 10:00 the app shows the check-in already due. It makes no claim that a notification was delivered at 09:50. Fixed clock times stay on the clock schedule. Ambiguous frequencies go back for clarification.

## Records and checks

- A source event identifies the patient, source, event, version, issuer and effective and recording times. Exact retries reuse the event ID. Wrong-patient events are rejected and conflicting records go to review.
- A care task identifies its approved plan, timing and evidence. A patient report stores the reported occurrence separately from when it was recorded.
- A clinician signs off on closure after reviewing the outcome. A message delivery receipt or attendance record is one piece of evidence.

## Internal interfaces

| Interface | What it supports |
| --- | --- |
| `/healthz` | Service and feature status |
| `/v1/communication` | Synthetic invitations, endpoint pairing, encrypted envelopes, inbox, delivery receipts and consented deadline routing |
| `/v1/ai/jobs` | Reviewed text, limited requests and a typed source-linked response |

The intended Abu Dhabi pathway uses authorised clinic record and e-prescription interfaces. FHIR R4 [Timing](https://hl7.org/fhir/R4/datatypes.html#Timing) and [MedicationRequest](https://hl7.org/fhir/R4/medicationrequest.html) inform illustrative mappings. A partner would need to confirm the actual profiles, permissions, matching and update rules. The full PDF contains synthetic lab and prescription examples.

[System architecture](architecture.md) · [Verification](verification.md) · [Documentation home](README.md)
