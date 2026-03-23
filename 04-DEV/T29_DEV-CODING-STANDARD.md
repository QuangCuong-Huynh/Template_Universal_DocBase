# Development & Coding Standard

**Domain:** `DEV` &nbsp; **Document ID Pattern:** `DEV-[PROJECT]-CODING-STD-[DATE]-01`

> Code quality rules (SRP, error handling, no dead code), security coding rules (input validation, parameterized queries, no secrets in code), testing requirements (AAA pattern, coverage), code review standards, and dependency management.

---

## Document Control

| Field | Value |
|---|---|
| Document ID | `DEV-[PROJECT]-CODING-STD-[DATE]-01` |
| Domain | DEV |
| Version | 1.0 |
| Status | DRAFT |
| Author | [Name, Role] |
| Reviewed By | [Name, Role] — [YYYY-MM-DD] |
| Approved By | [Name, Role] — [YYYY-MM-DD] |
| Effective Date | [YYYY-MM-DD] |
| Next Review Date | [YYYY-MM-DD] |
| Project | [PROJECT] |
| Applies To | All engineers writing production code for [PROJECT] |
| Feeds Into | QMS-NAMING-STD, DEV-CICD-STD, GRC-SEC |
| Key Placeholders | [PROJECT], [Coverage targets], [Logger library], [Validation library], [Review SLAs], [Dependency approval process] |

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

**General:** SRP, no dead code, max function length [N] lines, no magic numbers, handle all errors, no console.log in production.

**Security:** Validate all user input, parameterized queries only, no secrets in code, auth at middleware level, no PII in logs.

**Testing:** Unit tests required, AAA pattern, one behaviour per test, no external dependencies in unit tests, no real PII in test data.

**Review:** [N] required approvals, `[BLOCK]` vs `[NIT]` comment taxonomy, no self-merge.


---

*Part of the [Universal Project Document Base](../README.md) — replace all `[BRACKETED]` placeholders before use.*
