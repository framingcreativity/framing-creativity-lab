# Remediation Register — FCL-DOC-AUDIT-2026-001

**Document ID:** FCL-AUD-REG-001  
**Version:** 1.0  
**Status:** Open — baseline actions not yet evidenced as complete  
**Source:** `02-AUDIT-REPORT.md`  
**Baseline commit:** `e026bdc5cc4a78dd80570f8c93d50008711de262`

> This register translates audit findings into trackable work. A recommendation is not a completed correction. Change a status only after the relevant repository state or configuration has been verified and record the commit or evidence reference.

## 1. Status vocabulary

- **Open:** no verified corrective action recorded.
- **In progress:** work has started; completion is not verified.
- **Blocked — decision:** requires an explicit maintainer decision.
- **Blocked — configuration:** requires a repository setting or operational channel to be checked or configured.
- **Resolved:** the corrected file or configuration has been inspected and verified.
- **Accepted risk:** the maintainer has explicitly accepted and documented the remaining risk.
- **Not applicable:** scope has materially changed; provide rationale.

## 2. Findings register

| Finding | Severity | Affected area | Corrective action | Dependency / decision | Initial status |
|---|---|---|---|---|---|
| AUD-001 | High | `QUALITY-STANDARDS.md.`; `RESPONSIBLE-AI.md.`; internal references | Rename to exact `.md` paths, update references, and validate links on the target platform. | Repository write access; verify exact final paths. | Open |
| AUD-002 | High | README, Charter, Governance, Lifecycle, Quality, Template | Make `PROJECT-LIFECYCLE.md` authoritative for stages and statuses; separate stage, status, maturity, publication state, and production readiness. | Maintainer approval of canonical vocabulary. | Blocked — decision |
| AUD-003 | High | README, Contributing, Publication Policy | Define the permission/licence terms for external contributions before accepting or merging external IP. Preserve the intentional absence of a general repository licence unless a separate decision changes it. | Explicit licensing and contribution-rights decision; potentially legal review. | Blocked — decision |
| AUD-004 | Medium | Security, Code of Conduct, Contributing | Verify GitHub Private Vulnerability Reporting; establish and publish an actual private conduct-reporting route. Do not invent contact details or describe unconfigured routes as operational. | GitHub setting access and a real reporting channel. | Blocked — configuration |
| AUD-005 | Medium | README and cross-document references | Add a linked documentation index and clickable relative links between related policies. | Correct filenames and confirmed folder structure. | Open |
| AUD-006 | Medium | Publication Policy, Responsible AI, Project Template | Adopt a shared data classification taxonomy and consistently represent personal-data status. | Maintainer approval of taxonomy. | Blocked — decision |
| AUD-007 | Medium | Publication Policy, Project Template | Clarify P1 public-release conditions; require formal reclassification and renewed review before any P2/P3 reconsideration. | Publication-policy decision. | Blocked — decision |
| AUD-008 | Medium | Quality Standards, Project Template, README | Separate technical maturity/evidence, publication status, and production readiness into distinct fields. | Canonical terminology from AUD-002. | Blocked — decision |
| AUD-009 | Medium | README, Charter, Governance, Contributing, Security, Quality, Research, AI, Lifecycle, Template | Reduce duplicated procedures; retain detailed requirements in their designated authoritative documents and cross-link summaries. | Document ownership map; can be phased. | Open |
| AUD-010 | Low | Metadata across policy/template documents | Standardize metadata field names and status conventions while preserving meaningful historical dates. | Metadata convention decision. | Open |
| AUD-011 | Low | Project Template | Retain the comprehensive master template and prepare a shorter public project brief; keep restricted assessment details outside public project records. | Confirm user need and publication model. | Open |

## 3. Phase plan

### Phase 1 — Publication blockers and operational gates

- AUD-001 — exact filenames and references.
- AUD-002 — lifecycle/status taxonomy.
- AUD-003 — contribution permissions and licence terms.
- AUD-004 — operational private reporting channels.

### Phase 2 — Coherence and usability

- AUD-005 — navigation and cross-links.
- AUD-006 — data classification.
- AUD-007 — publication classifications.
- AUD-008 — maturity/readiness dimensions.
- AUD-009 — duplicate policy content.
- AUD-010 — metadata conventions.
- AUD-011 — project template usability.

### Phase 3 — Future operational improvements

The source report suggests decision/publication records, specialist research templates, automated Markdown/link and filename validation, and proportionate security scanning as the Lab's work expands. These are future improvements, not baseline defects requiring immediate implementation.

## 4. Evidence log

| Date | Finding | Action / evidence | Commit or configuration reference | Verified by | Status |
|---|---|---|---|---|---|
| 2026-11-25 | Baseline audit | Audit report generated against the baseline commit. | `e026bdc5cc4a78dd80570f8c93d50008711de262` | Audit record | Baseline |

Add a row for every material change. For status “Resolved”, include enough detail for another reviewer to reproduce the verification.

## 5. Completion rule

The audit is not closed merely because files have been edited. Close a finding only after a read-only validation confirms that the intended change exists, references resolve, no contradictory terminology remains in the in-scope documents, and no private or proprietary content was introduced.
