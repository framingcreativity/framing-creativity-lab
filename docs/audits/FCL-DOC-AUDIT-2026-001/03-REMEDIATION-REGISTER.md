# Remediation Register — FCL-DOC-AUDIT-2026-001

**Document ID:** FCL-AUD-REG-001  
**Version:** 1.1  
**Status:** Open — remediation in progress  
**Source:** `02-AUDIT-REPORT.md`  
**Baseline commit:** `e026bdc5cc4a78dd80570f8c93d50008711de262`  
**Last verified:** 25 November 2026  
**Maintainer:** J-ART

> This register records the status of the original documentation-audit findings. A draft, recommendation, or locally prepared
replacement is not a completed repository correction. A finding may be marked **Resolved** only after the canonical file or setting
has been inspected on `main` and the evidence has been recorded.

## 1. Status vocabulary

- **Open:** no corrective implementation has been verified on `main`.
- **In progress:** implementation or drafting has started, but the canonical change is not yet fully applied and verified.
- **Blocked — decision:** an explicit maintainer decision is required before the corrective action can be completed.
- **Blocked — configuration:** a repository setting, access control, or operational channel must be checked or configured.
- **Resolved:** the canonical file or configuration has been inspected and the correction has been verified.
- **Accepted risk:** the maintainer has explicitly accepted and documented the remaining risk.
- **Not applicable:** the scope has materially changed; rationale and approval must be recorded.

## 2. Findings register

| Finding | Severity | Affected area | Required corrective action | Current status | Verification condition |
|---|---|---|---|---|---|
| AUD-001 | High | `QUALITY-STANDARDS.md.` and `RESPONSIBLE-AI.md.` | Keep the corrected filenames at the exact canonical `.md`
paths and verify internal references and repository links. | **Resolved** | Both canonical paths exist on `main`; neither malformed
dotted filename remains. Verified by commit `c073e881e7c9fc3d7e17f2c735b703d6be23e745`. |
| AUD-002 | High | README, Charter, Governance, Lifecycle, Quality, Project Template | Apply the approved vocabulary consistently.
`PROJECT-LIFECYCLE.md` owns the nine Lifecycle Stages and ten Project Status values. Other fields must remain distinct and point to
their authoritative documents. | **In progress** | Lifecycle/Status distinction was committed in `PROJECT-LIFECYCLE.md`; the
remaining canonical documents still require alignment and cross-reference validation. |
| AUD-003 | High | `CONTRIBUTING.md`, `PUBLICATION-POLICY.md`, repository licensing | Define the permission or licence terms under
which the Lab may incorporate, modify, maintain, and distribute accepted external contributions. Preserve the intentional absence of
a general repository licence unless a separate decision changes it. | **Blocked — decision** | An explicit maintainer decision is
recorded; contribution and publication terms agree; no rights are inferred from submission alone. Legal review should be considered
where appropriate. |
| AUD-004 | Medium | `SECURITY.md`, `CODE-OF-CONDUCT.md`, reporting channels | Verify whether GitHub Private Vulnerability Reporting
is enabled. Establish an actual private route for conduct reports. Do not describe conditional or unpublished channels as
operational. | **Blocked — configuration** | Repository setting is checked and recorded; reporting routes are usable and accurately
described in the relevant policies. Current public documentation makes the security route conditional on enablement; actual
configuration has not been verified in this audit. |
| AUD-005 | Medium | `README.md`, cross-document references | Add a useful documentation index with working relative links and
validate references between authoritative documents. | **In progress** | A replacement README has been prepared, but the canonical
`README.md` on `main` remains unchanged. Verify links after the replacement is applied. |
| AUD-006 | Medium | `PUBLICATION-POLICY.md`, `RESPONSIBLE-AI.md`, `PROJECT-TEMPLATE.md` | Adopt and use a consistent data
classification model. Clearly distinguish information classification from personal-data status and AI risk classification. |
**Open** | The same approved terms and definitions appear in the authoritative policies and the project template, with no
contradictory labels. |
| AUD-007 | Medium | `PUBLICATION-POLICY.md`, `PROJECT-TEMPLATE.md` | Clarify the requirements and approval conditions for P1
controlled publication. Require documented resolution, formal reclassification, and renewed review before any P2/P3 material can be
reconsidered. | **Blocked — decision** | The maintainer approves explicit P1 release conditions and P2/P3 reassessment rules; the
policy and template reflect the same process. |
| AUD-008 | Medium | `QUALITY-STANDARDS.md`, `PROJECT-TEMPLATE.md`, `README.md`, `PROJECT-LIFECYCLE.md` | Separate Lifecycle Stage,
Project Status, Technical Maturity, Operational Readiness, Publication Classification, and Publication Status. Do not treat
technical maturity or public availability as evidence of production readiness. | **In progress** | Lifecycle/Status separation is
present in `PROJECT-LIFECYCLE.md`. A Quality Standards v2.0 draft exists as a separate root file, but it has not replaced `QUALITY-STANDARDS.md`; the project template and README also remain to be aligned. |
| AUD-009 | Medium | README, Charter, Governance, Contributing, Security, Quality, Research, Responsible AI, Lifecycle, Template | Reduce repeated policy text. Keep detailed requirements in their designated authoritative documents and use concise summaries and links elsewhere. | **In progress** | Full replacement drafts have been prepared for several core documents. They must be applied to their canonical paths and checked together before this finding can be resolved. |
| AUD-010 | Low | Metadata across policy and template documents | Establish a consistent metadata convention for document ID, version, status, effective or revision date, and maintainer. Preserve meaningful historical dates and distinguish draft status from approved policy status. | **Open** | A metadata convention is approved and consistently applied to the in-scope documents. |
| AUD-011 | Low | `PROJECT-TEMPLATE.md` | Retain a comprehensive internal master template while providing a shorter public project record or brief. Do not expose restricted review details in public project documentation. | **In progress** | A shorter replacement template has been prepared; it has not yet replaced the canonical `PROJECT-TEMPLATE.md`. The public/internal documentation boundary still needs to be checked. |

## 3. Approved canonical vocabulary

The maintainer approved the following separation of project dimensions. Their definitions must be maintained in the authoritative documents rather than independently redefined in every file.

| Dimension | Canonical values | Authoritative document |
|---|---|---|
| Lifecycle Stage | Idea and Intake; Proposal; Discovery and Feasibility; Experimentation and Development; Validation and Evaluation; Publication Review; Publication and Release; Maintenance and Evolution; Archival or Discontinuation | `PROJECT-LIFECYCLE.md` |
| Project Status | Proposed; Concept; Experimental; Prototype; Development; Validation; Published; Maintenance; Archived; Discontinued | `PROJECT-LIFECYCLE.md` |
| Technical Maturity | Not Assessed; Exploratory; Prototype; Validated | `QUALITY-STANDARDS.md` |
| Operational Readiness | Not Assessed; Research or Experimental Use Only; Demonstration Only; Limited Operational Use; Production-Oriented | `QUALITY-STANDARDS.md` |
| Publication Classification | P0; P1; P2; P3 | `PUBLICATION-POLICY.md` |
| Publication Status | PENDING; APPROVED; REJECTED; WITHDRAWN | `PUBLICATION-POLICY.md` |

These dimensions answer different questions. They must not be merged into a single status field or treated as interchangeable levels. AI Risk Classification is a separate subject governed by `RESPONSIBLE-AI.md` and must not be confused with the publication classification.

## 4. Verified repository state

The following canonical files were read from the default branch `main` during the latest read-only check on 25 November 2026:

| Canonical path | Observed state | Blob SHA (short) |
|---|---|---|
| `QUALITY-STANDARDS.md` | Version 1.0; not yet replaced by the v2.0 draft | `5cf468c4` |
| `PROJECT-TEMPLATE.md` | Version 1.0; not yet replaced by the prepared v2.0 draft | `1eb19040` |
| `README.md` | Existing README; prepared replacement not yet applied | `f2be2073` |
| `GOVERNANCE.md` | Version 1.0; prepared replacement not yet applied | `352806a5` |
| `LAB-CHARTER.md` | Version 1.0; prepared replacement not yet applied | `9e7b5d0d` |
| `PROJECT-LIFECYCLE.md` | Version 1.0 with canonical Lifecycle Stage / Project Status distinction added | `3cc79c43` |
| `03-REMEDIATION-REGISTER.md` | Version 1.0; this v1.1 replacement is not yet applied | `462c73de` |

**Draft-file caution:** `QUALITY-STANDARDS-v2.0-FULL-REWRITE.md` is present at the repository root as a separate draft file (added by commit `b711dbdbd9de7f58f8915a988ef6f8e33daae6d1`). It is not the canonical `QUALITY-STANDARDS.md`. After the canonical replacement is applied and verified, remove this duplicate root draft or relocate it deliberately to an appropriate archive location. Do not leave two competing files that appear to be the current standard.

## 5. Evidence log

| Date | Finding | Action / evidence | Commit or reference | Result |
|---|---|---|---|---|
| 2026-11-25 | Baseline | Initial audit performed against the baseline repository state. | `e026bdc5cc4a78dd80570f8c93d50008711de262` | Baseline recorded |
| 2026-11-25 | Audit archive | Audit report, prompt, register, validation prompt, and archive index added. | `386a3ac3e7cbfc70eb40226d4d1ce1e06af2606c` | Archive present |
| 2026-11-25 | AUD-001 | Corrected malformed filenames to `QUALITY-STANDARDS.md` and `RESPONSIBLE-AI.md`. | `c073e881e7c9fc3d7e17f2c735b703d6be23e745` | **Verified — Resolved** |
| 2026-11-25 | AUD-002 / AUD-008 | Added canonical Lifecycle Stage and Project Status distinction and references to separate maturity, readiness, and publication dimensions. | `216ce2ac33a2e14a2959fa54bb2cf9f8abd5c890` | **Partially implemented — In progress** |
| 2026-11-25 | AUD-008 | Added a v2.0 Quality Standards draft as a separate file; canonical file was not replaced. | `b711dbdbd9de7f58f8915a988ef6f8e33daae6d1` | Draft only — not a canonical correction || 2026-11-26 | AUD-001–AUD-011 | Read-only post-remediation validation completed. | Inspected commit: `b0a71f618cde4b75459b1094f80a30eec5a71543`; report: `06-POST-REMEDIATION-VALIDATION-2026-11-26.md` | Read-only validation | 1 Resolved; 3 Partially resolved; 3 Blocked; 4 Open |

Add a dated row for each subsequent material change. Include the commit SHA, the canonical path affected, and the verification
performed. A draft upload must be recorded as a draft, not as a resolved finding.

## 6. Remediation sequence

1. Replace `QUALITY-STANDARDS.md` with its prepared v2.0 content. Verify the canonical path, metadata, tables, links, and all six
project dimensions. Then remove or relocate the separate root draft file.
3. Replace `PROJECT-TEMPLATE.md` with its prepared v2.0 content. Verify that the project record uses the canonical field names and
values.
4. Replace `README.md` with its prepared v2.0 content. Verify the documentation index and every relative link.
5. Apply the prepared `GOVERNANCE.md` and `LAB-CHARTER.md` replacements. Check that the Charter states principles while Governance
defines operational authority and processes.
6. Resolve the contribution-rights and P1/P2/P3 publication decisions before changing AUD-003 or AUD-007 to Resolved.
7. Verify private security and conduct reporting settings and channels before changing AUD-004 to Resolved.
8. Harmonise data classification and document metadata, then check for duplicated policy text and conflicting terminology across the
9. full in-scope set.
10. Run the post-remediation validation prompt and record its findings before closing the audit.

## 7. Completion rule

The audit is not closed merely because replacement documents have been drafted or uploaded under alternate filenames. A finding
maybe closed only after read-only validation confirms that:

- the correction is present at the canonical repository path on `main`;
- cross-references and relative links resolve;
- authoritative definitions are consistent across dependent documents;
- no contradictory terminology remains within the finding's scope;
- required settings or reporting channels have actually been verified;
- no private, proprietary, or otherwise unauthorised material has been introduced; and
- the evidence log contains the relevant commit or configuration reference and a reproducible verification note.

The audit may be closed only when every finding is Resolved, Accepted risk, or Not applicable with an explicit rationale and
maintainer approval.
