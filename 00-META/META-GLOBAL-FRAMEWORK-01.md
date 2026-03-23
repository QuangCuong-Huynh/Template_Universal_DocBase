# Universal Document Framework Constitution

**Domain:** `META` &nbsp; **Document ID Pattern:** `META-GLOBAL-FRAMEWORK-01`

> Defines the Document ID taxonomy, ISO 14-field control standard, document lifecycle, authority model, repository structure, and quick-reference checklists governing all documents in the Universal Project DocBase.

---

## Document Control

| Field | Value |
|---|---|
| Document ID | `META-GLOBAL-FRAMEWORK-01` |
| Domain | META |
| Version | 1.0 |
| Status | DRAFT |
| Author | [Name, Role] |
| Reviewed By | [Name, Role] — [YYYY-MM-DD] |
| Approved By | [Name, Role] — [YYYY-MM-DD] |
| Effective Date | [YYYY-MM-DD] |
| Next Review Date | [YYYY-MM-DD] |
| Project | [PROJECT] |
| Applies To | All Project Teams, QA Director, Chief Architect, Compliance Officer |
| Feeds Into | All documents — this is the root governance document |

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


## Document ID Taxonomy

Full structure: `[DOMAIN]-[PROJECT]-[TAG]-[YYYYMMDD]-[SEQ]`

| Field | Format | Rules |
|---|---|---|
| DOMAIN | 2–5 uppercase chars | Approved codes: PM, BA, ARCH, ADR, DEV, QA, QC, QMS, GRC, META |
| PROJECT | 2–8 uppercase chars | Set in Project Charter. Used on ALL documents. |
| TAG | Uppercase hyphenated | From tag dictionary §3. Do not invent tags. |
| YYYYMMDD | ISO 8601 | Creation date. Never update on revision. |
| SEQ | NN | Two-digit, starts at 01. |


## ISO Control Block (14 Mandatory Fields)

Every document must include: Document ID, Document Title, Version, Status, Classification, Author, Reviewed By, Approved By, Effective Date, Next Review Date, Project, Applies To, Supersedes, Linked Documents.


## Document Lifecycle

`DRAFT` → `UNDER REVIEW` → `APPROVED` → `SUPERSEDED` → `RETIRED`

Retired and superseded documents move to `/99-ARCHIVE/`. Never deleted.


## Authority & RACI

| Domain | Reviewer | Approver |
|---|---|---|
| PM | BA Lead / Head of Eng | Product Owner / Sponsor |
| BA | Chief Architect | Product Owner |
| ARCH/ADR | Head of Engineering | Chief Architect |
| GRC | Chief Architect | Head of Security |
| QMS | Domain Lead | QA Director |
| QA/QC | Project Manager | QA Director |


---

*Part of the [Universal Project Document Base](../README.md) — replace all `[BRACKETED]` placeholders before use.*
