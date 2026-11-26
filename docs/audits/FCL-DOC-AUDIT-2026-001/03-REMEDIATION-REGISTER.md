# Remediation Register — FCL-DOC-AUDIT-2026-001

**Document ID:** FCL-AUD-REG-001  
**Version:** 1.2  
**Status:** Open — remediation in progress  
**Source:** `02-AUDIT-REPORT.md`  
**Baseline commit:** `e026bdc5cc4a78dd80570f8c93d50008711de262`  
**Last verified:** 26 November 2026  
**Inspected branch:** `main`  
**Inspected commit:** `f145370386281415ec443018c2734211bddc7347`  
**Maintainer:** J-ART

---

## Purpose

This register tracks the corrective actions arising from the initial documentation audit of Framing Creativity Lab.

It records the current status of each finding, the decisions or dependencies required to resolve it, and the evidence supporting its status.

A draft, recommendation, or locally prepared replacement is not a completed repository correction.

A finding may be marked **Resolved** only after the canonical file or configuration has been inspected on `main` and the correction has been verified.

The register is maintained as part of the permanent audit record. Historical findings and evidence must not be silently removed or rewritten.

---

## 1. Status Vocabulary

| Status | Definition |
|---|---|
| Open | No corrective implementation has been verified at the canonical repository location. |
| In progress | Corrective work has started, but the required changes have not yet been fully applied and verified. |
| Partially resolved | A substantive part of the correction is present, but one or more required conditions remain incomplete. |
| Blocked — decision | An explicit maintainer decision is required before the corrective action can be completed. |
| Blocked — configuration | A repository setting, access control, or operational channel must be checked or configured. |
| Resolved | The canonical file or configuration has been inspected and the correction has been verified. |
| Accepted risk | The maintainer has explicitly accepted and documented the remaining risk. |
| Not applicable | The scope has materially changed. The rationale and approval must be recorded. |

A finding must not be marked Resolved merely because a replacement document has been drafted or uploaded under an alternative filename.

---

## 2. Findings Register

| Finding | Severity | Affected area | Required corrective action | Current status | Verification condition |
|---|---|---|---|---|---|
| AUD-001 | High | Documentation filenames and internal references | Maintain the exact canonical filenames `QUALITY-STANDARDS.md` and `RESPONSIBLE-AI.md`. Verify references and repository paths. | **Resolved** | Both canonical paths exist on `main`, and neither malformed dotted filename remains. Verified by commit `c073e881e7c9fc3d7e17f2c735b703d6be23e745`. |
| AUD-002 | High | README, Charter, Governance, Lifecycle, Quality Standards, Project Template | Apply the approved project vocabulary consistently. Keep Lifecycle Stage and Project Status separate from Technical Maturity, Operational Readiness, Publication Classification, and Publication Status. | **Partially resolved** | `PROJECT-LIFECYCLE.md` contains the canonical nine Lifecycle Stages and ten Project Status values. The remaining canonical documents still contain conflicting or legacy terminology. |
| AUD-003 | High | `CONTRIBUTING.md`, `PUBLICATION-POLICY.md`, repository licensing | Define the permission or licence terms under which the Lab may incorporate, reproduce, modify, maintain, and distribute accepted external contributions. Preserve the intentional absence of a general repository licence unless a separate decision changes it. | **Blocked — decision** | An explicit maintainer decision is recorded. Contribution and publication terms agree. No rights are inferred merely from submission or acceptance. Legal review should be considered where appropriate. |
| AUD-004 | Medium | `SECURITY.md`, `CODE-OF-CONDUCT.md`, reporting channels | Verify whether GitHub Private Vulnerability Reporting is enabled. Establish an actual private route for conduct reports. Do not describe conditional or unpublished channels as operational. | **Blocked — configuration** | The repository setting is checked and recorded. Reporting routes are usable and accurately described in the relevant policies. The actual GitHub configuration has not yet been verified. |
| AUD-005 | Medium | `README.md`, documentation navigation, cross-document references | Add a useful documentation index to the root README and validate relative links between authoritative documents. | **Open** | The canonical `README.md` remains unchanged and does not contain the required documentation index. The audit collection index in `docs/audits/README.md` does not replace the main documentation index. |
| AUD-006 | Medium | `PUBLICATION-POLICY.md`, `RESPONSIBLE-AI.md`, `PROJECT-TEMPLATE.md` | Adopt and use a consistent data-classification model. Clearly distinguish information classification from personal-data status and AI risk classification. | **Open** | The same approved terms and definitions appear in the authoritative policies and project template, without contradictory categories or labels. |
| AUD-007 | Medium | `PUBLICATION-POLICY.md`, `PROJECT-TEMPLATE.md` | Clarify the requirements and approval conditions for P1 Controlled Publication. Require documented resolution, formal reclassification, and renewed review before P2 or P3 material can be reconsidered. | **Blocked — decision** | The maintainer approves explicit P1 release conditions and P2/P3 reassessment rules. The policy and template reflect the same process. |
| AUD-008 | Medium | `QUALITY-STANDARDS.md`, `PROJECT-TEMPLATE.md`, `README.md`, `PROJECT-LIFECYCLE.md` | Separate Lifecycle Stage, Project Status, Technical Maturity, Operational Readiness, Publication Classification, and Publication Status. Do not treat technical maturity or public availability as evidence of production readiness. | **Partially resolved** | The Lifecycle Stage and Project Status distinction is present in `PROJECT-LIFECYCLE.md`. `QUALITY-STANDARDS.md` contains separate maturity and readiness sections, but its operational-readiness table has formatting defects and the remaining documents are not aligned. |
| AUD-009 | Medium | README, Charter, Governance, Contributing, Security, Quality, Research, Responsible AI, Lifecycle, Project Template | Reduce duplicated policy content. Keep detailed requirements in their designated authoritative documents and use concise summaries and cross-references elsewhere. | **Partially resolved** | Some document restructuring and replacement drafts have been prepared. The canonical documents still contain substantial overlapping procedures and require a coordinated review after replacement. |
| AUD-010 | Low | Metadata across policy and template documents | Establish a consistent metadata convention for document ID, version, status, effective or revision date, and maintainer. Preserve meaningful historical dates and distinguish draft status from approved policy status. | **Open** | A metadata convention is approved and consistently applied to the in-scope documents. |
| AUD-011 | Low | `PROJECT-TEMPLATE.md` | Retain a comprehensive internal master template while providing a shorter public project record or brief. Keep restricted assessment details outside public project records. | **Open** | The canonical project template has been reviewed and the public/internal documentation boundary has been established. A separate concise public project brief is available where appropriate. |

---

## 3. Approved Canonical Project Vocabulary

The maintainer approved the following separation of project dimensions.

Their definitions must be maintained in the authoritative documents rather than independently redefined in every file.

| Dimension | Canonical values | Authoritative document |
|---|---|---|
| Lifecycle Stage | Idea and Intake; Proposal; Discovery and Feasibility; Experimentation and Development; Validation and Evaluation; Publication Review; Publication and Release; Maintenance and Evolution; Archival or Discontinuation | `PROJECT-LIFECYCLE.md` |
| Project Status | Proposed; Concept; Experimental; Prototype; Development; Validation; Published; Maintenance; Archived; Discontinued | `PROJECT-LIFECYCLE.md` |
| Technical Maturity | Not Assessed; Exploratory; Prototype; Validated | `QUALITY-STANDARDS.md` |
| Operational Readiness | Not Assessed; Research or Experimental Use Only; Demonstration Only; Limited Operational Use; Production-Oriented | `QUALITY-STANDARDS.md` |
| Publication Classification | P0; P1; P2; P3 | `PUBLICATION-POLICY.md` |
| Publication Status | PENDING; APPROVED; REJECTED; WITHDRAWN | `PUBLICATION-POLICY.md` |

These dimensions answer different questions:

- **Lifecycle Stage** identifies the project's position in the Lab's workflow.
- **Project Status** describes the current state of the project.
- **Technical Maturity** describes the maturity of the technical work and the evidence supporting it.
- **Operational Readiness** describes the conditions under which the work may be used.
- **Publication Classification** determines the applicable publication scrutiny and restrictions.
- **Publication Status** records the publication review state or decision.

They must not be merged into a single status field or treated as interchangeable levels.

AI Risk Classification is a separate subject governed by `RESPONSIBLE-AI.md`. Its A0–A4 values must not be confused with the publication classification P0–P3.

---

## 4. Verified Repository State

The following canonical files were inspected on the default branch `main` at commit:

`f145370386281415ec443018c2734211bddc7347`

Verification date: 26 November 2026.

| Canonical path | Observed state | Blob SHA (short) |
|---|---|---|
| `README.md` | Existing version; no complete documentation index; legacy project maturity vocabulary remains | `f2be2073` |
| `LAB-CHARTER.md` | Version 1.0; legacy project maturity and lifecycle vocabularies remain | `9e7b5d0d` |
| `PUBLICATION-POLICY.md` | Version 1.0; P1 publication conditions and data-classification consistency remain unresolved | `27596603` |
| `RESEARCH-METHODOLOGY.md` | Version 1.0; substantial methodology document | `7ea6f180` |
| `CONTRIBUTING.md` | Version 1.0; explicit permission terms for accepted external contributions remain unresolved | `e9ccc320` |
| `SECURITY.md` | Version 1.0; private vulnerability reporting remains conditional on configuration | `0a8182ad` |
| `CODE-OF-CONDUCT.md` | Version 1.0; a private conduct-reporting route has not been published | `540574b2` |
| `GOVERNANCE.md` | Version 1.0; legacy lifecycle and project-status definitions remain | `352806a5` |
| `PROJECT-LIFECYCLE.md` | Version 1.0; canonical Lifecycle Stage and Project Status distinction added | `3cc79c43` |
| `QUALITY-STANDARDS.md` | Version 1.0; separate maturity and readiness sections exist, but table formatting and cross-document alignment remain incomplete | `5cf468c4` |
| `RESPONSIBLE-AI.md` | Version 1.0; includes separate AI Risk Classification and data-handling sections | `f982800a` |
| `PROJECT-TEMPLATE.md` | Version 1.0; legacy mixed quality, lifecycle, and publication fields remain | `1eb19040` |

### 4.1 Additional Draft Files

The following v2.0 documents exist at the repository root as separate draft files:

| Draft file | Blob SHA (short) | Canonical replacement |
|---|---|---|
| `QUALITY-STANDARDS-v2.0-FULL-REWRITE.md` | `c9a181ed` | `QUALITY-STANDARDS.md` |
| `GOVERNANCE-v2.0-FULL-REWRITE.md` | `d52bec57` | `GOVERNANCE.md` |
| `LAB-CHARTER-v2.0-FULL-REWRITE.md` | `10d0d6fa` | `LAB-CHARTER.md` |

These files are drafts, not canonical replacements.

The prepared `README-v2.0-FULL-REWRITE.md` and `PROJECT-TEMPLATE-v2.0-FULL-REWRITE.md` were not present in the inspected repository tree. Their canonical counterparts remain unchanged.

The separate Quality Standards draft was added by commit:

`b711dbdbd9de7f58f8915a988ef6f8e33daae6d1`

The Governance and Lab Charter drafts were added separately and must not be treated as approved policy versions.

After the canonical documents have been replaced and verified, remove or deliberately relocate the separate root draft files. Do not leave competing files that appear to be current authoritative standards.

### 4.2 Audit Archive

The following audit records were present in the repository:

- `docs/audits/README.md`
- `docs/audits/FCL-DOC-AUDIT-2026-001/00-AUDIT-RECORD.md`
- `docs/audits/FCL-DOC-AUDIT-2026-001/01-MASTER-PROMPT.md`
- `docs/audits/FCL-DOC-AUDIT-2026-001/02-AUDIT-REPORT.md`
- `docs/audits/FCL-DOC-AUDIT-2026-001/03-REMEDIATION-REGISTER.md`
- `docs/audits/FCL-DOC-AUDIT-2026-001/04-POST-REMEDIATION-VALIDATION-PROMPT.md`
- `docs/audits/FCL-DOC-AUDIT-2026-001/06-POST-REMEDIATION-VALIDATION-2026-11-26.md`

The post-remediation validation report is an additional historical record. It does not replace the original audit report or this remediation register.

---

## 5. Evidence Log

| Date | Finding | Action / evidence | Commit or reference | Result |
|---|---|---|---|---|
| 2026-11-25 | Baseline | Initial documentation audit performed against the baseline repository state. | `e026bdc5cc4a78dd80570f8c93d50008711de262` | Baseline recorded |
| 2026-11-25 | Audit archive | Audit report, master prompt, register, validation prompt, and archive index added. | `386a3ac3e7cbfc70eb40226d4d1ce1e06af2606c` | Archive present |
| 2026-11-25 | AUD-001 | Corrected malformed filenames to `QUALITY-STANDARDS.md` and `RESPONSIBLE-AI.md`. | `c073e881e7c9fc3d7e17f2c735b703d6be23e745` | Verified — Resolved |
| 2026-11-25 | AUD-002 / AUD-008 | Added the canonical Lifecycle Stage and Project Status distinction and references to separate maturity, readiness, and publication dimensions. | `216ce2ac33a2e14a2959fa54bb2cf9f8abd5c890` | Partially implemented |
| 2026-11-25 | AUD-008 | Added a Quality Standards v2.0 draft as a separate root file. The canonical file was not replaced. | `b711dbdbd9de7f58f8915a988ef6f8e33daae6d1` | Draft only — not a canonical correction |
| 2026-11-25 | AUD-009 | Added Governance and Lab Charter v2.0 replacement drafts as separate root files. | `cf76ad7b86c95c331f1e3520db9ec95b25e85706`; `585a4f2eb3acaab9fbe3470fb49d650eda1d4878` | Drafts only — canonical files unchanged |
| 2026-11-26 | AUD-001–AUD-011 | Read-only post-remediation validation completed. | Inspected commit: `b0a71f618cde4b75459b1094f80a30eec5a71543` | 1 Resolved; 3 Partially resolved; 3 Blocked; 4 Open |
| 2026-11-26 | Validation archive | Post-remediation validation report renamed and archived under the audit folder. | `419f36d37c3189a4afa3841281c264805b6d38ca` | Report present |
| 2026-11-26 | Audit index | Added a link to the post-remediation validation report in `docs/audits/README.md`. | `bd39a2020b4f0bbe18bb93d822d45b9085ce5d63` | Index updated |
| 2026-11-26 | Register verification | Inspected the register, audit index, validation report, canonical documents, and relevant draft files on `main`. | `f145370386281415ec443018c2734211bddc7347` | Verification completed; register correction required |

Add a dated row for every subsequent material change.

Each evidence entry should identify:

- The finding affected.
- The canonical file or configuration changed.
- The commit or configuration reference.
- The verification performed.
- The resulting status.

A draft upload must be recorded as a draft, not as a resolved finding.

---

## 6. Remediation Sequence

The following sequence defines the remaining work.

1. Replace `QUALITY-STANDARDS.md` with the approved v2.0 content. Verify the canonical path, metadata, tables, links, and all six project dimensions. Remove or relocate the separate root draft after verification.

2. Replace `PROJECT-TEMPLATE.md` with the v2.0 content. Verify that the project record uses the canonical field names and values, and that it distinguishes public project information from restricted assessment details.

3. Replace `README.md` with the v2.0 content. Verify the documentation index, repository structure, and every relative link.

4. Replace `GOVERNANCE.md` and `LAB-CHARTER.md` with their respective v2.0 contents. Check that the Charter establishes foundational principles while Governance defines operational authority and decision processes.

5. Remove or deliberately archive the separate root-level draft files after their canonical replacements have been verified. Ensure that the repository does not contain competing versions of current policies.

6. Resolve the contribution-rights decision for AUD-003. Document the selected permission or licence arrangement before accepting external contributions under unclear terms.

7. Resolve the P1/P2/P3 publication decision for AUD-007. Define the conditions for P1 publication and the formal reassessment process for P2/P3 material.

8. Verify GitHub Private Vulnerability Reporting and establish the private conduct-reporting route for AUD-004. Record the actual configuration and confirm that the channels are usable.

9. Harmonise the data-classification terminology for AUD-006. Distinguish information sensitivity from personal-data status and AI risk classification.

10. Establish and apply a consistent document metadata convention for AUD-010. Preserve meaningful historical dates and distinguish drafts from approved policy documents.

11. Complete the public/internal project documentation distinction for AUD-011. Decide whether a separate concise public project brief is required in addition to the comprehensive master template.

12. Review the in-scope documents together for duplicated procedures, contradictory definitions, missing references, and inconsistent ownership of policy requirements.

13. Run the post-remediation validation protocol against the actual updated `main` branch. Record the inspected commit and produce a new dated validation report.

---

## 7. Completion Rule

The audit is not closed merely because replacement documents have been drafted or uploaded under alternate filenames.

A finding may be marked Resolved only after read-only validation confirms that:

- The correction exists at the canonical repository path on `main`.
- The file content and metadata are correct.
- Cross-references and relative links resolve.
- Authoritative definitions are consistent across dependent documents.
- No contradictory terminology remains within the finding's scope.
- Required repository settings and reporting channels have actually been verified.
- No private, proprietary, confidential, or otherwise unauthorised material has been introduced.
- The evidence log contains the relevant commit or configuration reference and a reproducible verification note.

The audit may be closed only when every finding is one of the following:

- Resolved.
- Accepted risk, with explicit maintainer approval and rationale.
- Not applicable, with explicit justification and maintainer approval.

The final validation must be based on the actual repository state, not on draft files, earlier summaries, or assumed completion.

---

**Framing Creativity Lab**  
*Independent Research · Applied AI · Creative Technology · Experimental Design*

**Maintainer:** J-ART
