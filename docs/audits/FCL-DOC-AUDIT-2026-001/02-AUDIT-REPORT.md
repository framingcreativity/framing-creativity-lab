# Framing Creativity Lab — Comprehensive Documentation Audit

**Audit scope:** Twelve foundational documentation files  
**Repository:** `framingcreativity/framing-creativity-lab`  
**Branch:** `main`  
**Audited commit:** `e026bdc5cc4a78dd80570f8c93d50008711de262`  
**Commit date:** 25 November 2026  
**Maintainer identified in the documents:** J-ART  
**Audit mode:** Read-only; no repository files, settings, branches, or Git history were modified.

---

## 1. Executive Summary

### Overall verdict

<ins>**CONDITIONALLY READY — corrections required before presenting the twelve files as a complete, coherent documentation framework.**</ins>

The public repository contains all twelve intended documents. The framework has a strong conceptual foundation: the Lab is consistently presented as an independent, founder-led research and experimentation initiative; confidentiality and publication are treated seriously; experimental maturity is not equated with production readiness; and the documents generally avoid inventing an institutional structure or promising unrealistic service levels.

The main weaknesses are not a lack of policy content. They are **document identity, cross-document taxonomy, contributor rights, and operational readiness**.

The most important findings are:

1. **Two filenames end with an accidental trailing period.** The repository contains `QUALITY-STANDARDS.md.` and `RESPONSIBLE-AI.md.` rather than the expected `QUALITY-STANDARDS.md` and `RESPONSIBLE-AI.md`. References elsewhere use the filenames without the final period, so they do not resolve to the actual paths.
2. **Project lifecycle stages, project statuses, and quality levels are not consistently separated.** The README, Charter, Governance document, Project Lifecycle, Quality Standards, and Project Template use overlapping vocabularies for different concepts.
3. **The contribution terms do not clearly grant the Lab permission to use accepted external contributions.** The repository intentionally has no general open-source licence, and contributors retain their rights, but the documents do not establish the specific licence or permission under which accepted contributions may be incorporated and distributed.
4. **Private reporting channels are described conditionally but not made discoverable.** The Security Policy depends on GitHub Private Vulnerability Reporting being enabled or on a separately published contact route. The Code of Conduct similarly requires a published private route. The feature's configuration was not verified during this audit.
5. **The documentation is difficult to navigate.** No Markdown links to the other `.md` files were found in the twelve files. The README does not provide a document index.

The documents are individually substantial and mostly well written. Collectively, however, they are too repetitive in several places and do not yet establish one authoritative vocabulary for status, maturity, publication, and data classification.

### Framework score

<ins>**3.7 / 5 — Strong foundation; not yet fully coherent or operational.**</ins>

This score reflects the actual public files at the audited commit, not the earlier drafts in conversation. It is not a legal, security, or compliance certification.

### Finding counts

| Severity | Count | Meaning |
|---|---:|---|
| Critical | 0 | No confirmed critical defect in the inspected documentation |
| High | 3 | Must be resolved before treating the framework as publication-ready |
| Medium | 6 | Material consistency or operational improvements required |
| Low | 2 | Editorial and usability improvements |
| **Total** | **11** | |

No private or proprietary project content was accessed or used. This audit cannot establish whether files outside this public repository contain confidential information; it is limited to the public repository requested.

---

## 2. Repository and Document Inventory

The public repository and its `main` branch were accessible. The recursive Git tree was complete and not truncated. The tree contained exactly the twelve expected document contents at the repository root, but two paths had an unexpected final dot.

| # | Actual repository path | Document ID | Version | Lines | Score | Assessment |
|---:|---|---|---|---:|---:|---|
| 1 | `README.md` | — | — | 517 | 3.2/5 | Strong identity statement; needs document navigation and less policy duplication |
| 2 | `LAB-CHARTER.md` | FCL-GOV-001 | 1.0 | 842 | 3.7/5 | Good foundational principles; overly broad and duplicates operational policies |
| 3 | `PUBLICATION-POLICY.md` | FCL-POL-001 | 1.0 | 1,057 | 4.0/5 | Strong publication controls; clarify P1/P3 and data taxonomy |
| 4 | `RESEARCH-METHODOLOGY.md` | FCL-METH-001 | 1.0 | 1,474 | 4.1/5 | Strongest methodological document; long and overlaps with adjacent policies |
| 5 | `CONTRIBUTING.md` | FCL-CONTRIB-001 | 1.0 | 1,025 | 3.3/5 | Detailed workflow; accepted contribution permissions remain unclear |
| 6 | `SECURITY.md` | FCL-SEC-001 | 1.0 | 597 | 3.5/5 | Responsible and realistic; reporting channel not yet demonstrably operational |
| 7 | `CODE-OF-CONDUCT.md` | FCL-GOV-002 | 1.0 | 497 | 3.7/5 | Clear, proportionate, and honest about single-maintainer limitations |
| 8 | `GOVERNANCE.md` | FCL-GOV-003 | 1.0 | 799 | 3.8/5 | Realistic founder-led model; duplicates lifecycle and status definitions |
| 9 | `PROJECT-LIFECYCLE.md` | FCL-PROC-001 | 1.0 | 1,058 | 4.2/5 | Clear lifecycle process; should become the single owner of lifecycle vocabulary |
| 10 | `QUALITY-STANDARDS.md.` | FCL-STD-001 | 1.0 | 1,207 | 4.0/5 | Good technical standards; “quality levels” mix quality, release, and operational readiness |
| 11 | `RESPONSIBLE-AI.md.` | FCL-AI-001 | 1.0 | 1,511 | 3.8/5 | Comprehensive internal AI policy; long and overlaps with Security, Research, and Quality |
| 12 | `PROJECT-TEMPLATE.md` | FCL-TPL-001 | 1.0 | 1,083 | 3.4/5 | Thorough but heavy; its lifecycle-stage field combines stages and statuses |

**Important path distinction:** the two trailing-dot files are present in the Git tree. Fetching the intended names without the dot returns 404. They are therefore not missing documents; they are misnamed documents.

### Repository observations

- All twelve files are at the repository root.
- No additional documentation folders or project folders appear in the audited tree.
- The README explicitly describes the proposed folder structure as an organisational direction to be introduced progressively. This is accurate and is not a defect.
- No `LICENSE` file is present. The README explicitly says there is no general open-source licence and that public visibility does not grant reuse rights. This appears intentional and should not be changed without a deliberate licensing decision.
- No `ATTRIBUTIONS.md` file is present. The Publication Policy recommends such a file where substantial third-party material is used; it does not make it a mandatory repository-wide document.
- The Git tree contains exactly these twelve files; no internal `.md` links were found by scanning the Markdown link syntax across the files.

---

## 3. Individual Document Audit

### 3.1 `README.md` — 3.2/5

**Strengths**
- Communicates a coherent identity, mission, research scope, and multidisciplinary direction.
- Clearly distinguishes the Lab from private and proprietary development environments.
- States that the repository has no general open-source licence and explains the effect of that decision.
- Describes the planned directory structure as progressive rather than claiming that the folders already exist.

**Weaknesses and corrections**
- It has no document index or links to the eleven supporting policies. This weakens its role as the repository entry point.
- Section 12 uses `Research`, `Exploration`, `Prototype`, `Experimental`, `Validated`, `Stable`, and `Archived`, which differs from the Project Lifecycle status vocabulary.
- Sections on methodology, AI experimentation, technical quality, experiment documentation, and confidentiality repeat detailed material owned by other documents.
- At 517 lines, it is unusually long for an entry-point README.

**Recommendation:** retain the identity, mission, research domains, operating principles, repository roadmap, and short confidentiality/licensing summary. Replace detailed policy duplication with a concise documentation index linking to the authoritative files.

### 3.2 `LAB-CHARTER.md` — 3.7/5

**Strengths**
- Explicitly establishes independence and avoids claiming the Lab is a company, formal research institution, or subsidiary.
- Clearly defines founder-led governance and does not invent a board or committee.
- Provides strong principles for confidentiality, intellectual property, and intentional publication.
- Correctly states that publication is separate from technical completion.

**Weaknesses and corrections**
- The Charter contains operational versions of the research methodology, publication policy, IP rules, AI policy, engineering standards, contribution principles, and project lifecycle.
- Section 7 maturity labels repeat the README vocabulary and conflict with the Project Lifecycle document.
- Section 16 supplies a separate lifecycle table (`Proposed`, `Research`, `Exploration`, `Development`, `Prototype`, `Evaluation`, `Published`, `Maintained`, `Archived`) that does not match the canonical lifecycle in `PROJECT-LIFECYCLE.md`.

**Recommendation:** keep the Charter constitutional: identity, independence, mission, foundational principles, governance authority, and policy hierarchy. Replace detailed operational procedures with references to the dedicated policies.

### 3.3 `PUBLICATION-POLICY.md` — 4.0/5

**Strengths**
- Strong publication workflow and review gates.
- Detailed treatment of ownership, third-party licences, Git history, repository metadata, credentials, privacy, technical validation, release management, and withdrawal.
- Correctly states that publication approval is scoped to reviewed material and that later material changes can trigger a new review.
- Avoids claiming privacy or legal compliance without a basis.

**Weaknesses and corrections**
- P1 (`Controlled publication`) needs an explicit rule stating whether and under what conditions P1 material may be publicly released. The Project Template says P1 is not “public-ready,” which is not necessarily the same as “not publishable.”
- P3 is described as non-publishable, but Section 4.2 says certain ineligible materials must not be published “without a separate, documented and valid authorisation.” Clarify that a genuine rights or permission change must trigger reclassification and a fresh review; P3 must not be bypassed by informal exception.
- Section 10.1 lists `Personal` as a data classification alongside `Public`, `Internal`, `Confidential`, and `Sensitive or restricted`. The Responsible AI Policy and Project Template use a different four-category scheme.
- The document recommends `ATTRIBUTIONS.md` or an equivalent file when substantial third-party material is used; this is a project-level recommendation, not a missing global file.

**Recommendation:** make classification, publication decision, and permission status three clearly separate concepts. Establish a shared data classification vocabulary.

### 3.4 `RESEARCH-METHODOLOGY.md` — 4.1/5

**Strengths**
- Strong research question, context, hypothesis, design, execution, evaluation, interpretation, and review sequence.
- Good treatment of variables, baselines, deviations, source traceability, and negative or inconclusive results.
- AI research requirements appropriately cover model identification, prompting, configuration, human evaluation, variability, and failure analysis.
- The E0–E5 evidence categories are explicitly identified as an internal descriptive framework, not a universal scientific hierarchy.
- Qualitative and creative research are not forced into quantitative metrics.

**Weaknesses and corrections**
- It is very long and repeats some standards also present in Quality Standards and Responsible AI.
- It recommends future specialist research templates in Section 19, but those templates have not yet been created. The text correctly frames them as future recommendations; they should not be presented elsewhere as existing assets.
- It defines experiment IDs as `FCL-EXP-YYYY-NNN`, but the Project Template has only a generic Project ID field. Distinguish project identifiers from experiment identifiers and provide a place to reference experiment records.

**Recommendation:** retain the methodology as the authoritative research document. Shorten repeated generic security and AI policy content by referring to the relevant specialist documents.

### 3.5 `CONTRIBUTING.md` — 3.3/5

**Strengths**
- Clearly describes the founder-led review model and contributor limitations.
- Covers proposals, issues, branches, pull requests, code quality, research integrity, confidentiality, attribution, and review outcomes.
- Requires contributors to have rights to submit their material and rejects unresolved ownership questions.
- Does not imply that submission automatically transfers ownership.

**High-impact gap**
- The repository has no general open-source licence, and the Contribution Guidelines state that the contributor retains their rights and that submission does not establish an open-source licence.
- However, the documents do not define the specific permission or licence grant that allows the Lab to incorporate, reproduce, modify, display, distribute, or maintain an accepted external contribution in the public repository.
- The statement that contribution rights are governed by applicable project terms and separate agreements does not resolve this unless those terms are actually defined for the relevant project.

**Recommendation:** before accepting or merging third-party code or creative material, establish project-specific licence terms and an explicit contribution permission/ agreement. Alternatively, restrict external code contributions until those terms exist. Do not add an open-source licence by default; the Lab must make an intentional choice.

### 3.6 `SECURITY.md` — 3.5/5

**Strengths**
- Covers application, infrastructure, data, dependency, AI, and agent security.
- Avoids guaranteed response times and acknowledges the single-maintainer operating model.
- Gives correct priority to revoking exposed credentials rather than simply deleting visible files.
- Distinguishes vulnerability reporting from ordinary feature requests and low-quality outputs.

**Operational gap**
- Section 6.1 says GitHub Private Vulnerability Reporting is preferred only if enabled, and explicitly requires the maintainer to enable it before presenting it as available.
- If it is unavailable, the document requires a separately published security contact method. No such fallback route is identified in the audited documentation.
- The GitHub setting itself was not verified in this audit; its state is therefore **unknown**, not assumed disabled.

**Recommendation:** verify and enable GitHub Private Vulnerability Reporting, or publish a real security contact route. Until that is done, describe the process as not yet operational rather than implying that a reporter can currently use it.

### 3.7 `CODE-OF-CONDUCT.md` — 3.7/5

**Strengths**
- Provides clear expectations, unacceptable behaviour, and proportionate enforcement measures.
- Explicitly acknowledges the limitations of a founder-led reporting process.
- Does not pretend that an independent ombudsperson or moderation committee exists.
- Avoids fixed response times and guarantees of independent adjudication.

**Operational gap**
- Section 8.1 requires an accessible private reporting method to be published before the reporting process is described as operational.
- No private conduct-reporting channel is identified in the audited files.

**Recommendation:** publish an actual route for private conduct reports, or clearly label the process as awaiting channel configuration. Keep the explicit disclosure that reports involving the maintainer cannot be guaranteed independent adjudication under the current model.

### 3.8 `GOVERNANCE.md` — 3.8/5

**Strengths**
- The founder-led model is described credibly, with no invented organisational bodies.
- Decision authority for strategic, operational, project, publication, and security matters is clearly assigned.
- Delegation, access control, conflicts of interest, and succession are addressed realistically.
- Distinguishes consultation from transfer of decision-making authority.

**Weaknesses and corrections**
- Section 6.3 contains its own project lifecycle vocabulary, while Section 6.4 contains another status vocabulary.
- These differ from both the Charter and Project Lifecycle document.
- Sections on project governance, IP, access, conflicts, and disputes duplicate material elsewhere.

**Recommendation:** retain the authority model and role definitions. Point to `PROJECT-LIFECYCLE.md` for the canonical lifecycle and use it as the sole authoritative definition of project statuses.

### 3.9 `PROJECT-LIFECYCLE.md` — 4.2/5

**Strengths**
- Its nine-stage process is clear and proportionate: Idea and Intake; Proposal; Discovery and Feasibility; Experimentation and Development; Validation and Evaluation; Publication Review; Publication and Release; Maintenance and Evolution; Archival or Discontinuation.
- Section 14 provides a useful distinct project status register.
- It separates technical completion from publication approval.
- It accounts for negative findings, scope changes, risk reassessment, maintenance limitations, and archival.

**Weaknesses and corrections**
- Other documents use different stage and status labels, so this document's good framework is not yet the shared framework.
- Some publication and quality details repeat the dedicated policies.

**Recommendation:** designate this document as the single source of truth for lifecycle stages and project status labels. Other documents should use the same vocabulary or link here.

### 3.10 `QUALITY-STANDARDS.md.` — 4.0/5

**Strengths**
- Broad and technically coherent coverage of code quality, architecture, testing, resilience, performance, security, privacy, UX, accessibility, AI evaluation, reproducibility, and documentation.
- Properly states that quality requirements should be proportional to project purpose, maturity, complexity, and risk.
- Avoids equating a successful demonstration with production readiness.

**Weaknesses and corrections**
- The five “Project Quality Levels” combine different dimensions: `Exploratory`, `Prototype`, and `Validated` are maturity/evidence descriptions; `Public Release` is a publication state; `Production-Oriented` is operational readiness.
- The Project Template calls this field `Quality Level`, making the mixed taxonomy harder to interpret.
- Section 13.7 refers to `RESPONSIBLE-AI.md`, while the actual file path has a final dot.
- The filename itself ends with a period and therefore differs from the expected path.

**Recommendation:** retain the engineering standards but separate project maturity/evidence, publication state, and production-readiness attributes. Rename the file to `QUALITY-STANDARDS.md` and update references.

### 3.11 `RESPONSIBLE-AI.md.` — 3.8/5

**Strengths**
- Separates AI as a development tool from AI as part of a deployed system.
- Explicitly labels A0–A4 as an internal Lab risk framework, not a regulatory classification.
- Covers human oversight, data handling, models and providers, prompts, agents, tool permissions, evaluation, fairness, IP, transparency, and resource considerations.
- Does not treat a language model as an authorization boundary.

**Weaknesses and corrections**
- Data classification differs from Publication Policy §10.1.
- The document is very long and repeats security, privacy, AI evaluation, and research requirements also present in other files.
- Its filename ends with a period, while other files refer to `RESPONSIBLE-AI.md` without it.

**Recommendation:** keep the AI-specific policy as the authority for AI risk and use controls. Consolidate the data taxonomy and reduce repeated generic software security and research method passages by cross-referencing the relevant documents. Rename the file to `RESPONSIBLE-AI.md`.

### 3.12 `PROJECT-TEMPLATE.md` — 3.4/5

**Strengths**
- Covers the full project record, from objectives and scope through architecture, AI, data, security, testing, IP, publication, maintenance, and review.
- Clearly marks several sections as optional and warns against publishing confidential information or placeholders.
- Includes separate fields for publication classification and publication decision, which is conceptually sound.

**Weaknesses and corrections**
- The 27-section, 1,083-line template is too heavy as the default form for small experiments. Its completeness is useful as a master reference, but not every project should be forced to fill every field.
- Section 20.1 `Current Lifecycle Stage` mixes stage labels and project status labels, and it does not match the nine stages in Project Lifecycle §4.
- Section 9.2's data checkboxes use a taxonomy different from Publication Policy §10.1.
- The public project record includes sensitive classification choices and publication restrictions. The template does warn against revealing restricted information, but it should explicitly distinguish private assessment records from safe public summaries so metadata does not disclose confidential project existence or details.
- The note in Section 18 says P1, P2, and P3 are not “public-ready,” but does not explain that P1 may be eligible for controlled public release after additional checks and approval (if that is the intended meaning).

**Recommendation:** retain this as a comprehensive master template, but create a short project brief/README template for small experiments. Separate lifecycle stage, project status, maturity/quality, publication classification, and publication decision. Keep sensitive internal review details out of the public-facing version.

---

## 4. Cross-Document Consistency Matrix

| Topic | Documents compared | Current state | Resolution / authoritative owner |
|---|---|---|---|
| Lab identity and mission | README, Charter, Governance | Consistent: independent, founder-led, multidisciplinary Lab | README owns the public overview; Charter owns foundational identity/principles |
| Founder-led decision authority | Charter, Governance, Contributing, Lifecycle, AI policy | Mostly consistent; J-ART retains final authority | `GOVERNANCE.md` owns authority and roles |
| Publication approval | Charter, Publication Policy, Governance, Lifecycle, Template | Generally consistent: maintainer approves publication after review | `PUBLICATION-POLICY.md` owns the detailed publication procedure; Governance names the authority |
| Confidentiality and private-project separation | README, Charter, Publication Policy, Governance, Security, Contributing | Strong and consistent | `PUBLICATION-POLICY.md` owns publication/confidentiality checks; README summarises boundary |
| Project lifecycle stages | Charter, Governance, Project Lifecycle, Template | Inconsistent vocabularies | `PROJECT-LIFECYCLE.md` should be authoritative for stages |
| Project statuses | README, Charter, Governance, Project Lifecycle, Template | Multiple non-equivalent lists | `PROJECT-LIFECYCLE.md` should be authoritative for status labels |
| Quality and maturity | Quality Standards, Template, Lifecycle | Quality level mixes readiness and publication state | `QUALITY-STANDARDS.md` owns technical quality; separate maturity/readiness axes |
| Publication classification | Publication Policy, Template | Mostly aligned, but P1/P3 implications need clarification | `PUBLICATION-POLICY.md` owns P0–P3 definitions and decision workflow |
| AI risk levels | Responsible AI, Template | Aligned A0–A4; internal-only disclaimer is appropriate | `RESPONSIBLE-AI.md` owns A0–A4 |
| Data classification | Publication Policy, Responsible AI, Template | Inconsistent use of Personal vs Restricted | Define one canonical data classification and treat personal data consistently |
| Research evidence | Research Methodology, Lifecycle, Quality, Template | Strong in the research document; other docs summarise differently | `RESEARCH-METHODOLOGY.md` owns methods and E0–E5 evidence framework |
| Contribution rights | README, Contributing, Publication Policy | Rights retention is clear; licence/permission to use accepted contribution is not | `CONTRIBUTING.md` plus an explicit project licence/contribution agreement |
| Vulnerability reporting | Security, Contributing | Conditional on private channel being available | `SECURITY.md` owns the process; verify GitHub setting and publish fallback if needed |
| Conduct reporting | Code of Conduct | Private route required but not identified | `CODE-OF-CONDUCT.md` owns conduct process; publish actual route |
| Document navigation | All twelve files | No internal Markdown links found | README should own the index; cross-references should be clickable |

### Recommended document ownership map

| Subject | Authoritative file | Other files should |
|---|---|---|
| Public identity and overview | `README.md` | Link to policies; avoid copying their full content |
| Foundational mission and principles | `LAB-CHARTER.md` | State principles, not duplicate procedures |
| Publication eligibility, approval, withdrawal | `PUBLICATION-POLICY.md` | Refer to it for release decisions |
| Research method and evidence | `RESEARCH-METHODOLOGY.md` | Refer to it for experimental protocols |
| Contribution workflow and rights | `CONTRIBUTING.md` | Refer to relevant policies for security and publication |
| Vulnerability reporting | `SECURITY.md` | Avoid repeating the reporting process elsewhere |
| Behaviour and conduct reports | `CODE-OF-CONDUCT.md` | Refer to it for collaboration behaviour |
| Roles and decision authority | `GOVERNANCE.md` | Avoid restating authority matrices |
| Lifecycle stages and project statuses | `PROJECT-LIFECYCLE.md` | Reuse its exact vocabulary |
| Engineering and quality | `QUALITY-STANDARDS.md` | Refer to it for tests and technical gates |
| AI-specific principles and controls | `RESPONSIBLE-AI.md` | Refer to it for AI risk and oversight |
| Project record format | `PROJECT-TEMPLATE.md` | Use a short derivative template for small projects |

---

## 5. Terminology and Classification Register

### 5.1 Canonical project lifecycle stages

Use the nine stages in `PROJECT-LIFECYCLE.md` §4 without renaming them across documents:

1. Idea and Intake
2. Proposal
3. Discovery and Feasibility
4. Experimentation and Development
5. Validation and Evaluation
6. Publication Review
7. Publication and Release
8. Maintenance and Evolution
9. Archival or Discontinuation

These are **workflow stages**, not project statuses.

### 5.2 Canonical project statuses

Use the status register in `PROJECT-LIFECYCLE.md` §14:

- Proposed
- Concept
- Experimental
- Prototype
- Development
- Validation
- Published
- Maintenance
- Archived
- Discontinued

A project can move through multiple lifecycle stages while using a current status that describes its present condition. A stage and a status should never be placed in the same field.

### 5.3 Quality and operational readiness

The current five-level Quality Standards model should be revised because it mixes distinct axes. Recommended treatment:

- **Technical maturity/evidence:** Exploratory, Prototype, Validated.
- **Publication state:** Not reviewed, Pending, Approved, Published, Withdrawn.
- **Operational readiness:** Experimental / Not production-oriented / Production-oriented (define only if needed).

This is a proposed design, not a claim that the current files already define these three taxonomies.

### 5.4 Publication classifications

Retain the existing internal classification definitions from `PUBLICATION-POLICY.md` §5:

- P0 — Public-ready.
- P1 — Controlled publication.
- P2 — Restricted review.
- P3 — Non-publishable.

Add an explicit rule for P1: whether public release is permitted after additional checks and a separate approval. Add an explicit reclassification procedure for P2 and P3 when new rights, permissions, or facts materially change the assessment. Do not treat publication classification as publication approval.

### 5.5 AI risk classifications

Retain the existing internal levels from `RESPONSIBLE-AI.md` §4:

- A0 — Minimal Risk.
- A1 — Low Risk.
- A2 — Moderate Risk.
- A3 — High Risk.
- A4 — Restricted Use.

Keep the document's disclaimer that this is an internal Lab framework, not a legal or regulatory classification.

### 5.6 Data classification

The three existing sources do not currently agree. Recommended common structure:

- Public
- Internal
- Confidential
- Restricted

Treat `Personal data` as a data attribute that can apply across one or more classes, rather than a mutually exclusive class, unless the Lab deliberately chooses a different model. Define whether Sensitive Personal Data is an additional marker or a subtype of Restricted. Reflect the chosen model in Publication Policy, Responsible AI, and Project Template.

### 5.7 Roles

The main role vocabulary is generally consistent:

- Founder and Maintainer — J-ART in the current model.
- Contributor — submits work or participates in an accepted contribution.
- Collaborator — participates in a specifically agreed activity.
- External Provider — operates an external service, platform, tool, or dependency.

Do not introduce Project Lead, Independent Reviewer, Committee, or other roles as if they currently exist. A project may assign a specific delegated responsibility, but it should record the delegation explicitly.

### 5.8 Mandatory and advisory language

The documents use `must`, `should`, and `may` reasonably often, but the framework does not contain a shared definitions section. Add a short convention in the Charter or a documentation standard:

- **MUST / MUST NOT:** mandatory requirement.
- **SHOULD / SHOULD NOT:** expected practice; deviations require a reason where material.
- **MAY:** permitted option.
- **Where applicable / where appropriate:** conditional on project scope and risk; state the condition when it is not self-evident.

Avoid changing every occurrence mechanically; apply this only where the intended force is ambiguous.

---

## 6. Critical Findings Register

Severity uses the audit prompt's categories. The count is 3 High, 6 Medium, 2 Low, and 0 Critical.

| ID | Severity | Document / section | Finding | Impact | Recommended action |
|---|---|---|---|---|---|
| AUD-001 | HIGH | `QUALITY-STANDARDS.md.`; `RESPONSIBLE-AI.md.`; references in Template and Quality Standards | Both actual filenames end with a trailing period. References use paths without the period and therefore do not match the actual Git paths. | Broken navigation and non-portable filenames; scripts and local checkouts may also handle trailing-dot names inconsistently across environments. | Rename both paths to the intended `.md` names; update all references; verify GitHub links and local checkout. |
| AUD-002 | HIGH | README §12; Charter §§7, 16; Governance §6; Lifecycle §§4, 14; Template header and §20.1 | Project lifecycle stages, project statuses, and maturity labels are mixed or use different vocabularies. The Template §20.1 combines stage and status terms in one field. | The Lab cannot reliably classify or report project state; templates and project documentation may contradict each other. | Make `PROJECT-LIFECYCLE.md` authoritative for stages and statuses; split template fields; align README, Charter, Governance and Quality Standards. |
| AUD-003 | HIGH | README §14; `CONTRIBUTING.md` §§12, 19 | Contributor ownership is retained, but no explicit licence or permission grant allows the Lab to incorporate and publicly distribute accepted contributions under defined terms. | Unclear rights to use, maintain, reproduce, modify, and distribute accepted third-party contributions, despite contribution workflow inviting submissions. | Decide on per-project licensing and explicit contribution terms before accepting external IP; consider a project-specific licence and suitable contribution agreement. Do not silently create an open-source licence. |
| AUD-004 | MEDIUM | `SECURITY.md` §6.1; `CODE-OF-CONDUCT.md` §8.1; `CONTRIBUTING.md` §7.5 | Private vulnerability and conduct reporting depend on channels that must be enabled or published, but no fallback contact or route appears in the audited docs. The GitHub Private Vulnerability Reporting setting was not verified. | A reporter may be instructed to report privately without a discoverable way to do so. | Verify/enable GitHub Private Vulnerability Reporting; publish a real private conduct-reporting route; do not invent a contact address. |
| AUD-005 | MEDIUM | README; all cross-document references | No Markdown links to the other `.md` files were found. References are plain inline-code filenames. | Poor discoverability, more friction for users and contributors, and harder maintenance of the policy set. | Add a linked documentation index to README and clickable relative links in related-document sections. |
| AUD-006 | MEDIUM | Publication Policy §10.1; Responsible AI §6.1; Project Template §9.2 | Data categories differ: Publication Policy includes Personal and Sensitive/restricted; Responsible AI and Template use Public/Internal/Confidential/Restricted. | A project could classify the same information differently in its publication review, AI risk review, and project record. | Define one canonical data classification; treat personal data consistently, preferably as an attribute/marker as well as a protected data type; update all three files. |
| AUD-007 | MEDIUM | Publication Policy §§4.2, 5.3–5.5; Project Template §18 | P1 controlled publication is not explicit about public release conditions; the Template says P1/P2/P3 are not public-ready, which can be read as if P1 were not publishable at all. P3's non-publishable definition sits alongside wording about separate authorisation. | Reviewers may interpret classifications and approval decisions differently. | State whether P1 can be publicly released after control checks and approval; clarify that P2/P3 can only be reconsidered after a material change and formal reclassification, not an informal exception. |
| AUD-008 | MEDIUM | Quality Standards §4; Project Template header | The Quality Standards “levels” combine maturity/evidence (`Exploratory`, `Prototype`, `Validated`), publication state (`Public Release`), and deployment orientation (`Production-Oriented`). | The `Quality Level` field is not a single coherent scale and may create misleading maturity claims. | Separate technical maturity, publication state, and production-readiness into distinct fields or rename/restructure the levels. |
| AUD-009 | MEDIUM | README; Charter; Governance; Contributing; Security; Quality; Research; Responsible AI; Lifecycle; Template | Significant duplication of operational rules across the 12 documents. The framework totals approximately 11,667 lines and 50,052 words; several files independently restate publication, lifecycle, AI, security, and quality material. | Policy drift becomes more likely as documents are edited independently; maintenance burden is high for a single-maintainer Lab. | Retain each document but establish strict ownership boundaries and replace repeated procedures with short summaries and links. Shorten the README and Charter first. |
| AUD-010 | LOW | Metadata across eleven policy/template files | Metadata uses different field names and status labels (`Established`, `Effective Date`, `Initial Charter`, `Initial Policy`, `Initial`, `Initial Guidelines`, `Active Template`). Dates and versions are otherwise broadly consistent. | Minor inconsistency in document register and future revision management. | Standardise a short metadata header: Document ID, Version, Status, Effective Date, Maintainer, Repository; preserve historical “Established” dates only where meaningful. |
| AUD-011 | LOW | Project Template §§5, 8–10, 18–20 | The master template is 27 sections and 1,083 lines; optionality is indicated locally but it is still too large as the default for small experiments. Public-facing project records also need a stronger distinction from private review data. | Users may skip the template, fill it mechanically, or expose sensitive internal classification details in a public project page. | Retain it as a comprehensive master template; create a concise project brief/README derivative and keep sensitive risk assessment records private. |

---

## 7. Duplication and Responsibility Analysis

### Content to keep

- The detailed publication approval, confidentiality, ownership, and withdrawal procedure belongs in `PUBLICATION-POLICY.md`.
- Research design, evidence categories, and experiment reporting belong in `RESEARCH-METHODOLOGY.md`.
- Technical tests, code quality, accessibility, performance, and definition of done belong in `QUALITY-STANDARDS.md`.
- AI risk, human oversight, model/provider review, and agent boundaries belong in `RESPONSIBLE-AI.md`.
- Decision rights and role responsibilities belong in `GOVERNANCE.md`.
- Lifecycle stages and project statuses belong in `PROJECT-LIFECYCLE.md`.
- Detailed project data entry belongs in `PROJECT-TEMPLATE.md`.

### Content to shorten or move to references

- **README:** reduce repeated process detail and link to authoritative policy sections.
- **LAB-CHARTER:** keep principles and authority; move detailed operational procedures to specialist policies.
- **GOVERNANCE:** keep decision authority and delegation; refer to Project Lifecycle and Publication Policy for detailed procedures.
- **CONTRIBUTING:** keep contributor workflow and rights; refer to Security, Quality, and Research Methodology rather than restating their technical rules.
- **PROJECT-LIFECYCLE:** keep stage gates and outcomes; refer to Publication Policy and Quality Standards for detailed review criteria.
- **SECURITY / RESPONSIBLE-AI / QUALITY:** keep each specialist scope clear; link between them rather than reproducing entire controls.

### Duplication classification

| Overlap | Classification | Treatment |
|---|---|---|
| Confidentiality principles in README, Charter, Publication Policy, Governance, Security, Contributing | Necessary reinforcement in summary form; detailed duplication should be reduced | Publication Policy owns the full rule set |
| Governance and lifecycle stage/status tables | Contradictory duplication | Project Lifecycle owns the lists; Governance links to it |
| Research evaluation in Research Methodology, Lifecycle, Quality, Responsible AI | Acceptable contextual repetition, but definitions should have one owner | Research Methodology owns research evaluation; Quality owns engineering test expectations; AI policy adds AI-specific evaluation |
| AI security in Security, Responsible AI, Quality | Acceptable overlap for context, but detailed controls should have a single owner | Security owns vulnerability handling; Responsible AI owns AI-specific use risks; Quality points to both |
| IP/licensing in Charter, Publication Policy, Contributing, Governance, Template | Repetitive and rights-sensitive | Publication Policy owns publication rights; Contributing owns the terms for submitted contributions |
| README methodology and quality sections vs specialist policies | Excessive summary duplication | README should summarise and link |

---

## 8. Missing Elements and Recommendations

### Essential before public presentation as an operational framework

1. Correct the two filenames with trailing dots and update references.
2. Adopt a single lifecycle-stage and project-status register.
3. Resolve contribution permissions and project licensing for any external contributions.
4. Establish and publish private security and conduct reporting channels; verify relevant GitHub configuration.
5. Add a README documentation index and clickable cross-links.
6. Align data classification and publication classification semantics.

### Important operational improvements

- Add a concise record format for material decisions and publication approval if the Lab begins accepting external contributors or publishing more complex software.
- Specify whether a P1 release may be public after additional controls and explicit approval.
- Separate a public project summary from any private publication/security assessment record.
- Establish an explicit document hierarchy: applicable law and contract/licence obligations first; Charter for foundational Lab principles; specialist policy for detailed subject-specific procedure; project-specific requirements may add stricter controls but not override the foundations.

### Optional future documentation

The existing documents already identify possible future templates, including Research Brief, Experiment Protocol, AI Evaluation Protocol, Technical Evaluation Report, Comparative Study, and Research Findings Report. These may be introduced when real projects require them.

Do not create another policy for every topic. The current twelve-document set is already extensive.

### Not identified as a defect

- No `LICENSE` file: consistent with the README's explicit no-general-open-source-licence statement.
- No `ATTRIBUTIONS.md`: currently a recommendation for projects with substantial third-party material, not a universal requirement.
- No `docs/`, `experiments/`, `tools/`, `prototypes/`, `templates/`, or `resources/` directories: the README explicitly says those folders will be introduced progressively.
- No separate board, committee, independent reviewer, or security team: the documents correctly describe a founder-led operating model and disclose its limitations.

---

## 9. Legal, Regulatory, and Compliance Claims

No broad statement was identified in the inspected files claiming that Framing Creativity Lab is certified or fully compliant with a particular legal or regulatory framework.

Positive points:

- The AI risk framework says it is internal and not a legal/regulatory classification.
- Security policy states it is not a security certification or guarantee that vulnerabilities do not exist.
- Publication Policy warns against unsupported claims that a project is anonymous, privacy-preserving, or compliant.
- Research Methodology distinguishes internal evidence labels from a universal scientific evidence hierarchy.

However, terms such as “appropriate legal basis,” “personal data,” “sensitive information,” “copyright,” and “third-party licence” depend on jurisdiction and context. This documentation audit did not perform a legal review or verify compliance under any specific jurisdiction. For projects processing personal data or using third-party content, targeted legal/licensing review may still be necessary.

**Do not add a blanket compliance claim to the README or Charter.**

---

## 10. GitHub and Markdown Readiness

| Check | Result | Comment |
|---|---|---|
| Repository access | Pass | Public repository and `main` branch accessible |
| Twelve content files present | Pass with path issue | All 12 are in the tree; two filenames end with a dot |
| Root structure | Pass | Flat root is consistent with the README's progressive folder plan |
| README navigation to policies | Fail | No policy index or links to the other documents |
| Markdown links between `.md` files | Fail | No internal Markdown links found in the 12 files |
| Document IDs | Pass | Eleven non-README documents have unique IDs |
| Version numbers | Pass | All identified policy/template files show v1.0 |
| Metadata conventions | Minor issue | Status/date field names differ |
| License file | Intentional | README explicitly states there is no general open-source licence |
| GitHub Private Vulnerability Reporting | Not verified | Policy says the setting must be enabled before representing it as available |
| Markdown syntax | Partial | Content and fenced blocks were fetched; no separate full Markdown renderer/linter was run |
| External link validation | Not performed | No broad external-link crawl was included in this read-only content audit |

### Navigation recommendation

Add a compact section to README, for example `Documentation`, with a short description and relative link for each policy. Convert “Related Documents” lists in the other files from inline-code filenames to relative Markdown links. Use links that match the corrected exact file paths.

---

## 11. Remediation Plan

### Phase 1 — Publication blockers

| Priority | Affected files | Issue | Proposed resolution | Dependency | Expected outcome |
|---|---|---|---|---|---|
| P0 | `QUALITY-STANDARDS.md.`, `RESPONSIBLE-AI.md.`, all references | Trailing-dot paths | Rename to exact expected `.md` names and update references | None | All twelve filenames resolve consistently |
| P0 | README, Charter, Governance, Project Lifecycle, Quality Standards, Project Template | Status/stage/quality taxonomy conflict | Adopt separate authoritative stage, status, maturity/quality, publication, and AI risk fields; align every reference | Taxonomy decision | No contradictory project state fields |
| P0 | README, Contributing, Publication Policy | Accepted contribution rights unclear | Decide licence/permission terms for incoming contributions before external merges | Maintainer rights decision | Clear lawful basis for accepting and distributing contributions |
| P0 | Security, Code of Conduct | Private report routes unavailable or unverified | Verify/enable GitHub private vulnerability reporting; publish a private conduct channel | GitHub setting and real contact route | People can actually report sensitive matters privately |

### Phase 2 — Consistency and quality improvements

| Priority | Affected files | Issue | Proposed resolution | Dependency | Expected outcome |
|---|---|---|---|---|---|
| P1 | README, all related-document sections | No internal links | Add documentation index and cross-links | Correct filenames | Navigable repository documentation |
| P1 | Publication Policy, Responsible AI, Project Template | Data-classification mismatch | Define canonical data categories and personal-data marker; align tables/checklists | Taxonomy decision | Same data is classified consistently |
| P1 | Publication Policy, Project Template | P1/P3 rules ambiguous | Clarify controlled publication and formal reclassification | Publication policy decision | Reviewers distinguish classification from approval |
| P1 | Quality Standards, Project Template | Quality scale mixed with release/readiness | Separate technical maturity, publication state, and production readiness | Taxonomy decision | Meaningful and non-overlapping fields |
| P2 | README, Charter, Governance, Contributing, Quality, AI, Lifecycle | Duplicated procedures | Keep detailed rule in authoritative document; shorten and link summaries elsewhere | Ownership map | Lower maintenance burden and less policy drift |
| P2 | Project Template | Too large as default and sensitive fields | Keep master template; add concise derivative; separate private assessment from public page | Template design | Easier adoption without leaking internal assessments |

### Phase 3 — Future operational improvements

| Priority | Affected files / area | Improvement | Trigger |
|---|---|---|---|
| P3 | Repository governance | Add a lightweight decision/publication record template | When several projects or external collaborators are active |
| P3 | `templates/` | Add Research Brief, Experiment Protocol, AI Evaluation Protocol, ADR, and short Project Brief templates | When actual projects require them |
| P3 | Repository maintenance | Introduce automated Markdown link checking and filename validation | After the path and navigation corrections |
| P3 | Security operations | Consider secret scanning, dependency review, and code scanning where suitable | As code and dependencies are added; do not claim these are currently enabled |

---

## 12. Final Publication Checklist

### Content and governance

- [ ] The twelve expected files exist with exact filenames.
- [ ] Every document has one clear primary responsibility.
- [ ] Founder-led authority is described consistently.
- [ ] No nonexistent committee, role, or independent process is implied.
- [ ] Publication decisions have a single clear authority and process.
- [ ] Project lifecycle stages and statuses use one canonical vocabulary.
- [ ] Quality maturity is separate from publication and production readiness.

### Rights and confidentiality

- [ ] The no-general-licence position is intentional and clearly stated.
- [ ] The terms for accepted external contributions are explicit.
- [ ] Third-party assets, software, datasets, models, and generated outputs have been reviewed.
- [ ] No confidential/private project information, code, prompts, assets, or metadata is included.
- [ ] Public project records do not reveal restricted assessment details.

### Security, privacy, and reporting

- [ ] GitHub Private Vulnerability Reporting is verified and enabled, or a real private alternative is published.
- [ ] A private conduct-reporting route is published.
- [ ] Data classification is consistent across all documents.
- [ ] Credential, privacy, and incident procedures are aligned.
- [ ] No unsupported security or compliance guarantees are present.

### Navigation and Markdown

- [ ] README has a Documentation index with relative links to all eleven supporting files.
- [ ] All cross-document references are clickable and resolve.
- [ ] Trailing-dot filenames have been corrected.
- [ ] Headings, tables, code fences, and Mermaid diagrams render correctly.
- [ ] A Markdown/link checker has been run against the corrected branch.

### Metadata and approval

- [ ] Document IDs are unique.
- [ ] Version and effective-date conventions are consistent.
- [ ] Template placeholders are clearly marked and not mistaken for completed project content.
- [ ] All Phase 1 findings are resolved.
- [ ] The maintainer has reviewed the final public branch.

---

## 13. Final Verdict

### Overall maturity

**3.7 / 5 — Strong foundational content, but only conditionally ready for public presentation as a unified framework.**

### Findings summary

| Severity | Count |
|---|---:|
| Critical | 0 |
| High | 3 |
| Medium | 6 |
| Low | 2 |
| Informational (not counted as defects) | Several observations |

### Document readiness

| Readiness | Documents |
|---|---:|
| Ready with minor or bounded corrections | 5 |
| Require material revision or alignment | 7 |
| Total | 12 |

The five strongest documents in their subject areas are `PROJECT-LIFECYCLE.md`, `RESEARCH-METHODOLOGY.md`, `PUBLICATION-POLICY.md`, `QUALITY-STANDARDS.md.` and `GOVERNANCE.md`. They still need the cross-document and filename corrections described above.

The seven requiring material revision or alignment are `README.md`, `LAB-CHARTER.md`, `CONTRIBUTING.md`, `SECURITY.md`, `CODE-OF-CONDUCT.md`, `RESPONSIBLE-AI.md.`, and `PROJECT-TEMPLATE.md`.

### Three most important corrective actions

1. **Fix the document paths and establish a canonical taxonomy** for lifecycle stages, statuses, quality maturity, publication classification, and data classification.
2. **Resolve accepted contribution licensing/permission terms** before inviting or merging external intellectual property into a repository with no general licence.
3. **Make private reporting operational and discoverable**, then add the README documentation index and working cross-links.

### Final recommendation

Do not rewrite all twelve documents from scratch. Their foundation is sound, and several policies are already strong. Run a focused remediation pass that resolves the three high-severity findings first, then align the taxonomies, reporting channels, and navigation. After those changes, perform a second read-only validation against the corrected commit.

**Audit boundary:** This report assesses the public repository contents at the commit identified above. It does not certify legal compliance, security posture, or the status of GitHub settings that were not directly verified. No source file or repository setting was changed during the audit.
