# RBAC & Access Control Standard

**Domain:** `QMS` &nbsp; **Document ID Pattern:** `QMS-[PROJECT]-RBAC-STD-[DATE]-01`

> Defines RBAC principles (Least Privilege, Separation of Duties), role hierarchy, role definitions with permission levels, full permission matrix, and access provisioning/deprovisioning SLAs.

---

## Document Control

| Field | Value |
|---|---|
| Document ID | `QMS-[PROJECT]-RBAC-STD-[DATE]-01` |
| Domain | QMS |
| Version | 1.0 |
| Status | DRAFT |
| Author | [Name, Role] |
| Reviewed By | [Name, Role] — [YYYY-MM-DD] |
| Approved By | [Name, Role] — [YYYY-MM-DD] |
| Effective Date | [YYYY-MM-DD] |
| Next Review Date | [YYYY-MM-DD] |
| Project | [PROJECT] |
| Applies To | All roles. Enforced by Head of Security. |
| Feeds Into | GRC-SEC, DATA-DICT, QMS-API-STD |
| Key Placeholders | [PROJECT], [Role definitions], [Permission descriptions], [Provisioning SLAs] |

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


## Roles

| Role | Code | Level |
|---|---|---|
| Super Administrator | SUPER_ADMIN | L5 |
| System Administrator | SYS_ADMIN | L4 |
| HR Administrator | HR_ADMIN | L3 |
| Payroll Manager | PAYROLL_MGR | L3 |
| Manager | MANAGER | L2 |
| Employee Self-Service | ESS_USER | L1 |
| Read-Only Auditor | AUDITOR | L2 |
| Service Account | SERVICE_ACCT | L3 |


## Permission Matrix

● = Full access  ◐ = Read-only  ✎ = Own records only  — = No access

Full matrix in the `.docx` template covering: Employee Records, Salary/Payroll, Leave, Performance, Audit Logs, User Management, System Config, SPII Fields.


---

*Part of the [Universal Project Document Base](../README.md) — replace all `[BRACKETED]` placeholders before use.*
