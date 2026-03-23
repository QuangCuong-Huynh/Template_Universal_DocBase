# Contributing to the Universal Project Document Base

Thank you for contributing. This guide explains how to add, improve, or fix templates in the DocBase.

---

## Ground Rules

1. **Every template must conform to `META-GLOBAL-FRAMEWORK-01.docx`** — the Framework Constitution governs ID taxonomy, control blocks, lifecycle, and structure. Read it before contributing.
2. **No content in master templates** — templates must use `[BRACKETED]` placeholders throughout. Never include project-specific content in the master library.
3. **One PR per template** — keep contributions focused. A PR adding T19 should not also modify T07.
4. **Update the Index** — any new template addition must be accompanied by an update to `00-META/META-GLOBAL-INDEX-01.docx` registering the new document.
5. **Update CHANGELOG.md** — all changes must be documented under `[Unreleased]`.

---

## Branch Naming

| Change Type | Branch Format | Example |
|---|---|---|
| New template | `feat/template-[domain]-[name]` | `feat/template-dev-deployment-plan` |
| Template fix | `fix/[template-id]-[short-description]` | `fix/T07-missing-security-section` |
| Documentation | `docs/[what]` | `docs/readme-update-quickstart` |
| Governance update | `governance/[what]` | `governance/framework-tag-dictionary` |

---

## Adding a New Template

Follow these steps:

1. **Copy the closest existing template** as a structural starting point.
2. **Assign a new template number** (next sequential: T19, T20, …).
3. **Assign a Document ID pattern** using the Framework taxonomy.
4. **Replace all content with `[BRACKETED]` placeholders** — no real content.
5. **Ensure the control block** contains all 12+ ISO fields per `META-GLOBAL-FRAMEWORK-01.docx` §4.
6. **Place the file** in the correct domain folder (`01-PM/`, `02-BA/`, etc.).
7. **Register it** in `00-META/META-GLOBAL-INDEX-01.docx` Sections 4 and 5.
8. **Add it to `README.md`** in the correct domain table.
9. **Document it in `CHANGELOG.md`** under `[Unreleased]`.
10. **Open a pull request** using the PR template.

---

## Fixing an Existing Template

1. Open the `.docx` file in Microsoft Word.
2. Make the targeted fix — structural corrections, missing sections, control block updates.
3. Do **not** change the Document ID pattern or the cover page layout without discussion.
4. Document the fix in `CHANGELOG.md` under `[Unreleased]`.
5. Open a pull request.

---

## Pull Request Review Criteria

PRs will be reviewed against:

- [ ] Template conforms to `META-GLOBAL-FRAMEWORK-01.docx`
- [ ] All content sections use `[BRACKETED]` placeholders
- [ ] ISO control block contains all mandatory fields
- [ ] Cover page format matches existing templates
- [ ] File placed in correct domain folder
- [ ] File named `T[NN]_[DOMAIN]-[DESCRIPTION].docx`
- [ ] Index updated (if new template)
- [ ] README updated (if new template)
- [ ] CHANGELOG.md updated

---

## Questions

Open a GitHub Discussion or Issue before starting significant work. This prevents duplicate effort and ensures alignment with the DocBase governance model.
