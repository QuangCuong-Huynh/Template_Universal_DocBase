# Data Dictionary & Classification Register

**Domain:** `DATA` &nbsp; **Document ID Pattern:** `DATA-[PROJECT]-DICT-[DATE]-01`

> Field-level registry of all Confidential/PII/SPII data. Records: entity, field name, type, classification, encryption requirements, masking in non-prod, retention period, and GDPR legal basis.

---

## Document Control

| Field | Value |
|---|---|
| Document ID | `DATA-[PROJECT]-DICT-[DATE]-01` |
| Domain | DATA |
| Version | 1.0 |
| Status | DRAFT |
| Author | [Name, Role] |
| Reviewed By | [Name, Role] — [YYYY-MM-DD] |
| Approved By | [Name, Role] — [YYYY-MM-DD] |
| Effective Date | [YYYY-MM-DD] |
| Next Review Date | [YYYY-MM-DD] |
| Project | [PROJECT] |
| Applies To | Development Team, DBA, Security Team, Compliance, Data Stewards |
| Feeds Into | DATA-GOV-FWK, GRC-SEC, GRC-DPIA |
| Key Placeholders | [PROJECT], [Entity names], [Field names], [Data types], [Classification tiers], [Retention periods], [Legal bases] |

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


## Contents

1. Document Control
2. How to Use (12-column field register definition)
3. Entity & Field Classification Register (one section per entity/table)
4. PII/SPII Field Summary (consolidated audit table)

**Column schema per field:** Field ID, Entity/Table, Field Name, Data Type, Classification, Description, Data Owner, Encryption Required, Masking in Non-Prod, Retention Period, Legal Basis, Nullable


---

*Part of the [Universal Project Document Base](../README.md) — replace all `[BRACKETED]` placeholders before use.*
