# Database Schema & Object Naming Standard

**Domain:** `QMS` &nbsp; **Document ID Pattern:** `QMS-[PROJECT]-DB-NAMING-STD-[DATE]-01`

> Exhaustive database naming rules for: tables, columns, constraints, indexes, views, functions, stored procedures, triggers, migration files, and schema namespaces.

---

## Document Control

| Field | Value |
|---|---|
| Document ID | `QMS-[PROJECT]-DB-NAMING-STD-[DATE]-01` |
| Domain | QMS |
| Version | 1.0 |
| Status | DRAFT |
| Author | [Name, Role] |
| Reviewed By | [Name, Role] — [YYYY-MM-DD] |
| Approved By | [Name, Role] — [YYYY-MM-DD] |
| Effective Date | [YYYY-MM-DD] |
| Next Review Date | [YYYY-MM-DD] |
| Project | [PROJECT] |
| Applies To | All engineers writing migrations, DBA Lead, ORM modellers |
| Feeds Into | QMS-NAMING-STD, DATA-DICT, ARCH-HLD |
| Key Placeholders | [PROJECT], [Schema names], [Domain-specific tables] |

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


## Key Rules

- All names: `snake_case` (no exceptions)
- Tables: plural nouns (`employees`, not `employee`)
- PKs always named `id` (UUID preferred)
- FKs: `[referenced_table_singular]_id`
- Booleans: `is_`, `has_`, `can_` prefix
- Timestamps: `_at` suffix (TIMESTAMPTZ), `_date` suffix (DATE)
- All tables must have: `id`, `created_at`, `updated_at`


## Constraint Naming

`pk_[table]`, `fk_[table]_[ref]`, `uq_[table]_[cols]`, `ix_[table]_[cols]`, `uix_[table]_[cols]`, `ck_[table]_[desc]`


## View & Proc Naming

Views: `v_`, Materialised: `mv_`, Functions: `fn_`, Procedures: `sp_`, Triggers: `trg_[table]_[event]`


## Schema Namespaces

`hr`, `payroll`, `auth`, `audit`, `ref`, `[domain]` — avoid `public`


---

*Part of the [Universal Project Document Base](../README.md) — replace all `[BRACKETED]` placeholders before use.*
