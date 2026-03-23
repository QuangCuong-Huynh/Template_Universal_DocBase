# Universal DocBase Master Index

**Domain:** `META` &nbsp; **Document ID Pattern:** `META-GLOBAL-INDEX-01`

> Master registry of all 32 documents in the Universal DocBase. Contains inter-document dependency chains, cross-reference matrix, 10-step project onboarding guide, minimum viable DocSet by project type, and DocBase governance rules.

---

## Document Control

| Field | Value |
|---|---|
| Document ID | `META-GLOBAL-INDEX-01` |
| Domain | META |
| Version | 1.0 |
| Status | DRAFT |
| Author | [Name, Role] |
| Reviewed By | [Name, Role] — [YYYY-MM-DD] |
| Approved By | [Name, Role] — [YYYY-MM-DD] |
| Effective Date | [YYYY-MM-DD] |
| Next Review Date | [YYYY-MM-DD] |
| Project | [PROJECT] |
| Applies To | All project teams, QA Director, Chief Architect, Compliance Officer |
| Feeds Into | All 32 DocBase documents |

---

## Revision History

| Version | Date | Author | Summary |
|---|---|---|---|
| 1.0 | [YYYY-MM-DD] | [Name, Role] | Initial approved version |

---

## Approval Signatures

| Role | Full Name | Signature Ref | Date |
|---|---|---|---|
| [Approver Role] | [Full Name] | [SIG-XXXXXX] | [YYYY-MM-DD] |

---


## Quick Finder

| I need to… | Use this template |
|---|---|
| Start a project | T01 — PM-CHARTER |
| Document requirements | T04 — BA-SRS |
| Define acceptance criteria | T05 — BA-UAC |
| Design the architecture | T07 — ARCH-HLD |
| Record an architectural decision | T08 — ADR |
| Establish security governance | T09 — GRC-SEC |
| Govern data | T19 — DATA-GOV-FWK |
| Define naming conventions | T22 — QMS-NAMING-STD |
| Assess vendor risk | T28 — GRC-VENDOR-RISK |
| Plan testing | T12 — QA-MTP |
| Issue Go/No-Go | T15 — QC-QCREPORT |
| Authorize a release | T18 — QC-SUMMARY |


## Dependency Chains

```
Requirements:  PM-CHARTER → BA-SRS → BA-UAC → BA-SYSRS → ARCH-HLD → QA-MTP → QC-CYCLE-RPT → QC-QCREPORT → QC-SUMMARY
Governance:    META-FRAMEWORK → GRC-SEC → QMS-STD → QA-COMP-MTX → QA-RISK → QC-QCREPORT
Data:          DATA-GOV-FWK → DATA-DICT → DATA-RETENTION → GRC-DPIA
Dev:           NAMING-STD + DB-NAMING + API-STD → CODING-STD → CICD-STD → CHANGE-MGT
```


---

*Part of the [Universal Project Document Base](../README.md) — replace all `[BRACKETED]` placeholders before use.*
