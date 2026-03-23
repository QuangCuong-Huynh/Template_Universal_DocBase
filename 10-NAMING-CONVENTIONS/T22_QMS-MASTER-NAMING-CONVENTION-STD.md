# Master Naming & Code Convention Standard

**Domain:** `QMS` &nbsp; **Document ID Pattern:** `QMS-[PROJECT]-NAMING-STD-[DATE]-01`

> Comprehensive naming standards for: variables, functions, classes, files, branches, commits (Conventional Commits), environments, services, containers, and cloud resources.

---

## Document Control

| Field | Value |
|---|---|
| Document ID | `QMS-[PROJECT]-NAMING-STD-[DATE]-01` |
| Domain | QMS |
| Version | 1.0 |
| Status | DRAFT |
| Author | [Name, Role] |
| Reviewed By | [Name, Role] — [YYYY-MM-DD] |
| Approved By | [Name, Role] — [YYYY-MM-DD] |
| Effective Date | [YYYY-MM-DD] |
| Next Review Date | [YYYY-MM-DD] |
| Project | [PROJECT] |
| Applies To | All Development, DevOps, Database, and QA team members |
| Feeds Into | QMS-DB-NAMING-STD, QMS-API-STD, ARCH-HLD |
| Key Placeholders | [PROJECT], [Language-specific rules], [Tool names], [Cloud platform], [Ticket prefix] |

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


## Casing Reference

| Style | Used For |
|---|---|
| `PascalCase` | Classes, interfaces, React components |
| `camelCase` | Variables, functions, object properties |
| `SCREAMING_SNAKE_CASE` | Constants, environment variables |
| `kebab-case` | URL paths, CSS classes, file names (frontend) |
| `snake_case` | Database tables, columns, PostgreSQL objects |
| `dot.case` | Config keys, namespace identifiers |


## Branch Naming

`feat/[ticket]-[description]`, `fix/[ticket]-[description]`, `hotfix/[ticket]-[description]`, `release/v[N].[N].[N]`, `docs/[description]`


## Commit Convention

Follows [Conventional Commits](https://conventionalcommits.org):
```
feat(auth): add MFA support
fix(payroll): correct rounding error
docs(api): update v2 endpoint docs
BREAKING CHANGE: ...
```


---

*Part of the [Universal Project Document Base](../README.md) — replace all `[BRACKETED]` placeholders before use.*
