# Framing Creativity Lab — Cross-Document Consistency and Link Validation

**Document ID:** FCL-AUD-VALID-003  
**Version:** 1.0  
**Status:** Validation completed — corrective work remains open  
**Validation Date:** 26 November 2026  
**Repository:** `framingcreativity/framing-creativity-lab`  
**Branch:** `main`  
**Commit Inspected:** `d83ac013e7079dfae524d27d96f61b199fa11975`  
**Tree Inspected:** `fce459a2cfbe926e52d3bcb32826c7abd6966c29`  
**Inspection Mode:** Read-only  
**Maintainer:** J-ART

---

## 1. Executive Summary

### Overall Verdict

**NOT READY FOR AUDIT CLOSURE — further remediation is required.**

The root README has been updated and now distinguishes the preserved v1.0 documentation from the eleven v2.0 drafts under maintainer review.

The review confirms that the principal project taxonomies, data classification values, AI risk classification, publication classification, and document metadata are broadly consistent across the v2.0 suite.

However, the repository still contains material cross-document reference problems, incorrect document self-identification in three v2.0 footers, one malformed internal filename reference, and two broken active Markdown links in the audit index.

The audit index and remediation register also need to reflect the latest repository checkpoint. The register contains wording that describes the proposed v2.0 taxonomy as approved, despite every v2.0 document remaining a draft.

The validation therefore does not support audit closure or blanket approval of the v2.0 document suite.

### Principal Results

| Area | Result |
|---|---|
| Root README versioning and navigation | Updated and validated |
| Root README relative links | All inspected targets exist |
| Eleven v2.0 document headers | Consistent |
| Document ID uniqueness | 11 unique IDs across 11 documents |
| Project taxonomy | Broadly consistent |
| Data classification | Broadly consistent |
| AI and publication risk taxonomies | Properly distinguished |
| v2.0 cross-document references | Reconciliation required |
| Audit index links | Two active links are broken |
| v2.0 document footer identification | Three incorrect filenames |
| Repository reporting configuration | Not verified |
| External contribution agreement process | Incomplete |
| Concise public project brief | Not found |

---

## 2. Scope and Method

The inspection covered:

- The root `README.md`.
- All eleven root-level v2.0 documents.
- The eleven preserved root-level v1.0 documents, with attention to their existing document references.
- `docs/audits/README.md`.
- `docs/audits/FCL-DOC-AUDIT-2026-001/03-REMEDIATION-REGISTER.md`.
- The audit record, audit report, validation prompt, integration snippet, and historical validation report.
- The repository tree and the existence of referenced paths.

The review examined:

1. Document identity and metadata.
2. Cross-document policy references.
3. Internal filename references.
4. Relative Markdown link targets.
5. Project lifecycle and status definitions.
6. Technical maturity and operational readiness.
7. Publication classification and publication status.
8. AI risk classification.
9. Data classification and privacy terminology.
10. Intellectual property, contribution permissions, and publication authority.
11. Security and conduct reporting statements.
12. Versioning, draft status, and approval boundaries.

### Limitations

This was a read-only repository inspection.

It did not verify GitHub repository settings, activate vulnerability reporting, create a private conduct-reporting channel, execute a legal review, or establish external contribution agreements.

The historical validation report dated 26 November 2026 remains an immutable record of its earlier inspected commit. It is not replaced by this report.

---

## 3. Repository and Document Inventory

The inspected repository tree contains 32 tracked files.

The eleven v2.0 documents are present at their intended root paths:

| Document | Document ID | Version | Status |
|---|---|---:|---|
| `LAB-CHARTER-v2.0.md` | FCL-GOV-001 | 2.0 | Draft for Maintainer Review |
| `GOVERNANCE-v2.0.md` | FCL-GOV-003 | 2.0 | Draft for Maintainer Review |
| `PROJECT-LIFECYCLE-v2.0.md` | FCL-PROC-001 | 2.0 | Draft for Maintainer Review |
| `PROJECT-TEMPLATE-v2.0.md` | FCL-TPL-001 | 2.0 | Draft for Maintainer Review |
| `QUALITY-STANDARDS-v2.0.md` | FCL-STD-001 | 2.0 | Draft for Maintainer Review |
| `RESEARCH-METHODOLOGY-v2.0.md` | FCL-METH-001 | 2.0 | Draft for Maintainer Review |
| `PUBLICATION-POLICY-v2.0.md` | FCL-POL-001 | 2.0 | Draft for Maintainer Review |
| `RESPONSIBLE-AI-v2.0.md` | FCL-AI-001 | 2.0 | Draft for Maintainer Review |
| `CONTRIBUTING-v2.0.md` | FCL-CONTRIB-001 | 2.0 | Draft for Maintainer Review |
| `SECURITY-v2.0.md` | FCL-SEC-001 | 2.0 | Draft for Maintainer Review |
| `CODE-OF-CONDUCT-v2.0.md` | FCL-GOV-002 | 2.0 | Draft for Maintainer Review |

All eleven documents use the same status and pending effective-date convention.

All eleven Document IDs are unique.

The original v1.0 documents remain present. No v1.0 document was overwritten or removed by the v2.0 versioning strategy.

---

## 4. Cross-Document Consistency Findings

### 4.1 Project Lifecycle and Status

The review confirms the distinction between:

- Lifecycle Stage.
- Project Status.
- Technical Maturity.
- Operational Readiness.
- Publication Classification.
- Publication Status.

The nine lifecycle stages and ten Project Status values in `PROJECT-LIFECYCLE-v2.0.md` are consistent with the duplicated definitions in `GOVERNANCE-v2.0.md`.

The Technical Maturity and Operational Readiness vocabularies in `QUALITY-STANDARDS-v2.0.md` are reflected consistently in the Governance and Project Template drafts.

**Result:** Substantively consistent. Cross-document source references still need correction.

### 4.2 Publication Classification and Status

The Publication Policy defines:

| Value | Classification |
|---|---|
| P0 | Public-ready |
| P1 | Controlled publication |
| P2 | Restricted review |
| P3 | Non-publishable |

Publication Status uses:

- `PENDING`
- `APPROVED`
- `REJECTED`
- `WITHDRAWN`

The Project Template and Governance drafts reproduce the same values and maintain the distinction between classification and approval.

PENDING is not conditional approval. APPROVED does not itself mean a release has already been made public.

**Result:** Substantively consistent.

### 4.3 AI Risk Classification

The Responsible AI draft defines:

| Value | Classification |
|---|---|
| A0 | Minimal Risk |
| A1 | Low Risk |
| A2 | Moderate Risk |
| A3 | High Risk |
| A4 | Restricted Use |

AI Risk Classification is explicitly separate from Publication Classification P0–P3.

The distinction is preserved in the Research Methodology draft.

**Result:** Consistent.

### 4.4 Data Classification and Personal Information

The four data classification values used by Publication Policy, Responsible AI, Research Methodology, and Security are:

- Public
- Internal
- Confidential
- Restricted

Personal information and sensitive information are treated as data characteristics rather than additional classification values.

The Publication Policy defines the internal handling rule:

- Personal information should be classified at least as Confidential.
- Sensitive personal information and information subject to stricter restrictions should be classified as Restricted.

Research Methodology reflects these thresholds.

Responsible AI states that personal and sensitive information are characteristics and that the four classification values must remain consistent with Publication Policy.

**Result:** Broadly consistent. The Responsible AI draft should explicitly point readers to the Publication Policy's personal-information classification thresholds to make the dependency easier to locate.

### 4.5 Intellectual Property and Contribution Rights

The Charter, Governance, Publication Policy, and Contributing drafts are aligned on the following principles:

- Submission does not automatically transfer ownership.
- Acceptance does not itself grant unrestricted rights.
- Permission to incorporate, reproduce, modify, distribute, or publish a contribution must be established through applicable licence terms or an explicit written agreement.
- Third-party material remains subject to its own rights and restrictions.
- The repository has no general open-source licence.
- Public accessibility is not permission to reuse original material.

**Result:** The principles are consistent. The practical agreement process remains incomplete and must be clarified before external contributions are accepted for incorporation or distribution.

### 4.6 Governance and Conduct

The Governance and Code of Conduct drafts consistently describe the Lab as founder-led and maintained by J-ART.

The Code of Conduct explicitly states that:

- No independent internal complaints body currently exists.
- No guaranteed formal internal appeal mechanism exists.
- The founder and maintainer retains final internal decision-making authority, subject to applicable law, contracts, platform procedures, and third-party rights.

This is consistent with the Governance model.

**Result:** Consistent disclosure of the current governance structure. An independent reporting route has not been established.

### 4.7 Security Reporting

The Security draft states that GitHub Private Vulnerability Reporting is the preferred method only if enabled and verified.

It explicitly states that the repository's configuration has not yet been verified.

The Code of Conduct draft states that an accessible private conduct-reporting channel has not yet been verified as published.

Neither document claims that an unverified channel is operational.

**Result:** The documentary statements are appropriately cautious. The actual configuration and reporting channels remain unresolved operational dependencies.

---

## 5. Cross-Document Reference Reconciliation

The following references in v2.0 documents still point to unversioned v1.0 files even though corresponding v2.0 files exist.

These references should be reviewed and updated to the corresponding v2.0 filenames where the intended source is the revised draft suite.

| v2.0 document | References requiring review |
|---|---|
| `LAB-CHARTER-v2.0.md` | `PROJECT-LIFECYCLE.md`, `PUBLICATION-POLICY.md`, `RESPONSIBLE-AI.md`, `RESEARCH-METHODOLOGY.md`, `SECURITY.md`, `CONTRIBUTING.md`, `CODE-OF-CONDUCT.md` |
| `GOVERNANCE-v2.0.md` | `LAB-CHARTER.md`, `PROJECT-LIFECYCLE.md`, `QUALITY-STANDARDS.md`, `PUBLICATION-POLICY.md`, `SECURITY.md`, `CONTRIBUTING.md`, `CODE-OF-CONDUCT.md`, `RESEARCH-METHODOLOGY.md`, `RESPONSIBLE-AI.md` |
| `PROJECT-LIFECYCLE-v2.0.md` | `PUBLICATION-POLICY.md`, `SECURITY.md`, `RESPONSIBLE-AI.md`, `RESEARCH-METHODOLOGY.md`, `CONTRIBUTING.md`, `CODE-OF-CONDUCT.md` |
| `PROJECT-TEMPLATE-v2.0.md` | `PROJECT-LIFECYCLE.md`, `QUALITY-STANDARDS.md`, `PUBLICATION-POLICY.md`, `RESPONSIBLE-AI.md`, `SECURITY.md`, `CONTRIBUTING.md`, `LAB-CHARTER.md`, `GOVERNANCE.md`, `RESEARCH-METHODOLOGY.md`, `CODE-OF-CONDUCT.md` |
| `QUALITY-STANDARDS-v2.0.md` | `PUBLICATION-POLICY.md`, `SECURITY.md`, `RESPONSIBLE-AI.md`, `RESEARCH-METHODOLOGY.md`, `PROJECT-LIFECYCLE.md`, `CONTRIBUTING.md`, `CODE-OF-CONDUCT.md` |
| `RESEARCH-METHODOLOGY-v2.0.md` | `SECURITY.md`, `CONTRIBUTING.md`, `CODE-OF-CONDUCT.md` |
| `PUBLICATION-POLICY-v2.0.md` | `RESPONSIBLE-AI.md`, `SECURITY.md`, `RESEARCH-METHODOLOGY.md`, `CONTRIBUTING.md`, `CODE-OF-CONDUCT.md` |
| `RESPONSIBLE-AI-v2.0.md` | `SECURITY.md`, `RESEARCH-METHODOLOGY.md`, `CONTRIBUTING.md`, `CODE-OF-CONDUCT.md` |
| `SECURITY-v2.0.md` | `SECURITY.md`, `CONTRIBUTING.md`, `CODE-OF-CONDUCT.md` |
| `CONTRIBUTING-v2.0.md` | `CONTRIBUTING.md`, `SECURITY.md`, `CODE-OF-CONDUCT.md` |
| `CODE-OF-CONDUCT-v2.0.md` | `CODE-OF-CONDUCT.md`, `CONTRIBUTING.md`, `SECURITY.md` |

This is a reference reconciliation task, not an instruction to delete, rename, or overwrite the v1.0 documents.

The original files remain preserved. A deliberate reference to a v1.0 document may remain where the text specifically concerns the earlier baseline or historical policy state.

The v2.0 documents currently use code-formatted filenames for most internal references rather than clickable Markdown links. Converting appropriate policy references into relative Markdown links would improve navigation after the target versions have been reconciled.

---

## 6. Link and Filename Validation

### 6.1 Root README

The relative Markdown links in the updated root `README.md` were checked against the repository tree.

All inspected targets exist, including:

- Both v1.0 and v2.0 root documents.
- The audit index at `docs/audits/README.md`.

The README correctly distinguishes preserved original documents from drafts under review.

**Result:** Passed.

### 6.2 Audit Index — Broken Historical Validation Link

The current link is:

`FCL-DOC-AUDIT-2026-11-26.md`

That path does not exist.

The actual historical validation report is:

`FCL-DOC-AUDIT-2026-001/06-POST-REMEDIATION-VALIDATION-2026-11-26.md`

The active Markdown link in `docs/audits/README.md` must be updated to that exact relative target.

**Result:** Failed — correction required.

### 6.3 Audit Index — Broken Archive Link

The current target is:

`archive/README.md`

From `docs/audits/README.md`, this resolves to:

`docs/audits/archive/README.md`

That file does not exist.

The repository instead contains:

`docs/archives/README.md`

The corresponding relative path from `docs/audits/README.md` is:

`../archives/README.md`

The existing `docs/archives/README.md` is currently empty and should be populated with a meaningful archive description or the index should avoid linking to it until it has content.

**Result:** Failed — correction required.

### 6.4 Malformed v2.0 Filename Reference

In `CONTRIBUTING-v2.0.md`, the document reference table contains:

`PROJECT-LIFECYCLE-v2.0`

The actual repository filename is:

`PROJECT-LIFECYCLE-v2.0.md`

The reference must include the `.md` extension.

The physical file itself is correctly named. This is an internal reference defect.

**Result:** Failed — correction required.

### 6.5 Document Self-Identification

Three v2.0 footers identify the v1.0 filename rather than the file being reviewed.

| Actual file | Current footer identification | Correct identification |
|---|---|---|
| `CONTRIBUTING-v2.0.md` | `CONTRIBUTING.md` | `CONTRIBUTING-v2.0.md` |
| `SECURITY-v2.0.md` | `SECURITY.md` | `SECURITY-v2.0.md` |
| `CODE-OF-CONDUCT-v2.0.md` | `CODE-OF-CONDUCT.md` | `CODE-OF-CONDUCT-v2.0.md` |

The related-policy references in the Contributing footer should also be checked against the v2.0 filenames.

**Result:** Failed — correction required.

### 6.6 References That Are Not Broken Links

The following references should not be classified as missing repository files:

- `PROJECT.md` in `PROJECT-TEMPLATE-v2.0.md` is the expected filename of a project record generated from the template. It is not expected to exist in the documentation root.
- `ATTRIBUTIONS.md` in `PUBLICATION-POLICY-v2.0.md` is presented as a recommended project-level attribution file or equivalent, not as an existing mandatory root document.
- The Markdown link shown inside the fenced code block in `05-README-INTEGRATION-SNIPPET.md` is example content intended to be inserted into the root README. It is not an active relative link from the snippet's own directory.
- References to earlier full-rewrite filenames in the historical validation report belong to that report's earlier inspection context. The historical report must remain unchanged.

---

## 7. Audit Index and Remediation Register Consistency

The latest repository commit is:

`d83ac013e7079dfae524d27d96f61b199fa11975`

The corresponding commit tree is:

`fce459a2cfbe926e52d3bcb32826c7abd6966c29`

The root README update is included in that commit.

The audit index still records the earlier checkpoint at:

`417b114874d17e64f5d86c3bcb071cdcff13834f`

It also states that the root README still requires alignment. That statement is now outdated.

The audit index should be updated to reflect:

- The root README has been aligned with the v1.0 preservation and v2.0 draft strategy.
- Cross-document reference reconciliation remains outstanding.
- Two active links in the audit index still require repair.
- The latest inspected checkpoint is the README commit listed in this report.
- The latest remediation register must describe the current status rather than continue presenting the earlier checkpoint as the latest one.

The current remediation register is Version 1.3. A subsequent version should record this new checkpoint and update the evidence log.

### 7.1 Approval Language Conflict

Section 4 of the current remediation register is titled:

`Approved Canonical Project Vocabulary`

It also describes the taxonomy as a maintainer-approved framework.

This wording conflicts with the status of the eleven v2.0 documents, all of which remain:

`Draft for Maintainer Review`

Their effective dates remain pending approval.

Recommended correction:

- Rename the section to **Proposed Canonical Project Vocabulary — v2.0 Draft**.
- Replace language implying formal approval with wording that identifies the values as the proposed v2.0 framework.
- Preserve the distinction between a proposed taxonomy and an approved policy.

The presence of a complete and internally consistent draft framework does not establish formal approval.

---

## 8. Outstanding Findings and Dependencies

The following issues remain open or incomplete.

| Finding | Current conclusion | Required next action |
|---|---|---|
| AUD-001 | Physical v2.0 lifecycle filename is correct, but a malformed internal reference remains. | Correct the missing `.md` extension and revalidate all path references. |
| AUD-002 | The six project dimensions are defined, but cross-document references remain inconsistent. | Reconcile references and confirm authority boundaries. |
| AUD-003 | Contribution rights language is substantially improved. | Establish the practical written agreement and permission process before accepting external contributions. |
| AUD-004 | Reporting routes are explicitly identified as unverified. | Verify GitHub Private Vulnerability Reporting and establish a private conduct-reporting route. |
| AUD-005 | Root README alignment is complete. | Repair audit-index links and finish navigation validation. |
| AUD-006 | Four-level data classification is broadly consistent. | Preserve the shared definitions and complete final review and approval. |
| AUD-007 | P0–P3 and Publication Status definitions are consistent. | Complete final policy review and approval. |
| AUD-008 | Six project dimensions are distinguished. | Finish reference reconciliation and final approval. |
| AUD-009 | Policy responsibilities are more clearly separated, but references still point to v1.0 files in many v2.0 drafts. | Reconcile references and reduce remaining duplication. |
| AUD-010 | Header metadata is consistent; three v2.0 footer identities are wrong. | Correct the three footer filenames and revalidate document metadata. |
| AUD-011 | A separate concise public project brief has not been verified. | Decide whether to create a short public project brief distinct from the comprehensive project template. |

No finding should be marked Resolved solely because a draft file exists.

No repository setting or reporting route should be marked operational without direct verification.

---

## 9. Required Remediation Sequence

The following work is required before another complete validation:

1. Reconcile the v1.0 and v2.0 references in the eleven v2.0 documents according to Section 5.

2. Correct the missing `.md` extension in `CONTRIBUTING-v2.0.md`.

3. Correct the self-identification and related-policy filenames in the Contributing, Security, and Code of Conduct v2.0 footers.

4. Correct the two broken active Markdown links in `docs/audits/README.md`.

5. Populate `docs/archives/README.md` or remove the archive navigation entry until the archive has a meaningful description.

6. Update the remediation register to a new version reflecting the README commit and the findings in this report. Correct the approval language in its proposed vocabulary section.

7. Update the audit index to a new version, record the new checkpoint, and point to the current remediation register and this validation report.

8. Resolve the practical contribution-permission process and the private reporting channel dependencies.

9. Decide whether a concise public project brief is required.

10. Run a new read-only validation against the actual `main` branch, including relative link resolution, document identity, cross-reference targets, and policy vocabulary.

The historical audit report and the earlier historical validation report must remain unchanged.

---

## 10. Final Assessment

The documentation suite has progressed materially.

The root README now reflects the intended versioning strategy. The eleven v2.0 documents are present, their metadata is consistent, and the core project, publication, data, and AI risk vocabularies are broadly aligned.

The remaining defects are not primarily structural omissions. They concern the precision of the document system: references to the wrong version, incorrect self-identification, broken navigation, stale audit records, and unresolved operational channels.

The distinction matters. A coherent policy suite is not simply a collection of individually well-written documents. Its authority depends on whether each document points to the correct source, whether the same terms retain the same meaning, and whether the stated procedures can actually be used.

**Validation result: NOT READY FOR AUDIT CLOSURE.**

A subsequent validation must be performed after the corrective work and must identify the exact commit and tree inspected.

---

**Framing Creativity Lab**  
Independent Research · Applied AI · Creative Technology · Experimental Design

**Maintainer:** J-ART  
**Document:** `07-CROSS-DOCUMENT-VALIDATION-2026-11-26.md`  
**Version:** 1.0
