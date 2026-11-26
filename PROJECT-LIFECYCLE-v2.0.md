# Project Lifecycle

**Document ID:** FCL-PROC-001  
**Version:** 2.0  
**Status:** Draft for Maintainer Review  
**Effective Date:** Pending approval  
**Maintainer:** J-ART  
**Repository:** Framing Creativity Lab

---

## 1. Purpose

Framing Creativity Lab develops independent research, technical experiments, prototypes, creative technologies, and digital tools.

Each project follows a lifecycle appropriate to its purpose, complexity, and maturity.

This document establishes a common framework for initiating, exploring, developing, evaluating, publishing, maintaining, and retiring projects within the Lab.

Its purpose is to:

- Provide a consistent structure for project development.
- Clarify the different stages of a project's lifecycle.
- Define expectations before significant development begins.
- Establish criteria for evaluating progress and readiness.
- Distinguish experimental work from validated and published work.
- Ensure that publication decisions consider quality, security, privacy, and intellectual property.
- Preserve useful knowledge from completed or discontinued projects.
- Support reproducibility and continuity across the Lab.

The lifecycle is designed to provide structure without imposing unnecessary process on small experiments.

Not every project requires the same degree of documentation, validation, or maintenance.

---

## 2. Scope

This lifecycle applies to projects and initiatives developed, maintained, or published under Framing Creativity Lab.

It may be used for:

- Artificial intelligence experiments.
- Machine learning explorations.
- Creative technology prototypes.
- Digital products and applications.
- Software tools and utilities.
- Research projects.
- Technical demonstrations.
- Experimental interfaces.
- Design and interaction systems.
- Technical documentation and reference implementations.
- Other independent initiatives aligned with the Lab's mission.

The lifecycle applies to both software and non-software projects.

A research report, for example, may follow the same broad progression as a software prototype while requiring different validation and publication criteria.

---

## 3. Lifecycle Principles

The project lifecycle follows several foundational principles.

### 3.1 Purpose Before Implementation

A project should begin with a sufficiently clear question, problem, opportunity, or creative intention.

Development should not become an end in itself.

The objective is to produce meaningful knowledge, a useful technical result, a demonstrable concept, or a clearly documented experiment.

### 3.2 Proportionate Process

The amount of structure should correspond to the project's scale and risk.

A short technical experiment may need only a concise description, implementation notes, and a conclusion.

A complex application or public-facing system may require requirements, architecture documentation, formal testing, security review, and maintenance planning.

### 3.3 Evidence Over Assumption

Project maturity should reflect demonstrated results rather than ambition or presentation quality.

A visually convincing prototype is not necessarily a validated product.

A successful demonstration does not automatically establish reliability, scalability, security, or production readiness.

### 3.4 Controlled Progression

Projects may advance when their objectives and relevant acceptance criteria have been met.

Progression should not be automatic.

A project may return to an earlier stage when new evidence, technical limitations, or risks require reconsideration.

### 3.5 Responsible Publication

Public release is a deliberate decision.

Completion of development does not automatically authorize publication.

Every public release must comply with the Lab's Publication Policy and applicable security, privacy, licensing, and confidentiality requirements.

### 3.6 Learning From Failure

A project does not need to succeed technically or commercially to produce value.

Negative results, failed hypotheses, abandoned approaches, and unexpected behavior can provide useful research knowledge when they are documented honestly.

---

## 4. Lifecycle Overview

Projects generally progress through the following stages:

| Stage | Name | Primary objective |
|---|---|---|
| 01 | Idea and Intake | Identify an opportunity or question |
| 02 | Proposal | Define purpose, scope, and expected outcomes |
| 03 | Discovery and Feasibility | Investigate context, constraints, and feasibility |
| 04 | Experimentation and Development | Build, test, and explore |
| 05 | Validation and Evaluation | Assess results against defined criteria |
| 06 | Publication Review | Determine whether the project is suitable for release |
| 07 | Publication and Release | Approve and publish the work |
| 08 | Maintenance and Evolution | Correct, improve, and maintain where applicable |
| 09 | Archival or Discontinuation | Preserve knowledge or formally close the project |

### 4.1 Lifecycle Stage and Project Status

Lifecycle Stage and Project Status are separate fields.

- **Lifecycle Stage** identifies the point reached in the Lab's project workflow. The nine canonical stages are defined in this section.
- **Project Status** describes the project's current state. The canonical status vocabulary is defined in Section 14.

The two fields answer different questions and must not be used interchangeably. A stage describes process position; a status describes the current state of the work. They may be related, but one must not be inferred solely from the other.

Technical Maturity and Operational Readiness are separate assessment dimensions defined in `QUALITY-STANDARDS-v2.0.md`.

Publication Classification and Publication Status are governed by `PUBLICATION-POLICY-v2.0.md`.

A project record should use the relevant fields independently and should not describe a project as validated, publicly approved, or production-oriented without the corresponding evidence or decision.

This lifecycle is a reference framework, not a mandatory linear sequence.

A project may skip stages that are not relevant, repeat an experiment, remain exploratory, or be discontinued before publication.

---

## 5. Stage 01 — Idea and Intake

### 5.1 Objective

The first stage identifies a potential opportunity for research, experimentation, or development.

Ideas may emerge from:

- A technical problem.
- A research question.
- An emerging technology.
- A creative concept.
- An observed limitation.
- An opportunity for experimentation.
- A potential improvement to an existing public project.
- An independent exploration of a new method or approach.

### 5.2 Initial Assessment

At this stage, the project should be evaluated informally against the following questions:

- Does it relate to the Lab's mission?
- Is the underlying question or opportunity sufficiently interesting?
- Is there a potential technical, research, or creative outcome?
- Does the idea require access to external services or resources?
- Are there obvious intellectual property, privacy, or security concerns?
- Is the project feasible with available resources?

An idea does not require a complete technical specification before it can be explored.

### 5.3 Expected Output

The result may be a brief idea record containing:

- Working title.
- Initial description.
- Problem or opportunity.
- Research or creative question.
- Expected direction.
- Initial considerations.

### 5.4 Stage Exit

An idea may proceed to a formal proposal, remain in an idea backlog, be merged with another initiative, or be rejected.

No implementation or publication commitment is implied by its acceptance for further consideration.

---

## 6. Stage 02 — Proposal

### 6.1 Objective

The proposal defines what the project intends to investigate, develop, or demonstrate.

It establishes a shared understanding of the project's purpose and boundaries before significant resources are committed.

### 6.2 Project Definition

A proposal should contain, where relevant:

**Project Identity**
- Project name.
- Short description.
- Project category.
- Current Project Status.
- Responsible maintainer.

**Purpose**
- Problem statement or research question.
- Context and motivation.
- Intended contribution.
- Relevance to the Lab's mission.

**Objectives**
- Primary objective.
- Secondary objectives.
- Expected outcomes.
- Success criteria, where meaningful.

**Scope**
- Included functionality or research activities.
- Explicit exclusions.
- Intended users or audience, if applicable.
- Expected level of completeness.

**Technical Direction**
- Proposed technologies.
- Potential architecture.
- External dependencies.
- Data requirements.
- Model or service requirements, where relevant.

**Constraints and Risks**
- Technical limitations.
- Resource requirements.
- Privacy considerations.
- Security considerations.
- Intellectual property and licensing concerns.
- Potential operational dependencies.

### 6.3 Feasibility Review

The proposal should be reviewed according to:

- Strategic relevance.
- Technical feasibility.
- Research or creative value.
- Resource requirements.
- Potential risks.
- Expected maintenance implications.

The level of analysis should remain proportionate to the project.

### 6.4 Stage Exit

The project may be:

- Approved for exploration.
- Revised before progression.
- Deferred.
- Combined with another initiative.
- Rejected.

The Founder and Maintainer retains final approval authority under the Lab's governance model.

---

## 7. Stage 03 — Discovery and Feasibility

### 7.1 Objective

Discovery investigates the assumptions underlying the proposal.

The purpose is to determine whether the project is technically and conceptually viable before committing to substantial implementation.

### 7.2 Research Activities

Depending on the project, discovery may include:

- Literature and documentation reviews.
- Technology and framework evaluations.
- API and integration assessments.
- Existing solution comparisons.
- Architecture exploration.
- Data availability assessment.
- Preliminary performance testing.
- Prototype sketches.
- Proof-of-concept development.
- Risk assessment.
- Licensing and dependency review.

### 7.3 Assumption Validation

Important assumptions should be identified and tested.

Examples include:

- Whether a required API supports the intended functionality.
- Whether a selected model performs sufficiently well for the target task.
- Whether a proposed architecture can support the expected interactions.
- Whether the necessary data is available and legally usable.
- Whether a technical approach is reproducible.
- Whether the solution can operate within available resources.

### 7.4 Feasibility Categories

A project may be assessed as:

| Assessment | Meaning |
|---|---|
| Feasible | The proposed direction appears technically and operationally viable |
| Feasible with Constraints | Viable subject to identified limitations or changes |
| Uncertain | Additional investigation is necessary |
| Not Feasible | Current assumptions or constraints prevent meaningful progression |

### 7.5 Expected Output

Discovery may produce:

- Research notes.
- Technical comparisons.
- Proofs of concept.
- Architecture sketches.
- Risk assessments.
- Feasibility conclusions.
- Revised project scope.

### 7.6 Stage Exit

The project may proceed to experimentation and development, return for proposal revision, remain under investigation, or be discontinued.

A negative feasibility result is a valid outcome when supported by evidence.

---

## 8. Stage 04 — Experimentation and Development

### 8.1 Objective

This stage transforms the approved direction into an experiment, prototype, tool, or working implementation.

The focus is on testing assumptions, exploring implementation choices, and producing demonstrable results.

### 8.2 Development Approach

Work may include:

- Software implementation.
- Interface and interaction development.
- AI integration.
- Model experimentation.
- Data processing.
- Workflow automation.
- Technical prototyping.
- System integration.
- Performance exploration.
- Creative experimentation.

Implementation should follow the relevant development and quality practices established by the Lab.

### 8.3 Incremental Development

Where practical, work should be divided into manageable iterations.

Each iteration should aim to produce an identifiable improvement, tested component, or documented finding.

Changes should be reviewed for:

- Functional correctness.
- Maintainability.
- Dependencies.
- Security implications.
- Data handling.
- Compatibility.
- Technical limitations.

### 8.4 Experiment Documentation

Experiments should record relevant information, including:

- Objective.
- Hypothesis or working assumption, if applicable.
- Experimental configuration.
- Tools and dependencies.
- Model identifiers and relevant versions.
- Inputs and data sources.
- Test conditions.
- Observed results.
- Known limitations.
- Unexpected behavior.

The amount of documentation should reflect the experiment's complexity and importance.

### 8.5 Iteration and Scope Changes

Project scope may evolve as new findings emerge.

Material changes should be reviewed to determine whether they affect:

- Original objectives.
- Technical architecture.
- Resources.
- Risk exposure.
- Data requirements.
- Intellectual property.
- Expected publication.
- Maintenance obligations.

Significant changes should be documented.

Changes involving new confidential material, sensitive data, or materially different publication risks require renewed review.

### 8.6 Stage Exit

The project may progress to validation when the intended experiment or implementation has reached a sufficiently stable state for meaningful evaluation.

It may also remain experimental, return to discovery, or be discontinued.

---

## 9. Stage 05 — Validation and Evaluation

### 9.1 Objective

Validation determines whether the project has achieved its intended objectives and whether its claims are supported by evidence.

The appropriate evaluation method depends on the type of project.

### 9.2 Technical Validation

Software and technical projects may be assessed through:

- Functional testing.
- Integration testing.
- Regression testing.
- Performance evaluation.
- Compatibility checks.
- Error handling.
- Accessibility evaluation, where applicable.
- Security review.
- Dependency checks.
- Reproducibility assessment.

Not every project requires all of these tests.

### 9.3 Research Validation

Research-oriented projects may be assessed through:

- Hypothesis evaluation.
- Comparison with baselines.
- Experimental repetition.
- Analysis of observed results.
- Evaluation of alternative explanations.
- Review of methodological limitations.
- Reproducibility checks.

Claims should reflect the strength and limitations of the available evidence.

### 9.4 AI System Evaluation

AI-enabled projects may require additional validation, such as:

- Output quality assessment.
- Model behavior testing.
- Prompt and configuration evaluation.
- Hallucination analysis.
- Robustness testing.
- Adversarial input testing.
- Bias and fairness considerations, where relevant.
- Data leakage assessment.
- Tool-use and agent permission testing.
- Human evaluation.

AI performance should not be judged solely through a small number of successful demonstrations.

### 9.5 Creative and Experiential Evaluation

Projects involving creative technology, interaction design, or digital experiences may also require qualitative evaluation.

Relevant criteria may include:

- Coherence of the creative concept.
- Quality of the interaction.
- Clarity of the experience.
- Responsiveness.
- Accessibility.
- Perceptual and aesthetic qualities.
- Alignment between intended and observed outcomes.

Not every creative result can or should be reduced to numerical metrics.

### 9.6 Evaluation Outcomes

Validation may result in:

- **Validated:** Defined objectives have been achieved with sufficient evidence.
- **Partially Validated:** Some objectives have been achieved, while others remain unresolved.
- **Not Validated:** Available evidence does not support the intended result.
- **Inconclusive:** Insufficient evidence is available to reach a reliable conclusion.

These are evaluation outcomes, not additional Project Status values. The canonical Project Status vocabulary remains defined in Section 14.

### 9.7 Expected Output

Validation may produce:

- Test results.
- Evaluation reports.
- Research findings.
- Performance measurements.
- Known limitations.
- Outstanding issues.
- Recommendations.
- A revised project assessment.

### 9.8 Stage Exit

A project may proceed to publication review when its intended release scope has been sufficiently evaluated.

A project may also remain experimental or be discontinued without publication.

Validation does not automatically authorize public release.

---

## 10. Stage 06 — Publication Review

### 10.1 Objective

Publication review determines whether a project or part of a project is appropriate for public release.

This is a distinct decision from technical completion.

The review considers what is being published, under which conditions, and with what responsibilities.

### 10.2 Publication Readiness

Before publication, the maintainer should review the following areas.

**Scope and Documentation**
- Is the published material clearly identified?
- Is its purpose understandable?
- Are limitations and maturity communicated?
- Are the relevant instructions available?
- Are unsupported claims avoided?

**Technical Quality**
- Has the relevant functionality been tested?
- Are obvious defects addressed or documented?
- Are dependencies identified?
- Is the project structure understandable?
- Is there unnecessary or sensitive material in the release?

**Security**
- Have secrets and credentials been removed?
- Have access permissions been reviewed?
- Have security-sensitive configurations been considered?
- Are known vulnerabilities addressed or clearly disclosed?

**Privacy and Data**
- Is personal data handled appropriately?
- Are data sources identified?
- Are data-use rights established?
- Have private datasets and confidential material been excluded?
- Are retention and processing considerations documented where relevant?

**Intellectual Property and Licensing**
- Is ownership or permission to publish sufficiently clear?
- Are third-party licenses compatible with the intended distribution?
- Are attribution requirements fulfilled?
- Are generated or contributed assets appropriately reviewed?
- Are project-specific usage conditions documented?

**External Dependencies**
- Are external APIs and services identified?
- Have relevant terms and restrictions been reviewed?
- Are credentials handled securely?
- Are externally hosted assets or services appropriately referenced?

**Public Communication**
- Does the description accurately represent the project?
- Are claims supported by evidence?
- Are known risks and limitations visible?
- Is the publication status clear?

### 10.3 Confidentiality Boundary

The public Lab must remain separate from proprietary and confidential work.

Before release, the maintainer must ensure that the project does not expose:

- Private source code.
- Confidential architecture or implementation details.
- Internal business information.
- Unpublished research material.
- Private user or client data.
- Credentials and infrastructure information.
- Restricted assets or third-party materials.

A public project must be independently suitable for publication.

The existence of related private work does not authorize the transfer of its implementation or confidential details into the Lab.

### 10.4 Publication Decision

The review may result in:

- Approved for publication.
- Approved with documented limitations.
- Approved after specified corrections.
- Deferred pending additional review.
- Rejected for publication.

Unresolved ownership, licensing, privacy, security, or confidentiality issues prevent publication until adequately addressed.

The detailed Publication Classification and Publication Status must be recorded according to `PUBLICATION-POLICY-v2.0.md`.

### 10.5 Approval Authority

Final publication authorization rests with the Founder and Maintainer under the Lab's governance model.

A technical review, successful demonstration, or contributor recommendation does not independently authorize publication.

---

## 11. Stage 07 — Publication and Release

### 11.1 Objective

Publication makes an approved project or result publicly available.

The release should accurately communicate the project's purpose, maturity, requirements, and limitations.

### 11.2 Publication Formats

Depending on the project, publication may involve:

- Source code.
- Documentation.
- Research reports.
- Technical notes.
- Demonstrations.
- Prototypes.
- Downloadable tools.
- Releases and packaged assets.
- Public presentations.

Publication does not necessarily mean distributing an entire source code repository.

An approved research result may be published separately from the underlying implementation.

### 11.3 Release Requirements

A release should identify, where relevant:

- Project name.
- Release or version identifier.
- Publication date.
- Current Project Status.
- Main capabilities.
- Requirements and dependencies.
- Setup instructions.
- Known limitations.
- Licensing and usage information.
- Relevant documentation.
- Security or privacy considerations.

### 11.4 Versioning

Where software is released in multiple versions, a consistent versioning approach should be used.

Semantic Versioning may be appropriate for software with a defined public interface and compatibility expectations.

Other projects may use simpler release identifiers, dates, milestones, or research iteration numbers.

Versioning should communicate meaningful changes rather than create administrative overhead.

### 11.5 Release Notes

Material releases should include release notes describing relevant changes.

These may include:

- New features.
- Improvements.
- Corrections.
- Breaking changes.
- Dependency changes.
- Known limitations.
- Security-related updates.

### 11.6 Publication Review Does Not End at Release

Publication is not a permanent guarantee that a project remains suitable for every use.

The maintainer may revise documentation, issue corrections, restrict access, or withdraw material when new information creates a material concern.

---

## 12. Stage 08 — Maintenance and Evolution

### 12.1 Objective

Maintenance covers the period during which a published project continues to receive corrections, improvements, or other updates.

Not all projects require ongoing maintenance.

The expected support level should be communicated clearly.

### 12.2 Maintenance Activities

Where applicable, maintenance may include:

- Bug fixes.
- Dependency updates.
- Security corrections.
- Compatibility improvements.
- Documentation updates.
- Performance improvements.
- Accessibility improvements.
- Model or API adjustments.
- Infrastructure changes.
- Feature development.

### 12.3 Maintenance Priorities

Maintenance priorities may consider:

1. Security and privacy vulnerabilities.
2. Critical functional failures.
3. Data integrity issues.
4. Significant compatibility problems.
5. Documentation defects.
6. General improvements and feature requests.

The actual priority depends on the project's status, risk, and available resources.

### 12.4 External Dependencies

Projects depending on third-party services may be affected by:

- API changes.
- Model retirement.
- Pricing changes.
- Service interruptions.
- Licensing changes.
- Dependency vulnerabilities.
- Provider policy changes.

Such dependencies should be documented where they materially affect project behavior or continued operation.

### 12.5 Maintenance Expectations

A published project should not imply guaranteed ongoing support unless such a commitment has been explicitly established.

The project documentation should distinguish between:

- Actively maintained projects.
- Projects receiving occasional updates.
- Projects with limited support.
- Archived projects.
- Discontinued projects.

### 12.6 Material Changes

Significant changes to functionality, architecture, data handling, or project purpose may require renewed evaluation and publication review.

---

## 13. Stage 09 — Archival or Discontinuation

### 13.1 Objective

A project may reach a point where continued development is no longer useful, feasible, or justified.

Archival or discontinuation provides a controlled way to close the lifecycle while preserving relevant knowledge.

### 13.2 Reasons for Archival or Discontinuation

Possible reasons include:

- Completion of the research objective.
- Replacement by a more suitable approach.
- Technical obsolescence.
- Lack of available resources.
- Unresolved external dependencies.
- Changes in project priorities.
- Security or privacy concerns.
- Inability to maintain the project responsibly.
- Discovery that the original assumptions were incorrect.

### 13.3 Archived Projects

An archived project is retained for reference but is no longer actively developed.

Where applicable, archival should include:

- A clear Archived Project Status.
- The date of archival.
- The reason for archival, where appropriate.
- The final supported version, if relevant.
- Known limitations.
- Important dependencies.
- Relevant documentation.
- A statement about maintenance expectations.

External deployments, access tokens, and unnecessary credentials should be disabled or revoked where appropriate.

### 13.4 Discontinued Projects

A discontinued project is no longer intended to receive further development.

Depending on its condition, it may be archived, withdrawn, or removed from public distribution.

A discontinued project should not continue to be presented as actively maintained.

### 13.5 Preserving Research Value

Where appropriate, the Lab should preserve useful knowledge generated by a project.

This may include:

- Research conclusions.
- Experimental results.
- Technical lessons.
- Failed approaches.
- Architectural decisions.
- Evaluation reports.
- Reusable non-confidential components.

Preservation must respect intellectual property, privacy, confidentiality, and licensing restrictions.

### 13.6 Withdrawal

Public material may be withdrawn when continuing publication presents an unacceptable risk or violates applicable rights or obligations.

Withdrawal may be appropriate when:

- Sensitive information has been exposed.
- A licensing or ownership issue is identified.
- Security risks cannot be adequately mitigated.
- Publication was unauthorized.
- Legal or contractual obligations require removal.

Where appropriate, the Project Status and relevant documentation should be updated to explain the withdrawal without revealing additional sensitive information.

---

## 14. Project Status Definitions

Project Status records the current state of the project. It is not a substitute for Lifecycle Stage, Technical Maturity, Operational Readiness, Publication Classification, or Publication Status.

Use the definitions below as the sole canonical Project Status vocabulary across the Lab's documentation.

| Status | Definition |
|---|---|
| Proposed | An idea or project proposal awaiting evaluation |
| Concept | An early-stage concept under exploration |
| Experimental | An active experiment or technical exploration |
| Prototype | A demonstrable implementation used to evaluate an approach |
| Development | An actively evolving implementation |
| Validation | A project undergoing structured testing or evaluation |
| Published | An approved project or result available publicly |
| Maintenance | A published project receiving ongoing updates |
| Archived | A project retained for reference without active development |
| Discontinued | A project formally closed and no longer intended for development |

A project may use a subset of these statuses.

The status should reflect actual project activity and maturity rather than an intended future condition.

Status labels do not constitute security ratings, product certifications, or commercial readiness claims.

### 14.1 Status and Lifecycle Stage Are Independent

A Project Status does not automatically determine a Lifecycle Stage.

For example, a project marked `Experimental` may be within Discovery and Feasibility or Experimentation and Development, depending on its actual activities.

Likewise, a project may enter Publication Review without being publicly available, and a project may be `Archived` after its active lifecycle has ended.

The current state and the workflow position must therefore be recorded separately.

### 14.2 Status Changes

A Project Status should be changed when the actual condition of the project changes.

Status changes should be supported by the project record and must not be used to imply:

- Technical validation that has not occurred.
- Operational readiness that has not been assessed.
- Publication approval that has not been granted.
- Maintenance commitments that have not been established.

---

## 15. Project Documentation Requirements

Documentation should support understanding, evaluation, continuity, and responsible use.

The appropriate documentation level depends on the project.

### 15.1 Minimum Project Record

A project record should generally identify:

- Name.
- Description.
- Purpose.
- Current Project Status.
- Objectives.
- Scope.
- Responsible maintainer.
- Main technologies or methods.
- Relevant dependencies.
- Known limitations.
- Current Lifecycle Stage.

### 15.2 Additional Documentation

More complex projects may require:

- Research specifications.
- Technical architecture.
- Design documentation.
- Experiment records.
- Test reports.
- Evaluation findings.
- Security considerations.
- Data documentation.
- Decision records.
- Release notes.
- Maintenance instructions.

### 15.3 Documentation Accuracy

Documentation must reflect the actual implementation and current status.

Outdated instructions, unsupported claims, and undocumented limitations should be corrected when identified.

Experimental findings must remain distinguishable from validated conclusions.

The standard project documentation structure is provided in `PROJECT-TEMPLATE-v2.0.md`.

---

## 16. Risk Management Throughout the Lifecycle

Risk assessment is not limited to publication review.

Relevant risks should be considered from the earliest stages and reassessed as the project evolves.

Potential risk areas include:

- Technical feasibility.
- Security vulnerabilities.
- Privacy and personal data.
- Intellectual property.
- Licensing.
- External dependencies.
- AI system behavior.
- Ethical considerations.
- Operational continuity.
- Resource requirements.
- Public interpretation and misuse.

The level of risk assessment should reflect potential impact.

A change introducing new external access, sensitive information, or autonomous execution may require additional review even when the original project was low-risk.

Applicable requirements are defined in the relevant Lab policies, including `SECURITY-v2.0.md`, `RESPONSIBLE-AI-v2.0.md`, and `PUBLICATION-POLICY-v2.0.md`.

---

## 17. Exceptions and Proportionate Implementation

The lifecycle is a framework rather than an inflexible administrative procedure.

Exceptions may be appropriate for:

- Small exploratory experiments.
- Temporary proofs of concept.
- Documentation-only contributions.
- Creative demonstrations.
- Short-lived technical investigations.
- Projects with limited scope and no public deployment.

An exception should not bypass fundamental obligations concerning:

- Intellectual property.
- Confidentiality.
- Security.
- Privacy.
- Publication authorization.
- Applicable law.

Where a stage is skipped, the decision should remain proportionate to the project's complexity and risk.

---

## 18. Roles and Responsibilities

Lifecycle responsibilities follow the Lab's governance model, as defined in `GOVERNANCE-v2.0.md`.

### Founder and Maintainer

The Founder and Maintainer is responsible for:

- Approving projects for significant development.
- Establishing or confirming project scope.
- Reviewing material changes.
- Determining Project Status.
- Approving publication.
- Reviewing archival or discontinuation decisions.
- Ensuring applicable policies are considered.
- Maintaining appropriate project documentation.

### Contributors

Contributors are expected to:

- Work within the agreed project scope.
- Follow the relevant development and research practices.
- Document significant changes and findings.
- Respect intellectual property and confidentiality requirements.
- Report important risks or technical limitations.
- Participate constructively in evaluation and review.

### Collaborators

Collaborators should follow the responsibilities and boundaries established for their agreed project scope.

Specific arrangements may be documented separately.

---

## 19. Relationship with Other Policies

This document should be read alongside:

| Document | Purpose |
|---|---|
| `README.md` | Lab mission, scope, and identity |
| `LAB-CHARTER-v2.0.md` | Foundational principles and institutional direction |
| `GOVERNANCE-v2.0.md` | Decision-making authority and responsibilities |
| `QUALITY-STANDARDS-v2.0.md` | Technical Maturity, Operational Readiness, and quality expectations |
| `PROJECT-TEMPLATE-v2.0.md` | Standard project documentation structure |
| `PUBLICATION-POLICY-v2.0.md` | Publication Classification, Publication Status, and release requirements |
| `RESEARCH-METHODOLOGY-v2.0.md` | Research and experimental practices |
| `CONTRIBUTING-v2.0.md` | Contribution process and expectations |
| `SECURITY-v2.0.md` | Security reporting and vulnerability handling |
| `CODE-OF-CONDUCT-v2.0.md` | Behavioral expectations and collaboration standards |
| `RESPONSIBLE-AI-v2.0.md` | Responsible AI requirements and risk considerations |

Where relevant, the requirements of these documents apply throughout the project lifecycle.

Technical quality and assessment must follow `QUALITY-STANDARDS-v2.0.md`.

Publication review must follow `PUBLICATION-POLICY-v2.0.md`.

Research and experiment evaluation should follow `RESEARCH-METHODOLOGY-v2.0.md`.

Security incidents must be handled according to `SECURITY-v2.0.md`.

---

## 20. Policy Review and Updates

This document may be updated as the Lab develops new project types, adopts new methodologies, or changes its operating model.

The Founder and Maintainer is responsible for approving and documenting changes in accordance with `GOVERNANCE-v2.0.md`.

Revisions should preserve the core objectives of the lifecycle:

- Clear project definition.
- Proportionate development practices.
- Evidence-based evaluation.
- Responsible publication.
- Sustainable maintenance.
- Preservation of useful knowledge.

Material revisions should update the version, status, effective date, and revision record as appropriate.

A revision to this document does not automatically change the status, maturity, readiness, or publication decision of an existing project. Relevant project records should be reassessed where the change materially affects them.

---

## 21. Closing Principle

A project is not defined only by what it produces.

Its value also lies in the question it explores, the assumptions it tests, the knowledge it generates, and the responsibility with which its results are shared.

The lifecycle gives this process a structure: from curiosity to investigation, from experimentation to evidence, and from publication to continuity.

Not every experiment needs to become a product. Not every prototype needs to become a release.

But every published result should have a clear purpose, an honest account of its maturity, and a responsible path forward.

**Explore with intention. Develop with discipline. Validate with evidence. Publish with responsibility.**
