# API Design & Versioning Standard

**Domain:** `QMS` &nbsp; **Document ID Pattern:** `QMS-[PROJECT]-API-STD-[DATE]-01`

> REST API design rules: URL structure, HTTP method usage, status code standards, error response body schema, versioning policy, deprecation process, and security rules.

---

## Document Control

| Field | Value |
|---|---|
| Document ID | `QMS-[PROJECT]-API-STD-[DATE]-01` |
| Domain | QMS |
| Version | 1.0 |
| Status | DRAFT |
| Author | [Name, Role] |
| Reviewed By | [Name, Role] — [YYYY-MM-DD] |
| Approved By | [Name, Role] — [YYYY-MM-DD] |
| Effective Date | [YYYY-MM-DD] |
| Next Review Date | [YYYY-MM-DD] |
| Project | [PROJECT] |
| Applies To | All engineers building or consuming REST APIs in [PROJECT] |
| Feeds Into | QMS-NAMING-STD, ARCH-HLD, BA-SRS |
| Key Placeholders | [PROJECT], [Rate limits], [Version sunset periods], [Auth mechanism] |

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


## URL Rules

- Base path: `/api/v{N}/{resource}`
- Resources: plural nouns in `kebab-case`
- Nesting: `/{parent}/{id}/{child}` (max 3 levels)
- No verbs in paths
- Query params: `camelCase`


## HTTP Methods

`GET` → 200 OK (idempotent, no side effects)
`POST` → 201 Created + Location header
`PUT` → 200 or 204 (full replacement, idempotent)
`PATCH` → 200 or 204 (partial update)
`DELETE` → 204 No Content (idempotent)


## Error Response Schema

```json
{
  "status": 400,
  "code": "VALIDATION_ERROR",
  "message": "Human-readable message",
  "details": [{"field": "email", "message": "Invalid format"}],
  "traceId": "abc-123",
  "timestamp": "2026-03-01T10:00:00Z"
}
```


## Versioning

- Version in URL only: `/api/v1/`, `/api/v2/`
- New version only for breaking changes
- Prior version supported ≥ [N] months after new version
- `Deprecation:` and `Sunset:` headers on deprecated versions


---

*Part of the [Universal Project Document Base](../README.md) — replace all `[BRACKETED]` placeholders before use.*
