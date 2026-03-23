# Document Authoring Standard

**Document ID:** `QMS-GLOBAL-AUTHORING-STD-01` &nbsp; **Version:** 1.0

> The complete working document authoring standard for the Universal Project DocBase. See `STANDARDS.docx` in `docx-working/` for the fully formatted version.

---

## 1. The Document ID System

```
[DOMAIN]-[PROJECT]-[TAG]-[YYYYMMDD]-[SEQ]

Example:  QA-ORBIT-MTP-20260301-01
```

| Field | Format | Rules |
|---|---|---|
| DOMAIN | 2–5 uppercase | PM, BA, ARCH, ADR, DEV, QA, QC, QMS, GRC, META |
| PROJECT | 2–8 uppercase | Set in Charter. Used on ALL documents. |
| TAG | Uppercase hyphenated | From Framework tag dictionary. Do not invent. |
| YYYYMMDD | ISO 8601 | Creation date — never update on revision. |
| SEQ | NN | Two digits, starts at 01. |

### ID Anti-Patterns

| ❌ Non-Conforming | ✓ Correct |
|---|---|
| `TestPlan_v2_FINAL.docx` | `QA-ORBIT-MTP-20260301-01` |
| `qa-orbit-mtp-20260301-01` | `QA-ORBIT-MTP-20260301-01` (must be uppercase) |
| `QA-ORBIT-MTP-01/03/2026-01` | `QA-ORBIT-MTP-20260301-01` (ISO 8601 only) |
| `QA-ORBIT-MASTERTEST-20260301-01` | `QA-ORBIT-MTP-20260301-01` (approved tags only) |

---

## 2. How to Use a Template

1. **Copy** the template from the DocBase — never edit the master
2. **Rename** to real Document ID: `QA-ORBIT-MTP-20260301-01.docx`
3. **Find & Replace** `[PROJECT]` → your project code
4. **Find & Replace** `[PROJECT NAME]` → your full project name
5. **Set Document ID** in the control block to match the filename
6. **Set all dates** — replace all `[YYYY-MM-DD]` placeholders
7. **Set Author/Approver** — replace all `[Name, Role]` placeholders
8. **Fill body content** — resolve all `[BRACKETED]` placeholders
9. **Run Quality Checklist** (Section 5 of STANDARDS.docx)
10. **Route for approval** → Reviewer → Approver → APPROVED status

---

## 3. Pre-Approval Quality Checklist

### Document Identity
- [ ] ID conforms to `[DOMAIN]-[PROJECT]-[TAG]-[YYYYMMDD]-[SEQ]`
- [ ] Filename matches Document ID in control block
- [ ] All 12+ ISO control block fields populated
- [ ] Status set correctly (DRAFT / UNDER REVIEW / APPROVED)
- [ ] Author, Reviewed By, Approved By contain real names

### Content Quality
- [ ] Zero `[BRACKETED]` placeholders remain
- [ ] All tables fully populated — no empty template rows
- [ ] All cross-references use real Document IDs (not patterns)
- [ ] All dates in ISO 8601 format (YYYY-MM-DD)
- [ ] All numeric thresholds specified (no `[X%]` or `[Amount]`)

### Sign-Off
- [ ] Approval Signatures table has real names
- [ ] Correct Approver for this domain signed (see §6.3)
- [ ] File saved as `.docx` and named with full Document ID
- [ ] File placed in correct domain folder

---

## 4. Document Lifecycle

| Status | Definition | Required to Advance |
|---|---|---|
| DRAFT | Being authored. Not authoritative. | Complete content + run checklist |
| UNDER REVIEW | Submitted for peer review. | Reviewer sign-off, comments resolved |
| APPROVED | All signatures obtained. Authoritative. | Populate Effective Date, store in repo |
| SUPERSEDED | Newer APPROVED version exists. | Move to `/99-ARCHIVE/` |
| RETIRED | No longer applicable. | Move to `/99-ARCHIVE/`, notify teams |

**Versioning:** `1.0` initial → `1.1` minor update → `2.0` major revision

---

## 5. Approval Authority by Domain

| Domain | Templates | Approver |
|---|---|---|
| PM | T01–T03 | Product Owner / Sponsor |
| BA | T04–T06 | Product Owner |
| ARCH/ADR | T07–T08 | Chief Architect |
| GRC | T09–T10, T27–T28 | Head of Security / CISO |
| QMS | T11, T25–T26 | QA Director |
| QA | T12–T14 | QA Director |
| QC | T15–T18 | QA Director |
| DATA | T19–T21 | Privacy Officer / DPO |
| NAMING | T22–T24 | Chief Architect |
| DEV | T29–T30 | Head of Engineering |
| META | Framework, Index | QA Director |

---

## 6. Testability Rule

Every requirement must be independently verifiable.

| ❌ Not Testable | ✓ Testable |
|---|---|
| "The system shall be fast." | "API responses ≤ 500ms at P95 under 200 concurrent users." |
| "The UI shall be user-friendly." | "SUS score ≥ 80 in usability test with 5 representative users." |
| "The system shall be secure." | "Zero Critical/High findings in OWASP ASVS Level 2 assessment." |

---

## 7. Cross-Reference Rules

Always reference other documents by their full Document ID — never by title alone.

| ❌ Incorrect | ✓ Correct |
|---|---|
| See the Master Test Plan. | See `QA-ORBIT-MTP-20260301-01` (Master Test Plan). |
| Per the SRS. | Per `BA-ORBIT-SRS-20260201-01` FR-AUTH-002. |

---

*See `STANDARDS.docx` in `docx-working/` for the complete formatted version with all rule tables.*
