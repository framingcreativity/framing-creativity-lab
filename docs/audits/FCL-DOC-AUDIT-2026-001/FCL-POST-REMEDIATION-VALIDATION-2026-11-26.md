# Framing Creativity Lab — Post-Remediation Validation Report

**Document ID:** FCL-AUD-VALID-002  
**Version:** 1.0  
**Status:** Validation completed — remediation remains open  
**Validation date:** 26 November 2026  
**Repository:** `framingcreativity/framing-creativity-lab`  
**Branch:** `main`  
**Commit inspected:** `b0a71f618cde4b75459b1094f80a30eec5a71543`  
**Commit timestamp:** 26 November 2026, 03:13:26 UTC (11:13:26 Asia/Kuala_Lumpur)  
**Mode:** Read-only  
**Maintainer identified in repository:** J-ART

---

## 1. Executive Summary

### Overall verdict

**NOT READY — the baseline audit has not yet been fully remediated.**

The repository has made two substantive improvements since the baseline: the malformed documentation filenames were corrected, and `PROJECT-LIFECYCLE.md` now explicitly distinguishes Lifecycle Stage from Project Status. The remediation register was also updated to version 1.1 and now records the incomplete state more accurately.

However, the current canonical documents still contain the original taxonomy conflicts, no general documentation index, unresolved contributor-permission terms, unverified private reporting routes, inconsistent data classification, and an unclear P1 publication rule. Several v2.0 replacement documents have been added to the repository as separate draft files rather than replacing the canonical files. Their presence does not resolve the findings.

### Finding status summary

| Status | Count | Findings |
|---|---:|---|
| Resolved | 1 | AUD-001 |
| Partially resolved | 3 | AUD-002, AUD-008, AUD-009 |
| Open | 4 | AUD-005, AUD-006, AUD-010, AUD-011 |
| Blocked | 3 | AUD-003, AUD-004, AUD-007 |
| **Total** | **11** | |

The validation does not establish legal compliance, security certification, or operational availability of private reporting channels.

---

## 2. Exact Repository State Inspected

The default branch is `main`. The latest branch commit returned during the validation was:

`b0a71f618cde4b75459b1094f80a30eec5a71543`

Commit message: `Update documentation audit remediation register (v1.1)`  
Commit timestamp: `2026-11-26T03:13:26Z`.

The repository metadata identifies the repository as public, with `main` as its default branch. GitHub's repository metadata returned no general licence identifier. This is consistent with the README's explicit statement that the repository has no general open-source licence; this validation does not recommend adding one by default.

### 2.1 Canonical baseline documents

All twelve expected baseline documents exist at their intended canonical paths:

| Document | Current observed state | Blob SHA (short) |
|---|---|---|
| `README.md` | Existing README; no document index; legacy project maturity vocabulary | `f2be2073` |
| `LAB-CHARTER.md` | Version 1.0; legacy maturity and lifecycle vocabularies | `9e7b5d0d` |
| `PUBLICATION-POLICY.md` | Version 1.0; P1 and data-classification issues remain | `27596603` |
| `RESEARCH-METHODOLOGY.md` | Version 1.0; substantial methodology document | `7ea6f180` |
| `CONTRIBUTING.md` | Version 1.0; no explicit permission grant for accepted external contributions | `e9ccc320` |
| `SECURITY.md` | Version 1.0; private reporting remains conditional | `0a8182ad` |
| `CODE-OF-CONDUCT.md` | Version 1.0; private conduct-reporting route not published | `540574b2` |
| `GOVERNANCE.md` | Version 1.0; legacy lifecycle and project-status definitions | `352806a5` |
| `PROJECT-LIFECYCLE.md` | Version 1.0; canonical stage/status distinction added | `3cc79c43` |
| `QUALITY-STANDARDS.md` | Version 1.0; maturity/readiness section exists, but table formatting and cross-document alignment remain | `5cf468c4` |
| `RESPONSIBLE-AI.md` | Version 1.0; separate AI risk classes and data-handling section | `f982800a` |
| `PROJECT-TEMPLATE.md` | Version 1.0; mixed lifecycle, quality, and publication fields | `1eb19040` |

### 2.2 Additional root-level draft files

The following files exist at the repository root as separate documents:

- `QUALITY-STANDARDS-v2.0-FULL-REWRITE.md`
- `GOVERNANCE-v2.0-FULL-REWRITE.md`
- `LAB-CHARTER-v2.0-FULL-REWRITE.md`

They are drafts, not canonical replacements. The canonical files listed in §2.1 remain at version 1.0.

The previously prepared `README-v2.0-FULL-REWRITE.md` and `PROJECT-TEMPLATE-v2.0-FULL-REWRITE.md` were not present in the inspected repository tree. Their canonical counterparts remain unchanged.

The `docs/audits/` collection contains its index and the six files belonging to `FCL-DOC-AUDIT-2026-001`.

### 2.3 Filename validation

The malformed paths `QUALITY-STANDARDS.md.` and `RESPONSIBLE-AI.md.` are no longer present. The exact canonical paths `QUALITY-STANDARDS.md` and `RESPONSIBLE-AI.md` exist. The filename correction is verified by commit `c073e881e7c9fc3d7e17f2c735b703d6be23e745`.

---

## 3. Finding-by-Finding Validation

| Finding | Severity | Validation status | Evidence and residual gap |
|---|---|---|---|
| AUD-001 | High | **Resolved** | The two canonical `.md` paths exist and the malformed trailing-dot paths are absent from the current root listing. The correction is recorded in commit `c073e881e7c9fc3d7e17f2c735b703d6be23e745`. Internal references should still be checked as part of the final link pass. |
| AUD-002 | High | **Partially resolved** | `PROJECT-LIFECYCLE.md` §4.1 separates Lifecycle Stage and Project Status and points to the separate maturity/readiness and publication documents. Its stage table defines the nine canonical stages, and §14 defines the ten canonical project statuses. However, `README.md` §12, `LAB-CHARTER.md` §§7 and 16, and `GOVERNANCE.md` §§6.3–6.4 still use competing vocabularies. `PROJECT-TEMPLATE.md` §20.1 still mixes stage and status labels. The v2.0 Charter and Governance documents exist only as alternate-name drafts. |
| AUD-003 | High | **Blocked** | `CONTRIBUTING.md` §3.2 clarifies that submission does not grant repository administration, maintainer privileges, decision authority, publication approval, or ownership of unrelated material. It does not establish the specific permission/licence grant the Lab needs to incorporate, reproduce, modify, maintain, and distribute accepted external contributions. The README states that there is no general repository licence. An explicit maintainer decision and project-specific terms are still required; the absence of a general licence must not be changed automatically. |
| AUD-004 | Medium | **Blocked** | `SECURITY.md` §6.1 makes GitHub Private Vulnerability Reporting conditional on enablement and states that the maintainer must enable it before describing it as available. The setting was not verifiable from the repository metadata returned in this read-only check. `CODE-OF-CONDUCT.md` §8.1 requires a private method explicitly published by the Lab, but no actual route is specified in the document. Neither route can be represented as operational based on the evidence available. |
| AUD-005 | Medium | **Open** | The canonical `README.md` still has no documentation index and no internal Markdown links to the supporting policy files. The README replacement was not present in the inspected repository tree. The separate `docs/audits/README.md` contains one relative link to the audit record; that path exists. This does not solve repository-wide navigation. |
| AUD-006 | Medium | **Open** | `PUBLICATION-POLICY.md` §10.1 lists Public, Internal, Confidential, Personal, and Sensitive or restricted. `RESPONSIBLE-AI.md` §6.1 uses Public, Internal, Confidential, and Restricted, while handling personal data separately in §6.3. `PROJECT-TEMPLATE.md` §9.2 lists Public, Internal, Confidential, and Restricted without a separate personal-data indicator. The classification model and the separate treatment of personal data have not been harmonised. |
| AUD-007 | Medium | **Blocked** | `PUBLICATION-POLICY.md` §5.3 lists additional P1 checks but does not explicitly state the conditions under which P1 material may be released, who approves it, or what restrictions must be disclosed. P2 material must remain unpublished pending resolution and reassessment (§5.4); P3 is excluded from the public process (§5.5), but the formal reclassification path after a material change is not defined. `PROJECT-TEMPLATE.md` §18.1 also uses `Not Reviewed` and `Deferred`, which are not part of the policy's `PENDING / APPROVED / REJECTED / WITHDRAWN` publication-status vocabulary. This needs an explicit maintainer decision. |
| AUD-008 | Medium | **Partially resolved** | `PROJECT-LIFECYCLE.md` §4.1 distinguishes Lifecycle Stage and Project Status. The canonical `QUALITY-STANDARDS.md` §4 defines Technical Maturity and Operational Readiness and distinguishes publication decisions. However, the Operational Readiness table in §4.2 has malformed row structure for `Limited Operational Use` and `Production-Oriented`. The README, Charter, Governance, and Project Template still conflate or reuse old maturity, stage, status, and release labels. The Quality Standards v2.0 file is a separate draft and does not replace the canonical standard. |
| AUD-009 | Medium | **Partially resolved** | The separate v2.0 Governance and Charter drafts indicate that consolidation work has started, and the Quality Standards v2.0 draft is also present. However, the canonical Charter, Governance, README, Quality, and Template files remain unchanged. Detailed methodology, lifecycle, AI, security, confidentiality, and publication material continues to be repeated across the canonical files. Duplication is not resolved until the drafts are applied at canonical paths and the full set is reviewed together. |
| AUD-010 | Low | **Open** | Metadata conventions remain inconsistent. The README has no document metadata block; the Charter and Publication Policy use `Established`; other policies use `Effective Date`; the Project Template uses `Created` and `Last Updated`; and the audit register has its own `Last verified` field. The canonical documents still carry mixed status wording. The register's `Last verified` date is 25 November 2026 although the latest `main` commit is dated 26 November 2026. A shared metadata convention has not been applied. |
| AUD-011 | Low | **Open** | `PROJECT-TEMPLATE.md` remains a 1,083-line, 27-section master template. The prepared replacement is not present at the canonical path in the inspected repository. In addition, a shorter replacement of the master alone does not satisfy the original recommendation to retain a comprehensive master while providing a separate short public project brief and keeping restricted assessment details out of public project records. A distinct short public brief has not been verified. |

---

## 4. Cross-Document Consistency Matrix

| Topic | Current assessment | Evidence / consequence |
|---|---|---|
| Lifecycle Stage vs Project Status | **Inconsistent** | `PROJECT-LIFECYCLE.md` now defines the distinction, but the README, Charter, Governance, and Project Template retain older overlapping lists. |
| Technical Maturity vs Operational Readiness vs Publication | **Partially separated** | `QUALITY-STANDARDS.md` §4 separates these dimensions in principle. The canonical template still has a single `Quality Level` field containing maturity, public-release, and production-oriented terms. |
| Data classification vs personal-data status | **Inconsistent** | Publication Policy, Responsible AI, and Project Template do not use the same model; personal data is treated as a classification in one place and a separate processing property in another. |
| Publication classes P0–P3 | **Incomplete** | P1 review requirements exist but controlled-publication release conditions are not explicit. P2/P3 reassessment and reclassification rules need a formal path. |
| Publication Status | **Inconsistent** | The Publication Policy uses `PENDING`, `APPROVED`, `REJECTED`, and `WITHDRAWN`; the Project Template adds `Not Reviewed` and `Deferred`. |
| AI Risk Classification A0–A4 | **Defined separately** | `RESPONSIBLE-AI.md` §4 defines A0–A4 as an AI risk framework. It should remain distinct from P0–P3 publication classification. |
| Contribution permissions and no-general-licence position | **Incomplete** | The lack of a general repository licence is intentional, but accepted external contributions lack an explicit permission/licence basis for incorporation and distribution. |
| Decision authority / founder-led model | **Consistent in principle** | `LAB-CHARTER.md` §5, `GOVERNANCE.md` §§3–5, and `CONTRIBUTING.md` §3 describe a founder-led model without claiming a board or committee. |
| Security and conduct reporting | **Not operationally verified** | Security reporting is conditional on a GitHub feature setting; conduct reporting requires a separately published private channel. |
| Metadata and document identity | **Inconsistent** | Metadata fields, date labels, and status descriptors vary; README has no common metadata block. |
| Policy ownership and duplicate requirements | **Partially aligned** | The specialised policies exist, but the canonical overview documents still repeat detailed lifecycle, AI, quality, confidentiality, and publication rules instead of consistently linking to their owners. |

---

## 5. Public-Repository and Navigation Checks

### 5.1 Repository paths

The twelve expected baseline documents are present at their exact canonical paths. The two malformed trailing-dot paths are absent. Three additional v2.0 draft files are present at the root and may create ambiguity because their canonical counterparts remain unchanged.

### 5.2 Markdown navigation

The twelve foundational documents were checked for internal Markdown hyperlinks. No internal Markdown links to the other foundational documents were found in that set. The canonical README therefore remains a non-linked policy overview rather than a functional documentation index.

`docs/audits/README.md` contains a relative link to `FCL-DOC-AUDIT-2026-001/00-AUDIT-RECORD.md`; the target file exists.

Many documents mention other policies as inline code filenames. Such references are readable but are not clickable navigation links.

### 5.3 Publication-safety limits

The validation was restricted to the public repository and its documentation. No private or proprietary repository or project material was accessed. This report does not certify that every historical commit, external dependency, or future change is free from confidential material or credentials. A dedicated secret scan and a separate history review were not performed as part of this documentation validation.

No legal-compliance or security-certification claim is made.

---

## 6. Updated Remediation Priorities

### Priority 1 — Apply canonical replacements

Replace the files at their intended canonical paths rather than leaving alternate-name drafts at the repository root:

1. `QUALITY-STANDARDS.md`
2. `PROJECT-TEMPLATE.md`
3. `README.md`
4. `GOVERNANCE.md`
5. `LAB-CHARTER.md`

After each replacement, inspect the exact canonical file on `main`. Once a replacement is verified, remove or deliberately archive the corresponding `*-v2.0-FULL-REWRITE.md` duplicate so two documents do not appear authoritative.

### Priority 2 — Close decision-dependent findings

- **AUD-003:** decide whether accepted external contributions require a project-specific licence, a contributor permission grant, a separate agreement, or a restriction on external code contributions until terms exist. Do not add a general repository licence by default.
- **AUD-007:** define P1 release conditions, approval authority, required disclosures, and formal P2/P3 reclassification conditions.
- **AUD-006:** approve one data-classification model and specify how personal-data status is recorded separately, where applicable.

### Priority 3 — Make reporting operational

- Verify the GitHub Private Vulnerability Reporting setting in repository settings.
- Establish and publish an actual private conduct-reporting route.
- Update `SECURITY.md` and `CODE-OF-CONDUCT.md` only after the routes are genuinely available.

### Priority 4 — Navigation and documentation quality

- Add a clickable documentation index to the canonical README.
- Add relative links between the authoritative policies.
- Establish and apply a common metadata convention.
- Provide a separate short public project brief while retaining an appropriately scoped comprehensive master template.
- Reduce duplicated procedures by keeping detailed requirements in the specialist policy documents.

### Priority 5 — Final verification

After the canonical changes and decisions have been applied:

1. Re-fetch all twelve canonical documents from `main`.
2. Validate all six project dimensions and their authoritative owners.
3. Recheck P0–P3, publication status, and AI risk A0–A4 as separate frameworks.
4. Validate all internal Markdown links and inline filename references.
5. Check metadata, document IDs, versions, and dates.
6. Run a dedicated secret scan and review public-facing content for unauthorised material.
7. Update the remediation register with current evidence and commit references.
8. Run a final read-only review before closing the audit.

---

## 7. Final Readiness Checklist

- [x] All twelve baseline documents exist at canonical paths.
- [x] Malformed trailing-dot filenames are corrected.
- [x] `PROJECT-LIFECYCLE.md` distinguishes Lifecycle Stage from Project Status.
- [ ] All dependent documents use the same canonical lifecycle and status vocabulary.
- [ ] Technical Maturity and Operational Readiness are correctly represented in the canonical template and README.
- [ ] Data classification and personal-data handling are harmonised.
- [ ] P1 release conditions and P2/P3 reclassification rules are explicit.
- [ ] Accepted external contribution permissions are defined without automatically adding a general repository licence.
- [ ] Security and conduct reporting routes are verified and operational.
- [ ] README contains a linked index of the Lab's documentation.
- [ ] Cross-document relative links are implemented and validated.
- [ ] Metadata conventions are consistent.
- [ ] A distinct short public project brief exists alongside the master template.
- [ ] Duplicate draft files are removed or intentionally archived after canonical replacements.
- [ ] Public-repository secret and publication-safety checks are completed.
- [ ] The remediation register reflects the latest repository commit and evidence.

### Final recommendation

Do not close `FCL-DOC-AUDIT-2026-001` yet. The filename issue is resolved and the Lifecycle/Status distinction is a valid partial correction, but the repository does not yet operate as one fully coherent documentation framework. Apply the canonical replacements, obtain the required maintainer decisions, verify the reporting routes, and repeat this read-only validation against the resulting `main` commit.

---

**Validation performed against the public repository only.**  
**No repository files, settings, branches, or Git history were modified during this validation.**
