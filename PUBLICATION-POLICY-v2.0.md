# Framing Creativity Lab — Publication Policy

**Document ID:** FCL-POL-001  
**Version:** 2.0  
**Status:** Draft for Maintainer Review  
**Effective Date:** Pending approval  
**Maintainer:** J-ART  
**Repository:** Framing Creativity Lab  
**Applies to:** All material intended for public distribution under the Framing Creativity Lab identity.

---

## 1. Purpose

This policy defines the requirements, review procedures, classification framework, and approval conditions governing the publication of work under the Framing Creativity Lab identity.

Its purpose is to ensure that public releases are intentional, appropriately reviewed, accurately documented, and consistent with the Lab's principles.

It establishes a controlled process for moving material from private development, research, or experimentation into a public environment.

The policy addresses:

- Publication eligibility.
- Intellectual property and ownership.
- Confidentiality and information protection.
- Source code and repository review.
- Data classification and privacy.
- Security and credential management.
- Third-party dependencies and licensing.
- Technical validation and evidence.
- Documentation and public communication.
- Publication classification and review status.
- Approval authority and release conditions.
- Publication maintenance and withdrawal.

The policy applies regardless of whether the material is presented as research, an experiment, a prototype, a proof of concept, a tool, an application, a technical demonstration, or documentation.

**Public visibility is a publication decision, not a default development setting.**

---

## 2. Scope and Application

### 2.1 Covered Material

This policy applies to all material intended for public distribution through Framing Creativity Lab, including:

- GitHub repositories.
- Source code and scripts.
- Applications and prototypes.
- AI experiments and workflows.
- Prompt collections and model configurations.
- Technical documentation.
- Architecture diagrams.
- Research reports and technical studies.
- Demonstrations and screenshots.
- Generated datasets and sample files.
- Build and deployment configurations.
- Releases, packages, and downloadable assets.
- Public websites and project documentation.
- Public presentations and other distributed materials.

It also applies to updates, patches, releases, and subsequent versions of previously published projects.

### 2.2 Covered Publication Channels

The policy applies to public distribution through:

- GitHub repositories and GitHub Pages.
- Public package registries.
- Public documentation websites.
- Public AI and model repositories.
- Public demonstration platforms.
- External services used to distribute Lab projects.
- Community platforms that display or synchronise public repositories.
- Any other channel through which Lab material is intentionally made publicly accessible.

Specific publication requirements may differ depending on the platform and the nature of the material.

### 2.3 Internal and Private Development

Private development environments are not publication channels.

The policy does not authorise the transfer, disclosure, or publication of private commercial projects, client materials, confidential work, or restricted research.

A project does not become eligible for publication simply because:

- It was developed independently.
- It uses publicly available technologies.
- It contains no obvious confidential information.
- It is stored in a repository controlled by the Lab.
- It has been technically completed.
- It has been reviewed by a contributor.
- It has previously been used in a demonstration.

Publication eligibility must be established separately for the exact material and scope proposed for release.

### 2.4 Public Repository Boundary

A public Lab repository must remain independent from private and proprietary development environments.

It must not be used as:

- A mirror of a private project.
- A staging area for confidential code.
- A distribution channel for client deliverables.
- A backup location for restricted technical assets.
- A place to publish private prompts or workflows.
- A means of indirectly disclosing internal architecture or business logic.

A public project must be suitable for publication on its own merits and under its own documented rights and conditions.

---

## 3. Fundamental Publication Principles

Every publication decision must follow these principles.

### 3.1 Intentional Publication

A project or material must be explicitly selected for public release.

Public accessibility must never result from accidental repository configuration, unintended synchronisation, an unreviewed visibility change, or an assumption that all Lab material is public.

### 3.2 Ownership Before Publication

The right to publish all included material must be established before release.

Possession of a file, codebase, dataset, model, or asset does not automatically confer publication or redistribution rights.

### 3.3 Confidentiality by Design

Confidential information must remain outside public repositories.

Removing names or identifying references does not necessarily remove the confidential nature of technical implementation details, workflows, architecture, or business information.

### 3.4 Technical Integrity

Published code and documentation must accurately represent the state and capabilities of the project.

Incomplete, experimental, or unstable implementations may be published when their status and limitations are explicitly communicated and the applicable publication requirements are satisfied.

### 3.5 Transparency

A publication should describe what it does, how it works, what it requires, what evidence supports its claims, and what limitations are known.

Claims must be proportionate to available evidence.

### 3.6 Responsible Distribution

Publication must consider downstream use, third-party rights, data protection, security, accessibility, and foreseeable misuse.

### 3.7 Continuous Responsibility

Publication approval is not permanent immunity from future review.

Repositories and releases must be reassessed when significant code, data, dependencies, licences, operating conditions, or project purposes change.

### 3.8 Minimum Necessary Disclosure

Publication should disclose what is useful and authorised for public understanding, not every detail available during development.

Sensitive implementation details, confidential information, unnecessary metadata, and restricted assets must remain excluded.

---

## 4. Publication Eligibility

A project may be considered for publication when all applicable eligibility conditions are satisfied.

### 4.1 Potentially Eligible Material

Examples include:

- Original independent experiments.
- Independently developed tools.
- Original research and technical notes.
- Self-contained software demonstrations.
- Public-domain or appropriately licensed resources.
- Independently developed prototypes.
- Reusable components with established ownership.
- Educational examples.
- Technical evaluations based on authorised resources.
- Documentation created for public distribution.

Eligibility depends on the actual contents, ownership, implementation, and publication conditions, not merely the project category.

### 4.2 Ineligible Material

The following must not be published without a separate, documented, and valid authorization establishing the right to do so:

- Proprietary commercial source code.
- Confidential client deliverables.
- Private product architectures.
- Restricted internal documentation.
- Commercial business logic.
- Unreleased product specifications.
- Non-public research owned by another party.
- Private datasets.
- Unauthorised third-party code or assets.
- Credentials and access secrets.
- Private AI workflows or configurations.
- Material subject to contractual or legal restrictions.
- Personal information without an appropriate publication basis.
- Content whose ownership or publication rights are unclear.

Where authorization cannot be established, publication must be withheld.

### 4.3 Independent Implementation Requirement

An experiment may investigate a general concept that is also relevant to another private project.

However, the public implementation must be independently developed and reviewed.

It must not contain copied proprietary implementation details, confidential workflows, protected assets, internal documentation, or restricted configurations.

A similar idea does not justify the reuse of protected material.

Where independence cannot be established with reasonable confidence, publication must be withheld pending further review.

### 4.4 Eligibility Is Scope-Specific

A project may contain both eligible and ineligible components.

Publication may be considered for a clearly defined, independently suitable subset only when:

- The proposed subset is separable.
- Its ownership and publication rights are established.
- The removal of restricted components does not disclose protected information.
- No confidential dependencies remain embedded in the published material.
- The resulting publication can be accurately described.
- The revised scope receives a new or renewed review.

The existence of eligible components does not make the entire project eligible.

---

## 5. Publication Classification

Every proposed publication must receive a Publication Classification before the final review decision.

The classification determines the level of publication scrutiny and the restrictions that apply.

### 5.1 Canonical Classification Levels

| Level | Classification | General meaning |
|---|---|---|
| P0 | Public-ready | Independent, low-risk material with established publication rights and no unresolved publication restrictions. |
| P1 | Controlled publication | Material requiring additional checks, defined controls, or specific release conditions that must be satisfied before publication. |
| P2 | Restricted review | Material presenting unresolved ownership, security, privacy, confidentiality, or other material publication concerns. |
| P3 | Non-publishable | Material that is excluded from the public publication process in its current form. |

These four values are the Lab's canonical Publication Classification vocabulary.

They are not Project Status values, Technical Maturity values, Operational Readiness values, or AI Risk Classification values.

### 5.2 P0 — Public-Ready

P0 applies to independent, low-risk material whose publication rights and relevant publication conditions have been established.

Potential examples:

- Original standalone code.
- Independent technical experiments.
- Publicly licensed examples used within their licence terms.
- General technical documentation.
- Self-contained demonstrations without sensitive dependencies.
- Original creative or research material with established publication rights.

Expected review:

- Ownership and publication-rights check.
- Repository and content inspection.
- Appropriate credential and secret checks.
- Third-party dependency review.
- Documentation review.
- Relevant technical checks.
- Publication checklist completion.

P0 does not mean that a project is validated, production-ready, or free from all possible defects.

It means that the proposed material meets the applicable publication conditions without additional P1-specific controls.

### 5.3 P1 — Controlled Publication

P1 applies to material that may be publishable but requires additional checks or specific controls because of its technical, data, integration, operational, or distribution context.

Potential examples:

- Experiments using external APIs.
- AI applications interacting with third-party models.
- Projects using external datasets.
- Applications involving authorised user-submitted information.
- Projects containing complex third-party dependencies.
- Demonstrations deployed through external services.
- Projects relying on provider-specific terms or operating conditions.
- Applications requiring clearly defined limitations or user safeguards.

P1 is a controlled publication category, not an unresolved-risk category.

A P1 publication may proceed only when all applicable conditions in Section 14 have been completed, reviewed, and recorded.

Additional review may include:

- Data-flow assessment.
- External service and API terms.
- Licence compatibility.
- Privacy implications.
- Security configuration.
- Permission boundaries.
- Operational dependencies.
- Human oversight, where relevant.
- User-facing limitations.
- Monitoring or withdrawal considerations.
- Defined release scope and conditions.

**P1 publication conditions are mandatory. A P1 classification alone does not authorize publication.**

If a material concern remains unresolved, the material must remain under PENDING review or be reclassified P2 or P3 as appropriate.

### 5.4 P2 — Restricted Review

P2 applies when material has unresolved questions or risks that prevent publication approval.

Potential examples:

- Projects containing material with uncertain ownership.
- Experiments derived from confidential development environments.
- Applications involving potentially sensitive datasets without established authorization.
- Projects with unresolved security concerns.
- Repositories with unexplained third-party material.
- Codebases where separation from proprietary work cannot be established.
- Material with unresolved privacy or contractual restrictions.
- Publications whose risk cannot be adequately assessed.

P2 material must remain unpublished.

It must not be released through a public repository, demonstration, downloadable asset, public documentation page, or another distribution channel while the relevant concerns remain unresolved.

The existence of a P2 classification does not guarantee eventual publication.

A P2 classification may be reconsidered only after:

1. The reason for the restricted classification has been identified.
2. The relevant issue or risk has been resolved or demonstrably removed.
3. Supporting evidence or authorization has been obtained.
4. The affected material and publication scope have been reviewed again.
5. A new classification decision has been recorded.
6. The publication review has been repeated as necessary.
7. The maintainer has issued a new publication decision.

A change from P2 to P0 or P1 must not be made solely to permit publication.

The reassessment must demonstrate that the original reasons for restriction no longer prevent the proposed release.

### 5.5 P3 — Non-Publishable

P3 applies to material that must not enter the public Lab environment in its current form.

Potential examples:

- Confidential commercial source code.
- Unauthorised client data.
- Private credentials.
- Material that cannot legally or contractually be distributed.
- Proprietary implementation details without publication permission.
- Unauthorised personal information.
- Restricted third-party resources.
- Material whose disclosure would create unacceptable security or confidentiality exposure.

P3 material is excluded from the public publication process.

It must not be moved into a public repository for convenience, demonstration, partial disclosure, or temporary storage.

A P3 classification cannot be removed through an administrative label change or an informal approval.

Where a substantially revised or independently developed body of work is proposed, it must be treated as a new publication scope and undergo a complete eligibility and classification review.

The original restricted material remains excluded unless the necessary rights and authorizations have been explicitly established.

---

## 6. Publication Status

Publication Status records the current publication review state or decision.

The four canonical values are:

| Status | Definition |
|---|---|
| PENDING | Publication review or decision is incomplete. No publication authorization has been granted. |
| APPROVED | Publication has been explicitly authorized for the defined material and scope, subject to the recorded conditions. |
| REJECTED | The proposed publication has not been authorized. |
| WITHDRAWN | A previous publication approval or authorization has been withdrawn. This may also apply to material already released. |

### 6.1 PENDING

PENDING is the default status for a proposed publication that has not completed review.

It may be used while:

- Ownership is being established.
- Classification is being assessed.
- Technical or security checks are underway.
- Additional permissions are being obtained.
- P1 conditions are being verified.
- Documentation or release scope is being completed.

PENDING is not conditional approval.

No material under PENDING may be published.

### 6.2 APPROVED

APPROVED means that the maintainer has authorized publication of the precisely defined material and scope.

Approval must be supported by a completed review record.

For P1, all mandatory conditions must have been satisfied before the status becomes APPROVED.

Approval does not automatically mean that the material has already been released.

The actual public release must be recorded separately.

### 6.3 REJECTED

REJECTED means that the proposed publication has not been authorized.

The rejection record should identify the main reasons and relevant restrictions without exposing confidential information.

A rejected proposal may be reconsidered after a material change, new evidence, or resolution of the relevant issue.

A new review must be recorded. A previous rejection must not be silently replaced with an approval.

### 6.4 WITHDRAWN

WITHDRAWN applies when a previously granted publication approval or authorization is revoked.

Possible reasons include:

- Newly discovered ownership or licensing restrictions.
- Security or privacy concerns.
- Confidentiality exposure.
- Material changes to the approved scope.
- Inaccurate or misleading publication claims.
- Legal or contractual requirements.
- A decision to stop distributing the material.

If the material has already been released, the withdrawal procedure in Section 20 applies.

### 6.5 Status Transitions

The general publication decision sequence is:

**PENDING → APPROVED**

or

**PENDING → REJECTED**

A previously granted approval may later become:

**APPROVED → WITHDRAWN**

A new proposal following rejection or withdrawal must be reviewed again and recorded separately where appropriate.

The publication status must describe the current review decision, not the project's development state.

### 6.6 Separation from Other Project Fields

Publication Status must remain independent from:

- Lifecycle Stage.
- Project Status.
- Technical Maturity.
- Operational Readiness.
- Publication Classification.
- AI Risk Classification.

The authoritative definitions are maintained in the relevant specialist documents:

| Attribute | Authoritative document |
|---|---|
| Lifecycle Stage | `PROJECT-LIFECYCLE-v2.0.md` |
| Project Status | `PROJECT-LIFECYCLE-v2.0.md` |
| Technical Maturity | `QUALITY-STANDARDS-v2.0.md` |
| Operational Readiness | `QUALITY-STANDARDS-v2.0.md` |
| Publication Classification | This document |
| Publication Status | This document |
| AI Risk Classification | `RESPONSIBLE-AI-v2.0.md` |

No field should be inferred solely from another.

---

## 7. Standard Publication Review Process

All proposed publications must follow a review process appropriate to their scope and classification.

### 7.1 Standard Workflow

**1. Project Identification**

Define the project, material, or specific release being considered.

**2. Ownership Assessment**

Establish authorship, ownership, publication rights, and relevant permissions.

**3. Scope Assessment**

Identify the exact files, assets, documentation, dependencies, data, and release artefacts to be distributed.

**4. Risk and Classification Assessment**

Assess relevant publication risks and assign P0, P1, P2, or P3.

**5. Content Review**

Inspect source code, data, configuration, documentation, metadata, history, and associated assets.

**6. Security and Privacy Review**

Evaluate credentials, access controls, data flows, external services, and relevant security or privacy concerns.

**7. Technical Validation**

Test or evaluate the implementation sufficiently to support its stated capabilities and limitations.

**8. Documentation Review**

Confirm that the README and supporting documentation accurately describe the project, its scope, dependencies, and limitations.

**9. Final Decision**

Determine whether all applicable conditions are satisfied and record the maintainer's approval, rejection, or continued pending status.

**10. Publication**

Release only the approved material through the intended public channel.

**11. Post-Publication Review**

Consider feedback, defects, security reports, new dependencies, material changes, and withdrawal requirements.

### 7.2 Mandatory Review Gate

Publication must not proceed if any mandatory requirement remains unresolved.

A project may be technically complete while still being unsuitable for publication.

Documentation completeness cannot compensate for unresolved ownership or confidentiality concerns.

A successful technical demonstration does not replace a publication review.

### 7.3 Scope Control

Approval applies only to the material and scope that were reviewed.

Adding any of the following may trigger a new review:

- New datasets.
- New assets.
- Major features.
- External integrations.
- New AI models or services.
- New permissions or access capabilities.
- Additional distribution channels.
- Material changes to the intended audience or use.
- Significant changes to the project's architecture or data processing.

### 7.4 Review Evidence

Material publication decisions should be supported by a record identifying the scope, classification, principal checks, findings, and decision.

The record should provide enough information to demonstrate that the relevant publication requirements were considered without reproducing restricted material.

---

## 8. Intellectual Property and Ownership Review

Before publication, the maintainer must establish the rights associated with every significant component.

### 8.1 Ownership Questions

The review should establish:

- Who created the original work?
- Who owns the relevant intellectual property?
- Was the work created under a contract or employment arrangement?
- Are any third-party components included?
- Are redistribution rights available?
- Are there contractual confidentiality obligations?
- Are there restrictions on derivative works?
- Does the project include generated material subject to external terms?
- Are there contributor permissions or agreements?
- Are attribution requirements fulfilled?

### 8.2 Original Work

Original work may be published when the author has the appropriate rights and no conflicting obligations apply.

The fact that a project is described as independent does not remove the need to verify its actual contents and development history.

### 8.3 Third-Party Work

Third-party material must be reviewed individually.

Its inclusion must respect applicable licences, attribution requirements, redistribution permissions, usage restrictions, and relevant contractual terms.

### 8.4 AI-Generated Material

AI-generated output must not automatically be assumed to be free of third-party rights or other restrictions.

Relevant model, service, and asset-generation terms should be reviewed where material is intended for redistribution.

Where necessary, document the source, model, provider, generation context, and applicable usage conditions without disclosing restricted information.

### 8.5 Contributions

A contribution does not automatically transfer ownership to the Lab.

Submission, review, acceptance, or inclusion in a repository does not independently grant the Lab unrestricted permission to reproduce, modify, distribute, sublicense, or commercially exploit the contribution.

The rights required for the intended publication must be established through an applicable licence or explicit written agreement.

If the required permissions are not established, the contribution must not be published.

### 8.6 Ownership Uncertainty

Where ownership or permission cannot be established, the material must not be published until the uncertainty is resolved.

An assumption that a contribution is free to use is not sufficient evidence.

### 8.7 No Implied Open-Source Licence

The public Framing Creativity Lab repository currently has no general open-source licence.

Public availability does not, by itself, grant permission to reproduce, modify, distribute, sublicense, or commercially exploit original material.

Any project-specific licence or rights statement must be explicit and must identify the material it covers.

This publication policy does not create a general licence.

---

## 9. Confidentiality and Information Security Review

Confidentiality review must cover the complete publication context, not only the main source files.

### 9.1 Source Code

Inspect source files for:

- Proprietary business logic.
- Internal service references.
- Private application integrations.
- Non-public architecture.
- Internal identifiers.
- Confidential algorithms.
- Unreleased implementation details.
- Private workflows.
- Restricted prompts or instructions.

### 9.2 Configuration

Inspect:

- Environment files.
- Configuration examples.
- Build settings.
- Deployment configurations.
- Infrastructure references.
- API endpoints.
- Authentication mechanisms.
- Service identifiers.
- Internal hostnames and paths.
- Permission and access settings.

Sensitive values must never be committed.

Use environment variables and safe configuration examples where appropriate.

### 9.3 Documentation and Supporting Material

Inspect:

- README files.
- Technical specifications.
- Architecture documentation.
- Development notes.
- Diagrams.
- Screenshots.
- Generated documentation.
- Test fixtures.
- Sample files.
- Demonstration recordings.
- Metadata and exported reports.

Documentation can expose confidential information even when source code does not.

### 9.4 Git History

The review should consider repository history where relevant.

Sensitive information may remain in:

- Previous commits.
- Deleted files.
- Branches.
- Tags.
- Release assets.
- Historical configuration.
- Git objects.
- Commit messages.

Removing a file from the current branch does not guarantee that historical copies are no longer accessible.

Where a secret has been exposed, revocation or rotation is required. History cleanup alone does not invalidate an exposed credential.

### 9.5 Repository Metadata

Review:

- Repository name.
- Description.
- Topics.
- Branch names.
- Commit messages.
- Workflows and automation.
- Issues and discussions.
- Releases.
- Project URLs.
- Public configuration.
- Badges and external references.

All visible metadata must be appropriate for public release.

### 9.6 Independent Confidentiality Review

The maintainer should consider whether the proposed publication could reveal private work indirectly through:

- File naming.
- Internal identifiers.
- Similarity to proprietary architecture.
- Extracted technical patterns.
- Screenshots or visual references.
- Development history.
- External service configurations.
- Hidden metadata.

A material can be confidential even when it contains no personal names or obvious secrets.

---

## 10. Data Classification and Privacy Review

Projects involving data must establish an appropriate basis for its use and publication.

Data must be classified before it is included in a public release or transmitted to an external service.

### 10.1 Canonical Data Classification

The Lab uses the following four data classification levels:

| Classification | Description | General treatment |
|---|---|---|
| Public | Information explicitly approved or otherwise authorized for public distribution. | May be published subject to source rights and applicable restrictions. |
| Internal | Non-public working information intended for authorized Lab use. | Excluded from public release unless separately reviewed and authorized. |
| Confidential | Information subject to confidentiality obligations, restricted access, or material disclosure risk. | Must remain restricted unless the necessary rights and explicit authorization for the proposed use are established. |
| Restricted | Highly sensitive, legally or contractually restricted, security-critical, or otherwise unsuitable for ordinary disclosure. | Must not be placed in public repositories or submitted to external services without an explicitly established basis, authorization, and appropriate safeguards. |

These four values are the canonical data classification vocabulary used by the Lab.

### 10.2 Personal and Sensitive Information

Personal information and sensitive information are characteristics of data. They are not additional values in the four-level data classification vocabulary.

They must be assessed separately when assigning the applicable data classification.

As an internal handling rule:

- Personal information should be classified at least as Confidential.
- Sensitive personal information, security-critical information, or information subject to stricter restrictions should be classified as Restricted.
- Any stricter owner, contractual, legal, or regulatory classification takes precedence.

Removing direct identifiers does not automatically make personal information anonymous.

### 10.3 Data Classification Before Publication

Before release, the maintainer should establish:

- The source of the data.
- The owner or rights holder.
- The permitted purpose and use.
- Its data classification.
- Whether personal or sensitive information is present.
- Whether publication or redistribution is authorized.
- Whether data has been transformed, aggregated, or anonymized.
- Whether the transformation is sufficient for the intended disclosure.
- Whether the dataset contains embedded metadata.
- Whether third-party restrictions apply.

Only Public data may normally be included directly in a public release, and only when its source rights and publication conditions are established.

### 10.4 Personal Information

Public experiments should avoid exposing personal information unless there is a documented and appropriate basis for doing so.

This includes information contained in:

- Dataset files.
- Logs.
- Screenshots.
- Example inputs.
- Application outputs.
- Error reports.
- Test fixtures.
- User-submitted content.
- Generated reports.

### 10.5 Synthetic Data

Synthetic data is preferred when real information is unnecessary for an experiment.

However, synthetic data must not automatically be assumed to be anonymous or harmless.

Its generation method, provenance, characteristics, and potential to reproduce or reveal protected information should be considered.

### 10.6 External AI and Data Services

Projects using external AI providers or APIs must document relevant data-handling conditions.

This includes:

- What information is transmitted.
- Why it is transmitted.
- Which external service receives it.
- Whether processing is necessary.
- Whether personal, confidential, or restricted information is involved.
- Whether submitted information may be retained.
- Whether information may be used for model training or service improvement.
- Relevant processing locations and contractual conditions.
- Applicable safeguards and access controls.

Information must not be submitted where the necessary authorization, legal basis, or safeguards cannot be established.

### 10.7 Privacy Claims

Do not claim that a project is privacy-preserving, anonymous, or compliant with a particular regulation without an appropriate basis for that claim.

Claims must reflect actual processing, configurations, contractual arrangements, and evaluation.

---

## 11. Third-Party Dependencies and Licensing

### 11.1 Dependency Inventory

Each substantial project should maintain a record of its principal dependencies.

This may include:

- Software libraries.
- Frameworks.
- Model weights.
- AI APIs.
- Datasets.
- Fonts.
- Images.
- Audio.
- Icons.
- Video.
- External services.
- Documentation resources.
- Build and deployment tools.

### 11.2 Licence Compatibility

Before publication, verify that the intended use is compatible with the relevant terms.

Particular attention should be given to:

- MIT.
- Apache-2.0.
- BSD licences.
- GPL and AGPL licences.
- LGPL.
- Creative Commons licences.
- Proprietary software terms.
- Model-specific terms.
- Dataset-specific terms.
- Font and media licences.
- Platform and API usage terms.

The presence of an open-source dependency does not automatically make the entire project open source.

Licence compatibility must be considered in the context of the actual distribution and intended use.

### 11.3 Attribution

Required attribution must be included in the appropriate location.

Where substantial third-party material is used, an `ATTRIBUTIONS.md` or equivalent file is recommended.

Attribution must not imply endorsement, ownership, or affiliation where none exists.

### 11.4 No Implied Licensing

A public repository without a licence does not automatically grant open-source reuse permissions.

The repository must communicate its rights position clearly.

### 11.5 Unresolved Licensing

Material with unclear licensing conditions must not be distributed until the relevant rights have been clarified.

A dependency already being available publicly does not establish permission to redistribute it as part of a new release.

---

## 12. Security and Secret Detection

Security review must be proportionate to the project's technical scope and potential impact.

### 12.1 Credential Detection

Before publication, inspect for:

- API keys.
- Access tokens.
- Passwords.
- Private keys.
- SSH credentials.
- Certificates.
- Database connection strings.
- Cloud access credentials.
- Webhook secrets.
- Authentication cookies.
- Service account credentials.
- Recovery codes.
- Other authentication material.

### 12.2 Required Practices

Where relevant:

- Use environment variables for secrets.
- Provide a safe `.env.example`.
- Exclude private configuration through `.gitignore`.
- Use least-privilege access.
- Validate untrusted inputs.
- Avoid hardcoded privileged operations.
- Review exposed endpoints.
- Use maintained dependencies.
- Document authentication and permission requirements.
- Avoid logging secrets or sensitive data.

### 12.3 Automated Scanning

Appropriate automated security checks should be used when available.

These may include:

- Secret scanning.
- Dependency vulnerability scanning.
- Static analysis.
- Code quality checks.
- Configuration inspection.
- Container image scanning.
- Infrastructure configuration checks.

Automated tools are supplementary controls.

A clean scan does not establish that a repository contains no confidential information, intellectual property violations, or security weaknesses.

### 12.4 Critical Exposure

If a live credential is discovered:

1. Stop the publication process.
2. Revoke or rotate the exposed credential.
3. Investigate possible access or misuse.
4. Remove the exposed material from the appropriate locations.
5. Review repository history and distributed copies where relevant.
6. Record the remediation without reproducing the secret.

Deleting the visible credential is not a substitute for revocation.

### 12.5 Vulnerability Disclosure

Security vulnerabilities must be handled according to `SECURITY-v2.0.md`.

Do not disclose exploitable details through ordinary public issues or publication notes before an appropriate response has been established.

---

## 13. Technical Validation and Evidence

The technical review establishes that the proposed publication accurately represents the implementation and its demonstrated capabilities.

### 13.1 Minimum Checks

Depending on project scope, validate:

- Installation.
- Dependency resolution.
- Build or execution.
- Core functionality.
- Input validation.
- Error handling.
- Expected outputs.
- Configuration requirements.
- Relevant tests.
- Compatibility.
- Known limitations.
- Documented operating conditions.

### 13.2 Reproducibility

Where practical, the project should provide a reproducible setup.

This may include:

- Runtime requirements.
- Dependency versions.
- Lockfiles.
- Configuration examples.
- Installation commands.
- Test instructions.
- Example inputs.
- Expected output descriptions.
- Model and provider identifiers.
- Relevant experiment parameters.

Reproducibility must remain subject to intellectual property, privacy, confidentiality, licensing, and data-access restrictions.

### 13.3 Validation Claims

All claims must be accurate and appropriately qualified.

For example:

- A successful local build does not establish production reliability.
- A passing unit test suite does not prove complete functional correctness.
- A prototype demonstration does not establish scalability.
- A successful AI output does not establish model reliability.
- A public release does not establish operational readiness.
- A successful test in one environment does not establish compatibility with all environments.

### 13.4 Experimental Projects

Experimental projects may be published without satisfying production-grade expectations, provided their maturity, intended use, and limitations are clear and all publication conditions are met.

### 13.5 Unsupported Claims

Remove or qualify claims that cannot be supported by evidence.

Avoid presenting a project as:

- Secure.
- Anonymous.
- Validated.
- Reliable.
- Scalable.
- Production-ready.
- Fully accessible.
- Compliant.
- Autonomous.
- Reproducible.

unless the relevant claim has been assessed against appropriate criteria.

---

## 14. P1 Controlled Publication Requirements

P1 is a publishable classification only when its additional controls have been satisfied.

It must not be used as a way to release material with unresolved ownership, privacy, security, or confidentiality concerns.

### 14.1 Mandatory P1 Conditions

Before a P1 publication may receive APPROVED status, the maintainer must verify, where applicable:

**A. Defined Publication Scope**
- The exact files, assets, data, services, and release artefacts are identified.
- The intended publication channel is defined.
- Excluded material is documented where necessary.
- The public description accurately reflects the approved scope.

**B. Ownership and Licensing**
- Ownership and publication permissions are established.
- Third-party components have been identified.
- Relevant licences and terms have been reviewed.
- Attribution requirements are satisfied.
- No unresolved ownership or redistribution issue remains.

**C. Data and Privacy**
- Relevant data sources and data flows are documented.
- Data classification has been assigned.
- Personal and sensitive information has been identified.
- The use of external services has an appropriate basis and authorization.
- Retention and processing conditions are understood where relevant.
- No unauthorized confidential or restricted data is included.

**D. Security**
- Credentials and secrets have been removed.
- Access permissions are appropriate.
- Exposed interfaces and relevant integrations have been assessed.
- Material vulnerabilities have been resolved or publication has been withheld.
- Relevant security controls have been reviewed.

**E. External Services and Dependencies**
- Provider and API terms have been reviewed.
- External dependencies are identified.
- Important service limitations are documented.
- Dependency licensing has been assessed.
- Failure and availability assumptions are disclosed where relevant.

**F. Technical and Operational Conditions**
- The declared functionality has been tested sufficiently for its intended use.
- Configuration and installation requirements are documented.
- Important limitations are visible.
- Operational requirements and responsibilities are described where relevant.
- Required safeguards are implemented.

**G. Public Communication**
- AI involvement is disclosed where material.
- User-facing limitations are stated where relevant.
- Unsupported claims have been removed or qualified.
- The public documentation corresponds to the approved release.

### 14.2 P1 Conditions Register

For a substantial P1 publication, record the relevant controls in a conditions register.

| ID | Condition | Evidence or reference | Responsible person | State |
|---|---|---|---|---|
| P1-01 | Ownership and publication rights established | [Reference] | [Role] | [Pending / Complete] |
| P1-02 | External services and terms reviewed | [Reference] | [Role] | [Pending / Complete / N/A] |
| P1-03 | Data flows and classification reviewed | [Reference] | [Role] | [Pending / Complete / N/A] |
| P1-04 | Security and access controls reviewed | [Reference] | [Role] | [Pending / Complete] |
| P1-05 | Dependencies and licensing reviewed | [Reference] | [Role] | [Pending / Complete] |
| P1-06 | Technical validation completed | [Reference] | [Role] | [Pending / Complete] |
| P1-07 | Limitations and operating conditions documented | [Reference] | [Role] | [Pending / Complete] |
| P1-08 | Publication scope and release assets confirmed | [Reference] | [Role] | [Pending / Complete] |

Only applicable controls should be retained. An N/A decision should include a brief rationale where the control would ordinarily be relevant.

### 14.3 P1 Approval Gate

A P1 publication must remain PENDING until all mandatory conditions have been completed and verified.

The maintainer must not grant APPROVED status while:

- A required permission remains unresolved.
- A data-flow assessment is incomplete where relevant.
- A mandatory security control is missing.
- A confidentiality concern remains.
- A required dependency or licence check is incomplete.
- A required publication limitation is not communicated.
- The reviewed scope is uncertain.

### 14.4 P1 Approval Conditions

The approval record should identify:

- The P1 classification.
- The reviewed material and scope.
- Completed additional checks.
- Release limitations.
- Any continuing restrictions.
- Required maintenance or reassessment triggers.
- The approval date and decision authority.

P1 controls are not optional recommendations. They are conditions of publication.

### 14.5 Changes After P1 Approval

A material change to the approved project may invalidate part or all of the review.

Relevant changes include:

- New data sources.
- New external providers.
- Changes in model or provider.
- Expanded permissions.
- New user-facing functionality.
- New processing of personal information.
- Changes to release assets.
- Significant changes to deployment or access.
- Changes to terms or licensing.

The affected scope must be reassessed before the changed material is released.

---

## 15. Documentation Requirements

Documentation must provide enough information for a reader to understand the project, its purpose, and its limitations.

### 15.1 README

Substantial repositories should include a README containing:

- Project name.
- Purpose.
- Research domain.
- Current Project Status.
- Main capabilities.
- Technologies used.
- Installation instructions.
- Usage instructions.
- Requirements and dependencies.
- Known limitations.
- Attribution and licensing information.
- Relevant publication conditions.

### 15.2 Technical Documentation

Where relevant, include:

- Architecture overview.
- Configuration guide.
- API references.
- Data structures.
- Evaluation methodology.
- Testing procedures.
- Deployment instructions.
- Troubleshooting guidance.
- Security and privacy notes.
- Relevant model and provider information.

### 15.3 Screenshots and Demonstrations

Visual material must accurately represent the published implementation.

Do not include screenshots, diagrams, or recordings that reveal:

- Private infrastructure.
- Confidential interfaces.
- Personal information.
- Restricted content.
- Credentials.
- Unapproved functionality.
- Unreleased commercial work.

Conceptual visuals and mock-ups must be identified as such.

### 15.4 Documentation Accuracy

Documentation must be updated when significant changes make existing instructions or claims inaccurate.

Documentation should distinguish:

- Implemented functionality.
- Experimental functionality.
- Demonstrated functionality.
- Planned functionality.
- Unsupported or excluded functionality.

### 15.5 Documentation and Public Metadata

Review the repository description, topics, file names, commit history, badges, external links, and public project metadata.

Public metadata is part of the publication and must be reviewed accordingly.

---

## 16. Release Management

### 16.1 Release Eligibility

A release may be created only after the relevant publication checks have been completed and APPROVED status has been recorded for the defined scope.

### 16.2 Release Information

Where appropriate, releases should include:

- Project name.
- Version number or identifier.
- Release date.
- Summary of changes.
- Compatibility information.
- Known limitations.
- Migration instructions.
- Relevant dependencies.
- Relevant documentation.
- Licensing and attribution information.

### 16.3 Versioning

Projects should use a versioning model appropriate to their maturity.

Semantic Versioning may be used where a project exposes a stable interface or API.

Experimental projects may use alternative version identifiers, provided their meaning is clear.

Versioning should communicate meaningful changes rather than create unnecessary administrative overhead.

### 16.4 Release Assets

Downloadable binaries, datasets, archives, model files, and generated outputs must be reviewed independently.

Approval of source code does not automatically authorize distribution of every associated asset.

The release record should identify the approved artefacts.

### 16.5 Release Record

The actual publication event should be recorded separately from approval.

A release record should identify, where relevant:

- Project and repository.
- Release version or identifier.
- Approved review reference.
- Publication date.
- Public URL or distribution channel.
- Exact release scope.
- Relevant limitations.
- Maintainer responsible for the release.

### 16.6 Rollback and Correction

Where a release introduces a serious defect or security issue, affected releases should be corrected, superseded, restricted, or withdrawn as appropriate.

Users should be informed when the issue materially affects the safety, rights, or expected operation of the project.

---

## 17. Post-Publication Review

Publication responsibility continues after release.

### 17.1 Monitoring

Published projects should be reviewed when relevant changes occur, including:

- New features.
- New dependencies.
- Model or provider changes.
- Dataset additions.
- Licence changes.
- External service changes.
- Security advisories.
- User reports.
- Changes in project purpose.
- Changes in legal or contractual conditions.

### 17.2 Periodic Review

The maintainer should periodically assess whether published projects remain:

- Properly documented.
- Technically understandable.
- Appropriately licensed.
- Free of known unauthorized sensitive information.
- Consistent with the Lab's mission.
- Accurately represented.
- Appropriate for continued distribution.

Review frequency should reflect project activity, risk, and potential impact.

### 17.3 Issue Management

Reported defects, security issues, privacy concerns, and licensing questions should be assessed according to their severity and relevance.

Not every report requires an immediate code change, but material concerns must not be ignored.

Security concerns must be handled through the appropriate security process.

### 17.4 Abandoned Projects

Projects that are no longer maintained should communicate their status.

Where appropriate, mark them as archived or provide a maintenance notice.

An archived or discontinued project must not imply continuing support that has not been established.

### 17.5 Reassessment Triggers

A new publication review may be required when:

- The project purpose changes materially.
- The approved publication scope changes.
- New data or assets are introduced.
- New external services are integrated.
- Permissions or capabilities expand.
- A new distribution channel is added.
- A security or privacy incident occurs.
- A licence or ownership concern emerges.
- Material claims become inaccurate.
- A provider or dependency changes relevant terms.

The original approval must not be assumed to cover substantially different material.

---

## 18. Publication Approval and Decision Authority

### 18.1 Approval Authority

Under the current founder-led governance model, the Founder and Maintainer is responsible for approving publication under the Framing Creativity Lab identity.

This authority operates within applicable law, contractual obligations, third-party rights, and relevant platform procedures.

A technical review, successful demonstration, contributor recommendation, or repository merge does not independently authorize publication.

### 18.2 Approval Criteria

A project may be approved when:

- Its publication purpose is clear.
- Its ownership and publication rights are established.
- Its Publication Classification is appropriate.
- Confidentiality concerns have been resolved.
- Sensitive information has been checked.
- Dependencies and licences have been reviewed.
- Security and privacy requirements have been addressed.
- Technical validation is sufficient for the declared status.
- Documentation is accurate.
- Known limitations are disclosed.
- The public release scope is defined.
- All P1 conditions, where applicable, have been completed.

### 18.3 Approval Record

For substantial projects, retain a publication record containing:

- Project name.
- Repository URL.
- Version or commit reference.
- Review date.
- Publication Classification.
- Publication Status.
- Material and scope reviewed.
- Relevant findings.
- Completed conditions.
- Approval or rejection decision.
- Decision authority.
- Outstanding limitations.
- Release conditions or restrictions.

The record must not contain credentials, confidential material, or sensitive personal information.

### 18.4 Approval Scope

Approval applies only to the material and scope explicitly identified in the record.

Approval must not be interpreted as:

- A legal certification.
- An independent external security audit.
- A formal quality assurance certification.
- A warranty of functionality.
- A guarantee of operational readiness.
- Permission to publish unrelated project material.
- A general licence to reuse the published material.

### 18.5 Conditional Approval

A project with outstanding mandatory publication conditions must remain PENDING.

The Lab does not treat unresolved mandatory requirements as satisfied merely because a future correction has been promised.

An approval record may identify continuing restrictions or post-release obligations only where those conditions do not leave a mandatory pre-publication requirement unresolved.

---

## 19. Publication Review Checklist

The following checklist must be completed before a public release.

The exact checks should be adapted to the material and its classification. An item may be marked N/A only where it is genuinely not applicable.

### A. Ownership and Rights

- [ ] Project ownership has been established.
- [ ] Publication rights have been verified.
- [ ] Contributor permissions have been established where required.
- [ ] Third-party resources have been identified.
- [ ] Relevant licences and terms have been reviewed.
- [ ] Required permissions and attributions are present.
- [ ] No unauthorised proprietary material is included.
- [ ] The absence or scope of any project-specific licence is clear.

### B. Confidentiality

- [ ] No confidential project code is included.
- [ ] No private commercial architecture is disclosed.
- [ ] No client or internal documentation is included.
- [ ] No sensitive workflows or configurations are exposed.
- [ ] Screenshots and demonstrations have been inspected.
- [ ] Repository metadata has been reviewed.
- [ ] Git history has been considered where relevant.
- [ ] No restricted material is embedded in generated files or assets.

### C. Data and Privacy

- [ ] Data sources have been identified.
- [ ] Data classification has been assigned.
- [ ] Personal information has been identified.
- [ ] Sensitive information has been identified.
- [ ] Data-use rights have been established.
- [ ] External data processing has been considered.
- [ ] AI provider and API data handling has been reviewed.
- [ ] Personal or confidential data has been excluded or appropriately authorized.
- [ ] Privacy claims are supported and accurate.
- [ ] Data retention and processing conditions are documented where relevant.

### D. Security

- [ ] No API keys or credentials are committed.
- [ ] No private certificates or tokens are included.
- [ ] Configuration files have been reviewed.
- [ ] Input validation and relevant security controls have been assessed.
- [ ] Dependencies have been checked.
- [ ] Automated security checks have been considered.
- [ ] Relevant access permissions have been reviewed.
- [ ] Identified critical issues have been resolved.
- [ ] Security reporting and incident considerations are addressed.

### E. Technical Quality

- [ ] Installation instructions have been tested where applicable.
- [ ] Dependencies are documented.
- [ ] Build or execution has been validated where applicable.
- [ ] Core functionality has been tested.
- [ ] Known issues are documented.
- [ ] Technical Maturity is accurately described.
- [ ] Operational Readiness is accurately described.
- [ ] Reproduction instructions are available where practical.
- [ ] Public claims do not exceed available evidence.

### F. Documentation

- [ ] README is complete.
- [ ] Project purpose is clear.
- [ ] Technical structure is documented where necessary.
- [ ] Requirements and dependencies are identified.
- [ ] Limitations are disclosed.
- [ ] Attribution information is included.
- [ ] Licensing or rights information is explicit.
- [ ] Screenshots and examples represent the actual implementation.
- [ ] Public metadata has been reviewed.

### G. Classification and Approval

- [ ] Publication Classification has been assigned.
- [ ] P1 conditions have been completed where applicable.
- [ ] P2 or P3 restrictions have been resolved through a valid reassessment where applicable.
- [ ] All mandatory review items are resolved.
- [ ] Public repository contents have been reviewed.
- [ ] Intended publication channels are confirmed.
- [ ] Maintainer approval has been recorded.
- [ ] Publication Status is APPROVED.
- [ ] The exact approved release scope is documented.

### H. Release

- [ ] Release version or identifier is defined.
- [ ] Release assets have been reviewed.
- [ ] Release documentation is accurate.
- [ ] Release date and public channel are recorded.
- [ ] The actual publication event is documented.
- [ ] Post-publication responsibilities are understood.

**Publication Classification:** [P0 / P1 / P2 / P3]  
**Publication Status:** [PENDING / APPROVED / REJECTED / WITHDRAWN]  
**Review Date:** [YYYY-MM-DD]  
**Decision Authority:** [Maintainer or explicitly delegated role]  
**Review Reference:** [Record or Not Available]

---

## 20. Withdrawal and Removal Policy

A project or part of a project may be removed from public distribution when continued publication is no longer appropriate.

### 20.1 Reasons for Withdrawal

Examples include:

- Accidental disclosure of confidential information.
- Discovery of an ownership or licensing conflict.
- Security vulnerabilities.
- Privacy violations.
- Legal or contractual restrictions.
- Materially inaccurate documentation.
- Unauthorised third-party assets.
- Material changes to approved scope.
- Publication without the required authorization.
- A decision to discontinue public distribution.

### 20.2 Withdrawal Actions

Depending on the issue, actions may include:

1. Temporarily disabling access.
2. Removing affected files or releases.
3. Revoking exposed credentials.
4. Correcting repository history where appropriate.
5. Replacing affected assets.
6. Publishing a clarification.
7. Restricting distribution.
8. Archiving the repository.
9. Permanently removing the project.
10. Notifying affected users or parties where appropriate.

### 20.3 Historical Copies

Removing material from GitHub does not guarantee removal from forks, caches, downloaded archives, package registries, or independent copies.

Where sensitive information has been exposed, the response must consider the wider distribution context.

### 20.4 Security Exposure

Where credentials or secrets have been exposed, they must be revoked or rotated regardless of whether the material has been removed from the public repository.

Repository history modification does not substitute for credential revocation.

### 20.5 Withdrawal Record

Material publication or withdrawal decisions should be documented internally where appropriate.

The public record should not reproduce the confidential information that caused the withdrawal.

The record should identify the affected material, date, reason at an appropriate level of detail, actions taken, and resulting Publication Status.

### 20.6 Re-publication After Withdrawal

Withdrawn material must not be republished automatically.

A new review is required to establish:

- Whether the original reason for withdrawal has been resolved.
- Whether rights and authorizations remain valid.
- Whether security and privacy conditions are satisfied.
- Whether the new release scope is materially different.
- Whether a new classification is required.
- Whether approval can be granted again.

---

## 21. Exception Management

Exceptions should be rare, justified, and carefully considered.

### 21.1 No Exception to Fundamental Restrictions

This policy does not permit the publication of material that the Lab has no right to distribute.

Confidentiality, ownership, legal, contractual, and third-party restrictions cannot be bypassed through an informal exception.

No exception may authorize the exposure of credentials, private personal information, or restricted third-party material without an appropriate basis and authorization.

### 21.2 Scope-Specific Adjustments

Documentation depth, testing requirements, and review procedures may be adjusted to reflect the nature of a small or experimental project.

Such adjustments must not compromise essential publication controls.

### 21.3 Uncertainty

Where a material publication risk cannot be adequately assessed, the default decision is to withhold publication.

### 21.4 Exception Record

Where an exception to a procedural requirement is justified, the record should identify:

- The requirement concerned.
- The reason for the exception.
- The material and scope affected.
- The risk introduced.
- Alternative safeguards.
- The decision authority.
- The review or expiry condition.

An exception must not be used to bypass a mandatory P1 condition or to reclassify unresolved P2 or P3 material without the reassessment required by this policy.

---

## 22. Relationship with Other Lab Documents

This policy forms part of the Lab's publication and governance framework.

It should be read alongside the following documents:

| Document | Responsibility |
|---|---|
| `README.md` | Lab identity, mission, scope, and public overview |
| `LAB-CHARTER-v2.0.md` | Foundational principles and publication boundaries |
| `GOVERNANCE-v2.0.md` | Decision authority, responsibilities, and delegation |
| `PROJECT-LIFECYCLE-v2.0.md` | Lifecycle stages and canonical Project Status definitions |
| `PROJECT-TEMPLATE-v2.0.md` | Standard project record and publication fields |
| `QUALITY-STANDARDS-v2.0.md` | Technical Maturity, Operational Readiness, and technical quality expectations |
| `RESEARCH-METHODOLOGY-v2.0.md` | Research, experimentation, evidence, and reproducibility |
| `RESPONSIBLE-AI-v2.0.md` | AI risk, human oversight, data handling, and responsible AI requirements |
| `SECURITY-v2.0.md` | Security reporting and vulnerability handling |
| `CONTRIBUTING-v2.0.md` | Contribution process and contributor responsibilities |
| `CODE-OF-CONDUCT-v2.0.md` | Behavioural expectations and conduct concerns |

Publication Classification and Publication Status are defined only in this policy.

The Lifecycle Stage and Project Status are defined in `PROJECT-LIFECYCLE-v2.0.md`.

Technical Maturity and Operational Readiness are defined in `QUALITY-STANDARDS-v2.0.md`.

AI Risk Classification is defined separately in `RESPONSIBLE-AI-v2.0.md`.

A summary or reference in another document must not create a competing definition.

Where a policy-specific document governs a subject, its detailed requirements apply to that subject. Applicable laws, contractual obligations, and third-party rights remain controlling where relevant.

---

## 23. Policy Governance and Revision

### 23.1 Policy Ownership

This policy is maintained by J-ART under the governance principles established in `GOVERNANCE-v2.0.md` and the foundational principles of `LAB-CHARTER-v2.0.md`.

### 23.2 Approval Authority

The Founder and Maintainer is responsible for approving revisions to this policy under the current founder-led governance model.

A draft must not be represented as an approved or effective policy.

### 23.3 Revisions

Substantive revisions should include:

- Version number.
- Revision date.
- Summary of changes.
- Reason for revision.
- Approval record.

Previous versions should remain available in version control where appropriate.

### 23.4 Effective Application

This policy applies to new public releases and material updates to existing published projects once formally approved.

Existing repositories should be progressively reviewed against its requirements.

A new policy version does not automatically approve previously restricted material or invalidate a previously approved release. Relevant material should be reassessed where the changes materially affect publication conditions.

### 23.5 Consistency Review

Changes to this policy should be checked against:

- Project Status and Lifecycle Stage definitions.
- Technical Maturity and Operational Readiness definitions.
- Data classification terminology.
- Responsible AI requirements.
- Contribution and licensing conditions.
- Security and confidentiality procedures.
- Repository and release documentation.

Any terminology change must be coordinated with the relevant authoritative document rather than introduced in isolation.

---

## 24. Final Principle

Framing Creativity Lab does not measure success by how much material it can publish.

It measures the value of its public work through the quality of its research, the clarity of its implementation, the integrity of its documentation, and the responsibility with which it shares knowledge.

Publication is not simply a technical operation or a visibility setting. It is a decision that establishes what the Lab is prepared to make public and what responsibilities accompany that decision.

A publication should demonstrate something worth sharing without exposing something that should remain protected.

**Build openly where appropriate.  
Protect what must remain private.  
Verify before publishing.  
Document what is known.  
Be honest about what is not.**

---

**FRAMING CREATIVITY LAB**  
Independent Research · Applied AI · Creative Technology · Digital Innovation

**Maintainer:** J-ART  
**Document:** `PUBLICATION-POLICY-v2.0.md`  
**Reference:** `LAB-CHARTER-v2.0.md`

*Publication is not simply making work visible. It is taking responsibility for what becomes public.*
