# Remediation Register — FCL-DOC-AUDIT-2026-001

**Document ID:** FCL-AUD-REG-001  
**Version:** 1.5\
**Status:** Open — remediation in progress  
**Source:** `02-AUDIT-REPORT.md`  
**Baseline commit:** `e026bdc5cc4a78dd80570f8c93d50008711de262`  
**Last verified:** 26 November 2026  
**Inspected branch:** `docs/archive-v1-and-fix-v2`\
**Inspected commit:** `f507e0d81cf5e4c85faee85a4b600a1fe2083202`\
**Inspected tree:** `997dc39107b5caec9447737ec9b1a4eb788d8ffc`\
**Inspection status:** Committed topic-branch snapshot; not yet merged into `main`.\
**Maintainer:** J-ART

---

## Purpose

This register tracks the corrective actions arising from the initial documentation audit of Framing Creativity Lab.

It records the current status of each finding, the decisions or dependencies required to resolve it, and the evidence supporting its status.

The original audit report and previous validation report are historical records. They must not be silently rewritten to reflect later repository changes.

A draft, recommendation, or locally prepared replacement is not a completed repository correction.

A finding may be marked **Resolved** only after the relevant document or configuration has been inspected on `main` and the correction has been verified.

### 1.5 Verification Scope

This version records a read-only validation of the committed topic-branch snapshot at `f507e0d81cf5e4c85faee85a4b600a1fe2083202`.

The eleven v1.0 documents are preserved under `docs/archives/` with their contents unchanged from the committed main baseline. Git detects all eleven moves as 100% renames.

The eleven v2.0 documents retain their Draft for Maintainer Review status. The README, archive index, audit index, and selected cross-document references have been reconciled. Relative Markdown links and committed whitespace checks passed.

This validation applies to the topic branch only. The branch has not been merged into `main`. Repository security settings, private reporting channels, policy approval, and effective dates have not been independently verified.

---

## 1. Status Vocabulary

| Status | Definition |
|---|---|
| Open | No substantive corrective implementation has been verified. |
| In progress | Corrective work has started, but required changes have not yet been fully applied and verified. |
| Partially resolved | Substantive corrective material exists, but approval, implementation, configuration, or validation remains incomplete. |
| Blocked — decision | An explicit maintainer decision is required before the corrective action can be completed. |
| Blocked — configuration | A repository setting, access control, or operational channel must be checked or configured. |
| Resolved | The relevant document or configuration has been inspected and the correction has been verified. |
| Accepted risk | The maintainer has explicitly accepted and documented the remaining risk. |
| Not applicable | The scope has materially changed. The rationale and approval must be recorded. |

A finding must not be marked Resolved merely because a replacement document has been drafted or uploaded.

A v2.0 document with the status `Draft for Maintainer Review` is evidence of remediation work, but it must not be represented as an approved or effective policy.

---

## 2. Findings Register

| Finding | Severity | Affected area | Required corrective action | Current status | Verification condition |
|---|---|---|---|---|---|
| AUD-001 | High | Documentation filenames and internal references | Preserve the v1.0 documents in the archive, use the `-v1.0.md` suffix, and ensure current v2.0 references resolve to the correct `.md` files. | **Partially resolved** | The eleven archived files were verified byte-for-byte against the base commit and renamed with the `-v1.0.md` suffix. Final cross-document and relative-link validation is still required. |
| AUD-002 | High | Project vocabulary and cross-document references | Maintain the proposed separation of Lifecycle Stage, Project Status, Technical Maturity, Operational Readiness, Publication Classification, and Publication Status across the v2.0 draft suite. | **Partially resolved** | The v2.0 drafts define the proposed separate dimensions. The README and selected cross-document references have been aligned with the v2.0 draft set. Complete validation and maintainer approval remain outstanding. |
| AUD-003 | High | `CONTRIBUTING-v2.0.md`, `PUBLICATION-POLICY-v2.0.md`, `GOVERNANCE-v2.0.md` | Establish clear permission requirements for the Lab to incorporate, reproduce, modify, maintain, distribute, and publish accepted external contributions. Preserve the intentional absence of a general repository licence. | **Partially resolved** | The v2.0 documents state that submission or acceptance does not transfer ownership or grant unrestricted rights. Required permissions must be established through an applicable licence or explicit written agreement. The documents still require approval, and the practical agreement process must be clear before external contributions are accepted. |
| AUD-004 | Medium | `SECURITY-v2.0.md`, `CODE-OF-CONDUCT-v2.0.md`, reporting channels | Verify GitHub Private Vulnerability Reporting and establish an accessible private conduct-reporting route. | **Blocked — configuration** | GitHub configuration must be checked. A private conduct-reporting method must be explicitly established and published. The v2.0 documents correctly state that neither channel has yet been verified as operational. |
| AUD-005 | Medium | `README.md`, documentation navigation, cross-document references | Identify the archived v1.0 documents and the v2.0 draft suite clearly. Validate relative links and the repository structure. | **Partially resolved** | The README now distinguishes the archived v1.0 baseline from the v2.0 draft suite, and the archive index lists all eleven historical documents. Relative-link and final tree validation remain outstanding. |
| AUD-006 | Medium | `PUBLICATION-POLICY-v2.0.md`, `RESPONSIBLE-AI-v2.0.md`, `PROJECT-TEMPLATE-v2.0.md`, `RESEARCH-METHODOLOGY-v2.0.md` | Use a consistent four-level data-classification model. Distinguish data classification from personal-data characteristics and AI Risk Classification. | **Partially resolved** | The v2.0 Publication Policy and Responsible AI Policy use Public, Internal, Confidential, and Restricted. Personal and sensitive information are treated as characteristics rather than additional classification values. The project template delegates to the applicable classification requirements. Approval and complete cross-document validation remain outstanding. |
| AUD-007 | Medium | `PUBLICATION-POLICY-v2.0.md`, `PROJECT-TEMPLATE-v2.0.md` | Clarify P1 controlled-publication conditions and formal P2/P3 reassessment requirements. Keep Publication Status separate from Publication Classification. | **Partially resolved** | The v2.0 Publication Policy defines mandatory P1 conditions and a documented P2 reassessment process. P3 is excluded from the public process. The v2.0 Project Template uses the canonical Publication Status values. Formal approval and complete consistency validation remain outstanding. |
| AUD-008 | Medium | Lifecycle, Quality Standards, Project Template, README | Separate Lifecycle Stage, Project Status, Technical Maturity, Operational Readiness, Publication Classification, and Publication Status. | **Partially resolved** | The v2.0 Lifecycle, Quality Standards, Publication Policy, Charter, and Project Template distinguish the six dimensions. The README and cross-document references still require alignment. |
| AUD-009 | Medium | Governance, Charter, Contributing, Security, Quality, Research, Responsible AI, Lifecycle, Project Template, README | Reduce duplicated policy content. Keep detailed requirements in their designated documents and use concise summaries and cross-references elsewhere. | **Partially resolved** | The v2.0 suite establishes separate policy responsibilities and more explicit cross-references. Some references still point to v1.0 documents, and a full consistency review is outstanding. |
| AUD-010 | Low | Metadata across policy and template documents | Apply a consistent document metadata convention. Distinguish drafts from approved policies and preserve historical dates. | **Partially resolved** | The eleven v2.0 documents inspected use a consistent metadata structure: Document ID, Version, Status, Effective Date, Maintainer, and Repository. Approval, effective dates, and the final audit metadata convention remain outstanding. |
| AUD-011 | Low | `PROJECT-TEMPLATE-v2.0.md` and public project documentation | Retain a comprehensive project template while establishing a shorter public project brief or project record where appropriate. Keep restricted assessment details outside public project records. | **Open** | The v2.0 template is shorter and modular compared with the original template, but a separate concise public project brief has not been verified in the repository. |

### 2.1 Current Finding Summary

This summary reflects the committed topic-branch snapshot at `f507e0d81cf5e4c85faee85a4b600a1fe2083202`. It is not a final audit verdict or evidence of approval of the v2.0 drafts.

| Status | Count | Findings |
|---|---:|---|
| Resolved | 0 | — |
| Partially resolved | 9 | AUD-001, AUD-002, AUD-003, AUD-005, AUD-006, AUD-007, AUD-008, AUD-009, AUD-010 |
| Blocked — configuration | 1 | AUD-004 |
| Open | 1 | AUD-011 |
| **Total** | **11** | |

---

## 3. Document Versioning and Authority

The maintainer has chosen to preserve the original v1.0 documents and manage the revised documents through separate versioned files.

This is the repository's intended documentation-management approach.

### 3.1 Versioning Model

The repository maintains two document sets:

**Original v1.0 documents**

The original files remain at their existing root paths. They are preserved as the earlier documentation baseline and must not be overwritten or deleted as part of the v2.0 review.

**Revised v2.0 documents**

The revised documents are maintained as separately named files with the `-v2.0.md` suffix.

They are currently marked `Draft for Maintainer Review`, with their effective dates pending approval.

Their presence does not automatically make them approved or effective policies.

### 3.2 Root-Level v2.0 Documentation Set

The following eleven versioned documents were verified in the root of the repository at the inspected commit.

| Document | Blob SHA (short) | Status |
|---|---|---|
| `LAB-CHARTER-v2.0.md` | `b341bf75` | Draft for Maintainer Review |
| `GOVERNANCE-v2.0.md` | `d52bec57` | Draft for Maintainer Review |
| `PROJECT-LIFECYCLE-v2.0.md` | `81fb6be9` | Draft for Maintainer Review |
| `PROJECT-TEMPLATE-v2.0.md` | `a31c5b76` | Draft for Maintainer Review |
| `QUALITY-STANDARDS-v2.0.md` | `a09e3222` | Draft for Maintainer Review |
| `RESEARCH-METHODOLOGY-v2.0.md` | `b135d91e` | Draft for Maintainer Review |
| `PUBLICATION-POLICY-v2.0.md` | `496d097b` | Draft for Maintainer Review |
| `RESPONSIBLE-AI-v2.0.md` | `f7a3c8ff` | Draft for Maintainer Review |
| `CONTRIBUTING-v2.0.md` | `ef043907` | Draft for Maintainer Review |
| `SECURITY-v2.0.md` | `f349bf32` | Draft for Maintainer Review |
| `CODE-OF-CONDUCT-v2.0.md` | `6cd76f3e` | Draft for Maintainer Review |

### 3.3 Version 1.0 Preservation

The original root-level documents remain in place:

- `LAB-CHARTER.md`
- `GOVERNANCE.md`
- `PROJECT-LIFECYCLE.md`
- `PROJECT-TEMPLATE.md`
- `QUALITY-STANDARDS.md`
- `RESEARCH-METHODOLOGY.md`
- `PUBLICATION-POLICY.md`
- `RESPONSIBLE-AI.md`
- `CONTRIBUTING.md`
- `SECURITY.md`
- `CODE-OF-CONDUCT.md`

These files must not be overwritten, deleted, or silently repurposed as part of the versioned-document approach.

The README must clearly distinguish the retained v1.0 documents from the v2.0 drafts under review.

### 3.4 Approval Boundary

The v2.0 documentation set remains subject to maintainer review.

Before any document is treated as an effective replacement or current policy, its approval status and effective date must be established.

The repository must not imply that a draft policy has superseded an earlier document solely because its filename contains `v2.0`.

---

## 4. Proposed Canonical Project Vocabulary — v2.0 Draft

The proposed v2.0 framework separates six independent project dimensions. These definitions remain subject to maintainer review and are not approved policy.

The v2.0 documents define the following values.

| Dimension | Canonical values | Proposed authoritative v2.0 document |
|---|---|---|
| Lifecycle Stage | Idea and Intake; Proposal; Discovery and Feasibility; Experimentation and Development; Validation and Evaluation; Publication Review; Publication and Release; Maintenance and Evolution; Archival or Discontinuation | `PROJECT-LIFECYCLE-v2.0.md` |
| Project Status | Proposed; Concept; Experimental; Prototype; Development; Validation; Published; Maintenance; Archived; Discontinued | `PROJECT-LIFECYCLE-v2.0.md` |
| Technical Maturity | Not Assessed; Exploratory; Prototype; Validated | `QUALITY-STANDARDS-v2.0.md` |
| Operational Readiness | Not Assessed; Research or Experimental Use Only; Demonstration Only; Limited Operational Use; Production-Oriented | `QUALITY-STANDARDS-v2.0.md` |
| Publication Classification | P0; P1; P2; P3 | `PUBLICATION-POLICY-v2.0.md` |
| Publication Status | PENDING; APPROVED; REJECTED; WITHDRAWN | `PUBLICATION-POLICY-v2.0.md` |

These dimensions answer different questions:

- **Lifecycle Stage** identifies the project's position in the Lab's workflow.
- **Project Status** describes the current state of the project.
- **Technical Maturity** describes the maturity of the technical work and the evidence supporting it.
- **Operational Readiness** describes the operating context for which the work has been assessed.
- **Publication Classification** determines the applicable publication scrutiny and restrictions.
- **Publication Status** records the publication review state or decision.

They must not be merged into one status field or treated as interchangeable values.

### 4.1 AI Risk Classification

AI Risk Classification is a separate framework governed by `RESPONSIBLE-AI-v2.0.md`.

Its A0–A4 values must not be confused with Publication Classification P0–P3.

### 4.2 Data Classification

The v2.0 Publication Policy and Responsible AI Policy use the same four data classification values:

- Public
- Internal
- Confidential
- Restricted

Personal information and sensitive information are characteristics of data, not additional values in this classification framework.

Personal information should be classified at least as Confidential. Sensitive personal information, security-critical information, or information subject to stricter restrictions should be classified as Restricted.

### 4.3 Research Evidence Categories

Research Evidence Categories E0–E5 are a separate descriptive evidence framework defined in `RESEARCH-METHODOLOGY-v2.0.md`.

They are not Project Status, Technical Maturity, or Operational Readiness values.

---

## 5. Verified Repository State

The following repository state was inspected:

**Repository:** `framingcreativity/framing-creativity-lab`  
**Branch:** `docs/archive-v1-and-fix-v2`\
**Commit:** `f507e0d81cf5e4c85faee85a4b600a1fe2083202`\
**Tree:** `997dc39107b5caec9447737ec9b1a4eb788d8ffc`\
**Verification date:** 26 November 2026\
**Inspection mode:** Read-only inspection of committed topic-branch snapshot

### 5.1 Root Documentation

The working tree contains the eleven v2.0 draft documents at the repository root and the eleven original v1.0 documents under `docs/archives/`.

The README and archive index have been updated to distinguish the two documentation sets. Final relative-link validation and committed-state verification remain outstanding.

### 5.2 Lifecycle Filename

The v2.0 lifecycle document is now correctly named:

`PROJECT-LIFECYCLE-v2.0.md`

The rename was committed in:

`1728c382648ac1f41ed129f8a19709e1ba8650d2`

The earlier filename without the `.md` extension is no longer the current root path.

### 5.3 Audit Archive

The following audit records are present:

- `docs/audits/README.md`
- `docs/audits/FCL-DOC-AUDIT-2026-001/00-AUDIT-RECORD.md`
- `docs/audits/FCL-DOC-AUDIT-2026-001/01-MASTER-PROMPT.md`
- `docs/audits/FCL-DOC-AUDIT-2026-001/02-AUDIT-REPORT.md`
- `docs/audits/FCL-DOC-AUDIT-2026-001/03-REMEDIATION-REGISTER.md`
- `docs/audits/FCL-DOC-AUDIT-2026-001/04-POST-REMEDIATION-VALIDATION-PROMPT.md`
- `docs/audits/FCL-DOC-AUDIT-2026-001/05-README-INTEGRATION-SNIPPET.md`
- `docs/audits/FCL-DOC-AUDIT-2026-001/06-POST-REMEDIATION-VALIDATION-2026-11-26.md`

The original audit record, report, and validation report are historical records. They must not be overwritten to describe later repository states.

### 5.4 Outstanding Navigation and Reference Issues

The current README still lists the v1.0 files as the main documentation library.

Several v2.0 documents also contain references to unversioned document paths, including references to v1.0 files where a v2.0 counterpart exists.

Examples include cross-references in the v2.0 Governance, Charter, Project Template, Quality Standards, and Publication Policy documents.

These references must be reviewed during the final consistency and link-validation stage.

A link that resolves to a valid v1.0 file is not necessarily semantically correct when the intended reference is the v2.0 draft.

The final validation must distinguish between:

- A broken relative link.
- A valid link to a historical or v1.0 document.
- A reference that should point to the v2.0 document.
- A deliberately retained reference to a file without a v2.0 counterpart.

The absence of a separate concise public project brief also remains to be addressed under AUD-011.

---

## 6. Evidence Log

Historical evidence must remain intact. New entries are added chronologically.

| Date | Finding | Action / evidence | Commit or reference | Result |
|---|---|---|---|---|
| 2026-11-25 | Baseline | Initial documentation audit performed against the baseline repository state. | `e026bdc5cc4a78dd80570f8c93d50008711de262` | Baseline recorded |
| 2026-11-25 | Audit archive | Audit report, master prompt, register, validation prompt, and archive index added. | `386a3ac3e7cbfc70eb40226d4d1ce1e06af2606c` | Archive present |
| 2026-11-25 | AUD-001 | Corrected malformed filenames to `QUALITY-STANDARDS.md` and `RESPONSIBLE-AI.md`. | `c073e881e7c9fc3d7e17f2c735b703d6be23e745` | Verified — Resolved |
| 2026-11-25 | AUD-002 / AUD-008 | Added the Lifecycle Stage and Project Status distinction and references to separate maturity, readiness, and publication dimensions. | `216ce2ac33a2e14a2959fa54bb2cf9f8abd5c890` | Partially implemented |
| 2026-11-25 | AUD-008 | Added a Quality Standards v2.0 draft as a separate root file. The canonical v1.0 file was preserved. | `b711dbdbd9de7f58f8915a988ef6f8e33daae6d1` | Draft only |
| 2026-11-25 | AUD-009 | Added Governance and Lab Charter v2.0 drafts as separate root files. | `cf76ad7b86c95c331f1e3520db9ec95b25e85706`; `585a4f2eb3acaab9fbe3470fb49d650eda1d4878` | Drafts only |
| 2026-11-26 | AUD-001–AUD-011 | Read-only post-remediation validation completed against the then-current repository state. | Inspected commit: `b0a71f618cde4b75459b1094f80a30eec5a71543` | Historical result: 1 Resolved; 3 Partially resolved; 3 Blocked; 4 Open |
| 2026-11-26 | Validation archive | Post-remediation validation report renamed and archived under the audit folder. | `419f36d37c3189a4afa3841281c264805b6d38ca` | Report present |
| 2026-11-26 | Audit index | Added a link to the post-remediation validation report in `docs/audits/README.md`. | `bd39a2020b4f0bbe18bb93d822d45b9085ce5d63` | Index updated |
| 2026-11-26 | Lifecycle filename | Renamed the v2.0 Lifecycle document to include the `.md` extension. | `1728c382648ac1f41ed129f8a19709e1ba8650d2` | Verified — Resolved |
| 2026-11-26 | AUD-003 | Added `CONTRIBUTING-v2.0.md` with explicit requirements for permissions to incorporate, reproduce, modify, distribute, and publish external contributions. | `226dbdab0532e1a6ab7cc394c1e217dbf196b69b` | Draft added — approval and practical agreement process remain outstanding |
| 2026-11-26 | AUD-004 | Added `SECURITY-v2.0.md` with conditional private vulnerability reporting and explicit disclosure of unverified configuration status. | `f86742b0f0beceea61a14e27450b15af2c1d4134` | Draft added — configuration not verified |
| 2026-11-26 | AUD-004 | Added `CODE-OF-CONDUCT-v2.0.md` with explicit disclosure that a private conduct-reporting route has not been verified. | `417b114874d17e64f5d86c3bcb071cdcff13834f` | Draft added — private route not established |
| 2026-11-26 | AUD-002–AUD-011 | Inspected the eleven v2.0 documents, README, audit index, remediation register, and repository tree on `main`. | `417b114874d17e64f5d86c3bcb071cdcff13834f` | Current checkpoint recorded; complete validation still required |
| 2026-11-26 | AUD-005 | Confirmed that a README documentation index exists, but it still primarily describes the v1.0 document set. | README blob `3abf99c0` | Partially resolved |
| 2026-11-26 | AUD-006 / AUD-007 / AUD-008 | Verified the data classification, P1/P2/P3 publication rules, six project dimensions, and separate AI Risk Classification in the v2.0 document set. | v2.0 document blobs listed in Section 3.2 | Partially resolved pending approval and cross-document validation |
| 2026-11-26 | AUD-010 | Verified consistent metadata fields across the eleven v2.0 documents. | v2.0 document blobs listed in Section 3.2 | Partially resolved pending approval and final metadata review |
| 2026-11-26 | Register | Updated the remediation register to reflect the versioned v2.0 document strategy and the latest inspected repository state. | Current register Version 1.3 | Updated checkpoint |

| 2026-11-26 | AUD-001 / AUD-002 / AUD-005 / AUD-008 / AUD-009 | Committed the archive migration, README and audit-index corrections, archive index, and v2.0 cross-reference reconciliation. | `f507e0d81cf5e4c85faee85a4b600a1fe2083202` | Topic-branch commit; validation report 07 added; merge pending |

Add a dated row for every subsequent material change.

Each new evidence entry should identify:

- The finding affected.
- The canonical or versioned file changed.
- The commit or configuration reference.
- The verification performed.
- The resulting status.

A draft upload must be recorded as a draft, not as a resolved finding.

---

## 7. Remediation Sequence

The following sequence reflects the selected v1.0 preservation and v2.0 versioning approach.

1. Complete the supporting v2.0 documentation set and verify that all eleven versioned files remain present at their intended root paths.

2. Review and reconcile cross-document references so that each v2.0 document points to the intended v2.0 counterpart where one exists. Preserve deliberate references to supporting files that remain at their original paths.

3. Update `README.md` to explain the versioning model, distinguish the preserved v1.0 documents from the v2.0 drafts, and provide an accurate documentation index and repository structure.

4. Clarify the practical permission and agreement process for external contributions under AUD-003. Do not introduce a general open-source licence. The required permissions must be established explicitly for the intended use of each accepted contribution.

5. Verify GitHub Private Vulnerability Reporting and establish the private conduct-reporting channel under AUD-004. Record the actual configuration and confirm that the channels are usable before describing them as operational.

6. Decide whether a separate concise public project brief is required under AUD-011. Keep restricted internal assessments outside public project records.

7. Review the v2.0 documents as a coherent policy suite. Confirm the policy ownership boundaries, metadata convention, publication requirements, data classification, project vocabulary, and governance responsibilities.

8. Resolve remaining cross-document duplication, inconsistent terminology, outdated references, and any missing or misleading navigation.

9. Establish the approval and effective-date decisions for the v2.0 documents. Until then, retain their `Draft for Maintainer Review` status.

10. Perform the complete read-only post-remediation validation against the actual `main` branch. Record the inspected commit and produce a new dated validation report without overwriting the previous report.

---

## 8. Completion Rule

The audit is not closed merely because replacement documents have been drafted or uploaded.

A finding may be marked Resolved only after validation confirms that:

- The relevant file exists at the intended repository path on `main`.
- The file content and metadata are correct.
- The v1.0 preservation and v2.0 versioning approach is represented accurately.
- Cross-references and relative links resolve and point to the intended version.
- Authoritative definitions are consistent across dependent documents.
- The requirements of the relevant finding have been satisfied.
- Required repository settings and reporting channels have actually been verified.
- No private, proprietary, confidential, or otherwise unauthorized material has been introduced.
- The evidence log contains the relevant commit or configuration reference and a reproducible verification note.

The audit may be closed only when every finding is one of the following:

- Resolved.
- Accepted risk, with explicit maintainer approval and rationale.
- Not applicable, with explicit justification and maintainer approval.

The final validation must be based on the actual repository state, not on draft files, earlier summaries, or assumed completion.

---

**Framing Creativity Lab**  
Independent Research · Applied AI · Creative Technology · Experimental Design

**Maintainer:** J-ART
