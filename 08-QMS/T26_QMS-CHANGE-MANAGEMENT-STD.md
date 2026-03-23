# Change Management & Configuration Control Standard

**Domain:** `QMS` &nbsp; **Document ID Pattern:** `QMS-[PROJECT]-CHANGE-MGT-STD-[DATE]-01`

> Classifies changes (Standard/Normal/Emergency/Rejected), defines Change Request mandatory fields, Change Advisory Board (CAB) structure and cadence, and configuration management rules.

---

## Document Control

| Field | Value |
|---|---|
| Document ID | `QMS-[PROJECT]-CHANGE-MGT-STD-[DATE]-01` |
| Domain | QMS |
| Version | 1.0 |
| Status | DRAFT |
| Author | [Name, Role] |
| Reviewed By | [Name, Role] — [YYYY-MM-DD] |
| Approved By | [Name, Role] — [YYYY-MM-DD] |
| Effective Date | [YYYY-MM-DD] |
| Next Review Date | [YYYY-MM-DD] |
| Project | [PROJECT] |
| Applies To | All teams making changes to production systems |
| Feeds Into | DEV-CICD-STD, QC-SUMMARY, GRC-SEC |
| Key Placeholders | [PROJECT], [CAB members], [Notice periods], [Change freeze dates], [Approval quorum] |

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


## Change Types

| Type | Approval | Window |
|---|---|---|
| Standard | Pre-approved procedure | Anytime |
| Normal | CAB approval, [N] days notice | Maintenance window |
| Emergency | Head of Engineering (sync) | Immediate + post-review |
| Rejected | CAB rejection with reason | Not implemented |


## CR Required Fields

CR ID, Title, Change Type, Requestor, Affected Systems, Change Description, Business Justification, Risk Assessment, **Rollback Plan** (mandatory + tested), Test Evidence, Implementation Steps, Verification Steps, Maintenance Window, CAB Approval.


---

*Part of the [Universal Project Document Base](../README.md) — replace all `[BRACKETED]` placeholders before use.*
