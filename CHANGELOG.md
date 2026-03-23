# Changelog

All notable changes to the Universal Project Document Base are documented here.

This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html) and the [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) format.

---

## [2.1.0] - 2026-03-24

### Added

**Development (04-DEV)**

- `T31` — Development History & Complete Audit Log: A unified, append-only development audit trail covering 9 typed log sections (§4 Release & Deployment Log, §5 Code Merge Log, §6 Incident Log, §7 Architectural Decision Log, §8 Configuration & Infrastructure Log, §9 Security & Dependency Log, §10 Release Summary Dashboard). Governed by the append-only rule: entries are never modified — only AMENDMENT entries added.

**Meta & Guidance (00-META)**

- `META-GLOBAL-TRACE-01` — Traceability Report: A two-part report proving complete artefact coverage. Includes a dashboard (§2–3) for coverage by folder (11 domains, 33 governed outputs, 139 source artefacts traced), mapping pattern breakdown (Direct / Merged / Elevated / Absorbed / Split), and a 7-row gap coverage proof table. Features a full matrix (§4) tracing one row per source artefact across all 10 domains with mapping rationale notes and a verified 5-check orphan confirmation (zero unowned artefacts, zero empty templates, all gaps closed).

## [2.0.0] - 2026-03-24

### Added

**Data Governance (09-DATA-GOVERNANCE)**

- `T19` — Data Governance Framework (policies, ownership, stewardship, DQ)
- `T20` — Data Dictionary & Classification Register (field-level: PII/SPII/Internal/Public)
- `T21` — Data Retention & Disposal Policy

**Naming Conventions (10-NAMING-CONVENTIONS)**

- `T22` — Master Naming & Code Convention Standard (DB tables/columns, APIs, code, files, branches, environments)
- `T23` — Database Schema & Object Naming Standard
- `T24` — API Design & Versioning Standard

**Quality Management System (08-QMS)**

- `T25` — RBAC & Access Control Standard
- `T26` — Change Management & Configuration Control Standard

**Governance, Risk & Compliance (07-GRC)**

- `T27` — Privacy Impact Assessment (PIA / DPIA)
- `T28` — Vendor & Third-Party Risk Assessment

**Development (04-DEV)**

- `T29` — Development & Coding Standards
- `T30` — CI/CD & Deployment Standard

### Changed

- Expanded the repository structure to include `09-DATA-GOVERNANCE/` and `10-NAMING-CONVENTIONS/`.
- Implemented Dual Format support: Built all 12 new `.docx` templates, generated all 32 `.md` mirrors (T01–T30 + META docs), and assembled the dual folder tree.
- Created updated `.zip` release archive.

### Repository Structure Updated

```text
00-META/  01-PM/  02-BA/  03-ARCH/  04-DEV/
05-QA/    06-QC/  07-GRC/ 08-QMS/   09-DATA-GOVERNANCE/
10-NAMING-CONVENTIONS/              99-ARCHIVE/
```

---

## [1.0.0] - 2026-03-22

### Added — Phase 1: Framework Constitution

- `META-GLOBAL-FRAMEWORK-01.docx` — Universal Document Framework Constitution
  - Document ID taxonomy: `[DOMAIN]-[PROJECT]-[TAG]-[YYYYMMDD]-[SEQ]`
  - 12 domain codes, 45+ document type tags
  - ISO 14-field control block standard
  - Document lifecycle (DRAFT → UNDER REVIEW → APPROVED → SUPERSEDED → RETIRED)
  - Authority model and RACI matrix
  - Repository structure specification
  - Anti-pattern catalogue (8 correct examples, 8 incorrect examples)

### Added — Phase 2: Template Library (18 templates)

**Project Management (PM)**

- `T01_PM-PROJECT-CHARTER.docx` — Project Charter
- `T02_PM-STATUS-REPORT.docx` — Project Status Report
- `T03_PM-CLOSURE-REPORT.docx` — Project Closure Report

**Business Analysis (BA)**

- `T04_BA-SRS.docx` — Software Requirements Specification (FR/NFR/BR/UI requirements)
- `T05_BA-UAC.docx` — User Acceptance Criteria (Given/When/Then, P1/P2/P3 priority)
- `T06_BA-SYSRS.docx` — System Requirements Specification (hardware, performance, DR)

**Architecture & Design (ARCH / ADR)**

- `T07_ARCH-HLD.docx` — High-Level Design Document
- `T08_ADR-ARCHITECTURE-DECISION-RECORD.docx` — Architecture Decision Record

**Governance, Risk & Compliance (GRC)**

- `T09_GRC-SECURITY-COMPENDIUM.docx` — Security Governance Compendium
- `T10_GRC-COMPLIANCE-MATRIX.docx` — Compliance & Standards Alignment Matrix

**Quality Management System (QMS)**

- `T11_QMS-STANDARD-GUIDELINE.docx` — QMS Standard / Guideline

**Quality Assurance (QA)**

- `T12_QA-MASTER-TEST-PLAN.docx` — Master Test Plan
- `T13_QA-PLAN.docx` — Quality Assurance Plan
- `T14_QA-RISK-REGISTER.docx` — Risk Analysis Register

**Quality Control (QC)**

- `T15_QC-QUALITY-CONTROL-REPORT.docx` — Quality Control Report (Go/No-Go)
- `T16_QC-DEFECT-BUG-REPORT.docx` — Defect / Bug Report
- `T17_QC-TEST-CYCLE-REPORT.docx` — Test Cycle Report
- `T18_QC-RELEASE-READINESS-REPORT.docx` — Release Readiness Report

### Added — Phase 3: Index & Repo Infrastructure

- `META-GLOBAL-INDEX-01.docx` — Universal DocBase Master Index
  - Full detail registry for all 19 DocBase documents
  - Inter-document dependency chains (4 chains)
  - Full cross-reference matrix (12 × 12)
  - 10-step project onboarding guide
  - Minimum viable DocSet by project type
  - DocBase governance and maintenance rules
  - Quick Finder: 18 scenarios mapped to templates

- `README.md` — GitHub repository cover document
- `STANDARDS.docx` — Working document authoring standard
- `CHANGELOG.md` — This file
- `LICENSE.txt` — MIT License
- `.github/CONTRIBUTING.md` — Contribution guide
- `.github/pull_request_template.md` — PR template

### Repository Structure Established

```
00-META/  01-PM/  02-BA/  03-ARCH/  04-DEV/
05-QA/    06-QC/  07-GRC/ 08-QMS/   99-ARCHIVE/
```

---

## [Unreleased]

> Planned additions for future release:
>
> - GitHub Actions workflow for template linting
> - Automated placeholder validation script
