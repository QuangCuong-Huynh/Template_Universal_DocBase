# Changelog

All notable changes to the Universal Project Document Base are documented here.

This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html) and the [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) format.

---

## [1.0.0] — 2026-03-22

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

> Planned additions for v1.1.0:
> - `T19` — DEV: Deployment Plan (`DEV-[PROJECT]-DEPLOY-PLAN`)
> - `T20` — DEV: Release Notes (`DEV-[PROJECT]-RELEASE-NOTES`)
> - `T21` — DEV: API Specification (`ARCH-[PROJECT]-API-SPEC`)
> - `T22` — DATA: Data Dictionary (`DATA-[PROJECT]-DICT`)
> - GitHub Actions workflow for template linting
> - Automated placeholder validation script
