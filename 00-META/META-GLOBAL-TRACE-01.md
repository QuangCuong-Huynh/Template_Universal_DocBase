# Artifact-to-DocBase Traceability Report

**Domain:** `META` &nbsp; **Document ID:** `META-GLOBAL-TRACE-01`

> Maps every source project artefact (169+ files across 10 domains) to its governing DocBase template. Proves zero orphaned artefacts, documents all mapping decisions, and traces the 7 governance gaps closed by DocBase v2.0.

---

## Document Control

| Field | Value |
|---|---|
| Document ID | `META-GLOBAL-TRACE-01` |
| Version | 2.0 |
| Total Source Artefacts Traced | 139 |
| Total Target Templates | 31 templates + 2 META docs = 33 governed outputs |
| DocBase Version | Universal DocBase v2.0 |
| Linked Documents | META-GLOBAL-FRAMEWORK-01, META-GLOBAL-INDEX-01, T01–T31 |

---

## Coverage Summary

| Folder | Domain | Templates | Source Artefacts Mapped |
|---|---|---|---|
| 01-PM | PM | T01, T02, T03 | 12 |
| 02-BA | BA | T04, T05, T06 | 11 |
| 03-ARCH | ARCH | T07, T08 | 10 |
| 04-DEV | DEV | T29, T30, T31 | 9 |
| 05-QA | QA | T12, T13, T14 | 11 |
| 06-QC | QC | T15, T16, T17, T18 | 8 |
| 07-GRC | GRC | T09, T10, T27, T28 | 12 |
| 08-QMS | QMS | T11, T25, T26 | 7 |
| 09-DATA-GOVERNANCE | DATA | T19, T20, T21 | 7 |
| 10-NAMING-CONVENTIONS | NAMING | T22, T23, T24 | 5 |
| 00-META | META | Framework, Index | 2 |
| **TOTAL** | **11 domains** | **31 + 2 META** | **139** |

---

## Mapping Patterns

| Pattern | Count | Definition |
|---|---|---|
| Direct | ~55 | 1:1 mapping. Structure preserved and enhanced. |
| Merged | ~35 | N source artefacts → 1 template. Eliminates duplication. |
| Elevated | ~25 | Informal artefact → governed standard/policy. |
| Absorbed | ~20 | Content absorbed into a section of a broader template. |
| Split | ~4 | 1 source → multiple templates where content served different governance purposes. |

---

## Gap Coverage (v2.0 Additions)

| Gap | Governance Gap | Closed By |
|---|---|---|
| GAP-01 | No governed data ownership, classification, or PII register | T19, T20, T21 in `09-DATA-GOVERNANCE/` |
| GAP-02 | No enforced naming conventions across code, DB, API, branches | T22, T23, T24 in `10-NAMING-CONVENTIONS/` |
| GAP-03 | No formal RBAC standard — roles existed only in code/wikis | T25 in `08-QMS/` |
| GAP-04 | No CAB structure or mandatory Change Request fields | T26 in `08-QMS/` |
| GAP-05 | GDPR Art. 35 DPIA not performed | T27 in `07-GRC/` |
| GAP-06 | No vendor due diligence standard for processors accessing PII | T28 in `07-GRC/` |
| GAP-07 | `04-DEV/` empty — no coding standard, CI/CD standard, or dev audit trail | T29, T30, T31 in `04-DEV/` |

---

## Orphan Check

| Check | Result |
|---|---|
| Every source artefact maps to a template | ✅ 139/139 |
| Every template (T01–T31) has source artefacts | ✅ 31/31 |
| Every new folder closes a documented gap | ✅ 7/7 gaps closed |
| No duplicate governance | ✅ 0 conflicts |

> Full matrix with per-artefact mapping notes is in `META-GLOBAL-TRACE-01.docx`

---

*Part of the [Universal Project Document Base](../README.md)*
