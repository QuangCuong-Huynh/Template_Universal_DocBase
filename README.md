# Universal Project Document Base

**A complete, standards-aligned library of professional project document templates for software development teams.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE.txt)
[![Templates](https://img.shields.io/badge/Templates-18-blue.svg)]()
[![Standard](https://img.shields.io/badge/Standard-ISO%2027001%20%7C%20ISO%209001%20%7C%20OWASP%20ASVS-green.svg)]()
[![Version](https://img.shields.io/badge/Version-1.0.0-brightgreen.svg)](CHANGELOG.md)

---

## What Is This?

The **Universal Project Document Base** (Universal DocBase) is a structured library of 20 production-ready `.docx` templates covering every stage of a software project lifecycle — from project kick-off through architecture, requirements, quality assurance, security governance, and formal release.

Every template is:

- **Project-neutral** — uses `[PROJECT]` placeholders. One template, any project.
- **ISO-conformant** — every document carries a 14-field ISO control block with versioning, ownership, and review dates.
- **Fully traceable** — a structured Document ID taxonomy (`[DOMAIN]-[PROJECT]-[TAG]-[YYYYMMDD]-[SEQ]`) ensures nothing is unnamed or untracked.
- **Audit-ready** — together, the templates constitute a complete evidence package for ISO 27001, ISO 9001, GDPR, and OWASP ASVS assessments.

---

## Repository Structure

```
universal-docbase/
│
├── 00-META/                          # Governance layer
│   ├── META-GLOBAL-FRAMEWORK-01.docx   Framework Constitution (ID taxonomy, lifecycle, authority)
│   └── META-GLOBAL-INDEX-01.docx       Master Registry & Adaptation Guide (this library's index)
│
├── 01-PM/                            # Project Management
│   ├── T01_PM-PROJECT-CHARTER.docx
│   ├── T02_PM-STATUS-REPORT.docx
│   └── T03_PM-CLOSURE-REPORT.docx
│
├── 02-BA/                            # Business Analysis
│   ├── T04_BA-SRS.docx                 Software Requirements Specification
│   ├── T05_BA-UAC.docx                 User Acceptance Criteria
│   └── T06_BA-SYSRS.docx               System Requirements Specification
│
├── 03-ARCH/                          # Architecture & Design
│   ├── T07_ARCH-HLD.docx               High-Level Design Document
│   └── T08_ADR-ARCHITECTURE-DECISION-RECORD.docx
│
├── 04-DEV/                           # Development (extend here)
│
├── 05-QA/                            # Quality Assurance
│   ├── T12_QA-MASTER-TEST-PLAN.docx
│   ├── T13_QA-PLAN.docx
│   └── T14_QA-RISK-REGISTER.docx
│
├── 06-QC/                            # Quality Control
│   ├── T15_QC-QUALITY-CONTROL-REPORT.docx
│   ├── T16_QC-DEFECT-BUG-REPORT.docx
│   ├── T17_QC-TEST-CYCLE-REPORT.docx
│   └── T18_QC-RELEASE-READINESS-REPORT.docx
│
├── 07-GRC/                           # Governance, Risk & Compliance
│   ├── T09_GRC-SECURITY-COMPENDIUM.docx
│   └── T10_GRC-COMPLIANCE-MATRIX.docx
│
├── 08-QMS/                           # Quality Management System
│   └── T11_QMS-STANDARD-GUIDELINE.docx
│
├── 99-ARCHIVE/                       # Retired & superseded versions
│
├── .github/
│   ├── CONTRIBUTING.md
│   └── pull_request_template.md
│
├── README.md                         ← You are here
├── STANDARDS.docx                    Working document authoring standard
├── CHANGELOG.md
└── LICENSE.txt
```

---

## Quick Start — Onboarding a New Project

> Full step-by-step guide is in `00-META/META-GLOBAL-INDEX-01.docx` §7.

**5-minute version:**

```
1. Agree a project code  →  e.g., ORBIT, HRMS, PAYROLL  (2–8 uppercase chars)
2. Copy required templates to your project folder
3. Find & Replace  [PROJECT]  →  your project code  (Ctrl+H in Word)
4. Find & Replace  [PROJECT NAME]  →  your full project name
5. Assign real Document IDs  →  e.g., QA-ORBIT-MTP-20260301-01
6. Fill in [BRACKETED] content placeholders
7. Route for review → approval → sign-off
```

**Minimum Viable DocSet by project size:**

| Project Type | Required Templates |
|---|---|
| Small feature / sprint | T01, T04, T05, T12, T15, T16 |
| Medium project (< 6 months) | T01–T06, T07, T12–T18 |
| Large / enterprise | All 18 templates |
| Compliance / regulated | All 18 + T09, T10 mandatory |
| Architecture spike / POC | T08 (ADR), T07 (HLD) |

---

## Template Library

### Governance (META)

| ID | File | Purpose |
|---|---|---|
| META-GLOBAL-FRAMEWORK-01 | `00-META/META-GLOBAL-FRAMEWORK-01.docx` | ID taxonomy, ISO control standard, document lifecycle, authority model |
| META-GLOBAL-INDEX-01 | `00-META/META-GLOBAL-INDEX-01.docx` | Master registry, dependency map, onboarding guide, governance rules |

### Project Management (PM)

| # | ID Pattern | File | Purpose |
|---|---|---|---|
| T01 | `PM-[PROJECT]-CHARTER` | `01-PM/T01_PM-PROJECT-CHARTER.docx` | Formally authorizes the project. Scope, stakeholders, budget, milestones. |
| T02 | `PM-[PROJECT]-STATUS-RPT` | `01-PM/T02_PM-STATUS-REPORT.docx` | Periodic executive status: schedule, budget, risk, milestones. |
| T03 | `PM-[PROJECT]-CLOSURE` | `01-PM/T03_PM-CLOSURE-REPORT.docx` | Formal project closure: objectives, deliverables acceptance, lessons learned. |

### Business Analysis (BA)

| # | ID Pattern | File | Purpose |
|---|---|---|---|
| T04 | `BA-[PROJECT]-SRS` | `02-BA/T04_BA-SRS.docx` | Functional (FR) and non-functional (NFR) requirements. The dev–business contract. |
| T05 | `BA-[PROJECT]-UAC` | `02-BA/T05_BA-UAC.docx` | Given/When/Then acceptance criteria. UAT sign-off gateway. |
| T06 | `BA-[PROJECT]-SYSRS` | `02-BA/T06_BA-SYSRS.docx` | Hardware, software, performance, capacity, security, DR specifications. |

### Architecture & Design (ARCH / ADR)

| # | ID Pattern | File | Purpose |
|---|---|---|---|
| T07 | `ARCH-[PROJECT]-HLD` | `03-ARCH/T07_ARCH-HLD.docx` | Architecture pattern, components, data design, security zones, deployment. |
| T08 | `ADR-[PROJECT]-[TOPIC]` | `03-ARCH/T08_ADR-ARCHITECTURE-DECISION-RECORD.docx` | Single architectural decision: context, options, rationale, consequences. |

### Governance, Risk & Compliance (GRC)

| # | ID Pattern | File | Purpose |
|---|---|---|---|
| T09 | `GRC-[PROJECT]-SEC` | `07-GRC/T09_GRC-SECURITY-COMPENDIUM.docx` | Security principles, IAM, data classification, incident response, compliance. |
| T10 | `QA-[PROJECT]-COMP-MTX` | `07-GRC/T10_GRC-COMPLIANCE-MATRIX.docx` | Maps each clause of ISO 27001 / GDPR / OWASP / ISO 9001 to project controls. |

### Quality Management System (QMS)

| # | ID Pattern | File | Purpose |
|---|---|---|---|
| T11 | `QMS-[PROJECT]-STD` | `08-QMS/T11_QMS-STANDARD-GUIDELINE.docx` | Universal template for any organizational standard (RBAC, naming, coding). |

### Quality Assurance (QA)

| # | ID Pattern | File | Purpose |
|---|---|---|---|
| T12 | `QA-[PROJECT]-MTP` | `05-QA/T12_QA-MASTER-TEST-PLAN.docx` | Test levels, scope, environment, defect severity, release criteria, schedule. |
| T13 | `QA-[PROJECT]-PLAN` | `05-QA/T13_QA-PLAN.docx` | Strategic QA vision, shift-left approach, quality objectives, metrics. |
| T14 | `QA-[PROJECT]-RISK` | `05-QA/T14_QA-RISK-REGISTER.docx` | Living risk register. Likelihood × Impact matrix, mitigations, closed risks. |

### Quality Control (QC)

| # | ID Pattern | File | Purpose |
|---|---|---|---|
| T15 | `QC-[PROJECT]-QCREPORT` | `06-QC/T15_QC-QUALITY-CONTROL-REPORT.docx` | Formal Go/No-Go release recommendation with QA Director sign-off. |
| T16 | `QC-[PROJECT]-BUG` | `06-QC/T16_QC-DEFECT-BUG-REPORT.docx` | Individual defect record: steps to reproduce, root cause, fix, verification. |
| T17 | `QC-[PROJECT]-CYCLE-RPT` | `06-QC/T17_QC-TEST-CYCLE-REPORT.docx` | Sprint/phase test execution results, defects, blockers, exit criteria. |
| T18 | `QC-[PROJECT]-SUMMARY` | `06-QC/T18_QC-RELEASE-READINESS-REPORT.docx` | 11-gate pre-release checklist with formal multi-party release authorization. |

---

## Document ID Schema

```
[DOMAIN]-[PROJECT]-[TAG]-[YYYYMMDD]-[SEQ]

Example:  QA-ORBIT-MTP-20260301-01
          │   │     │    │        └─ Sequence (01, 02 …)
          │   │     │    └────────── Creation date (ISO 8601)
          │   │     └─────────────── Document type tag
          │   └───────────────────── Project code (2–8 chars)
          └───────────────────────── Domain code
```

**Domain codes:** `PM` · `BA` · `ARCH` · `ADR` · `DEV` · `QA` · `QC` · `QMS` · `GRC` · `META`

Full ID taxonomy and tag dictionary: `00-META/META-GLOBAL-FRAMEWORK-01.docx` §3.

---

## Standards & Compliance Alignment

This library is designed to support evidence collection for:

| Standard | Relevant Templates |
|---|---|
| **ISO 27001:2022** | T09, T10, T11, T14 |
| **ISO 9001:2015** | T12, T13, T10, T11 |
| **OWASP ASVS L2** | T09, T10, T12 |
| **GDPR (EU 2016/679)** | T09, T10 |
| **NIST CSF 2.0** | T09, T14 |
| **NIST RMF SP 800-37** | T14, T09 |

---

## Inter-Document Dependencies

Key document chains (→ = "feeds into"):

```
Requirements chain:
  PM-CHARTER → BA-SRS → BA-UAC → QA-MTP → QC-CYCLE-RPT → QC-QCREPORT → QC-SUMMARY

Architecture chain:
  BA-SRS / BA-SYSRS → ADR (per decision) → ARCH-HLD → Implementation → QA-MTP

Governance chain:
  META-FRAMEWORK → GRC-SEC → QMS-STD → QA-COMP-MTX → QA-RISK → QC-QCREPORT
```

Full cross-reference matrix: `00-META/META-GLOBAL-INDEX-01.docx` §6.

---

## Authoring Standards

See `STANDARDS.docx` for the complete working document authoring standard covering:
- How to use the templates
- Placeholder replacement rules
- ID assignment procedure
- Document lifecycle and status definitions
- Approval workflow
- Version control rules

---

## Contributing

See [`.github/CONTRIBUTING.md`](.github/CONTRIBUTING.md) for the full contribution guide.

**Quick summary:**
1. Fork the repository
2. Create a branch: `feat/template-[domain]-[name]` or `fix/[template-id]-[issue]`
3. Follow the authoring standard in `STANDARDS.docx`
4. New templates must conform to `META-GLOBAL-FRAMEWORK-01.docx`
5. Update `00-META/META-GLOBAL-INDEX-01.docx` to register the new template
6. Open a pull request using the PR template

---

## Changelog

See [CHANGELOG.md](CHANGELOG.md) for full release history.

**Latest:** [v1.0.0](CHANGELOG.md) — Initial release. 20 documents across 8 domains.

---

## License

This project is licensed under the **MIT License** — see [LICENSE.txt](LICENSE.txt) for details.

You are free to use, copy, modify, and distribute these templates for any purpose, including commercial projects, provided the copyright notice and license text are retained.

---

## Acknowledgements

Built to align with: ISO/IEC 27001:2022 · ISO 9001:2015 · OWASP ASVS 5.0 · NIST CSF 2.0 · NIST SP 800-37 · NIST SP 800-61 · GDPR (EU 2016/679) · ISTQB Foundation Level · ISO/IEC 25010.
