# FRAMING CREATIVITY LAB
## PUBLICATION POLICY

**Document ID:** FCL-POL-001  
**Version:** 1.0  
**Status:** Initial Policy  
**Established:** November 2026  
**Maintainer:** J-ART  
**Applies to:** All public repositories, projects, experiments, tools and documentation published under Framing Creativity Lab.

---

# 01 — PURPOSE

This policy defines the requirements, review procedures and approval criteria governing the publication of work under the Framing Creativity Lab identity.

Its purpose is to ensure that every public release is intentional, technically appropriate, properly documented and consistent with the lab's principles.

It establishes a controlled process for moving material from private development or experimentation into the public environment.

The policy addresses:

- Publication eligibility.
- Intellectual property and ownership.
- Confidentiality and information protection.
- Source code and repository review.
- Security and privacy.
- Third-party dependencies and licences.
- Technical validation.
- Documentation requirements.
- Release approval.
- Publication maintenance and withdrawal.

The policy applies regardless of whether the material is presented as a research experiment, prototype, proof of concept, tool, application, technical demonstration or documentation resource.

**Public visibility is a publication decision, not a default development setting.**

---

# 02 — SCOPE & APPLICATION

## 2.1 Covered material

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
- Releases, packages and downloadable assets.
- Public websites and project documentation.

It also applies to updates, patches, releases and subsequent versions of previously published projects.

## 2.2 Covered publication channels

The policy applies to public distribution through:

- GitHub repositories.
- GitHub Pages.
- Public package registries.
- Public documentation websites.
- Public AI and model repositories.
- Public demonstration platforms.
- External services used to distribute lab projects.
- Community platforms that display or synchronise public repositories.

The specific publication requirements may differ depending on the platform.

## 2.3 Exclusions

Private development environments are not publication channels.

The policy does not authorise the transfer, disclosure or publication of private commercial projects, client materials or confidential work.

A project does not become eligible for publication simply because it has been developed independently, uses publicly available technologies or contains no obvious confidential information.

Publication eligibility must be established separately.

---

# 03 — FUNDAMENTAL PUBLICATION PRINCIPLES

Every publication decision must follow these principles.

## 3.1 Intentional publication

A project must be explicitly selected for public release.

Public accessibility must never result from accidental repository configuration, unintended synchronisation or an unreviewed visibility change.

## 3.2 Ownership before publication

The right to publish all included material must be established before release.

Possession of a file, codebase, dataset or asset does not automatically confer publication or redistribution rights.

## 3.3 Confidentiality by design

Confidential information must remain outside public repositories.

Removing names or identifying references does not necessarily remove the confidential nature of technical implementation details, workflows or business information.

## 3.4 Technical integrity

Published code and documentation must accurately represent the state and capabilities of the project.

Incomplete, experimental or unstable implementations may be published when their status and limitations are clearly communicated.

## 3.5 Transparency

The project must describe what it does, how it works, what it requires and what limitations are known.

Claims must be proportionate to available evidence.

## 3.6 Responsible distribution

Publication must consider downstream use, third-party rights, data protection, security and potential misuse.

## 3.7 Continuous responsibility

Publication approval is not permanent immunity from future review.

Repositories must be reassessed when significant code, data, dependencies, licences or project purposes change.

---

# 04 — PUBLICATION ELIGIBILITY

A project may be considered for publication when all applicable eligibility conditions are satisfied.

## 4.1 Eligible material

Examples of potentially eligible material include:

- Original independent experiments.
- Independently developed tools.
- Original research and technical notes.
- Self-contained software demonstrations.
- Public-domain or appropriately licensed resources.
- Independently developed prototypes.
- Reusable components with clear ownership.
- Educational examples.
- Technical evaluations based on authorised resources.

Eligibility depends on the specific contents and implementation, not merely the project category.

## 4.2 Ineligible material

The following must not be published without a separate, documented and valid authorisation:

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
- Content whose ownership or publication rights are unclear.

## 4.3 Independent implementation requirement

An experiment may investigate a general concept that is also relevant to another private project.

However, the public implementation must be independently developed and reviewed.

It must not contain copied proprietary implementation details, confidential workflows, protected assets or extracted internal documentation.

A similar idea does not justify reuse of protected material.

Where independence cannot be established with reasonable confidence, publication must be withheld pending further review.

---

# 05 — PUBLICATION CLASSIFICATION

Projects must be classified before review.

The classification helps determine the appropriate level of scrutiny.

## 5.1 Classification levels

| Level | Classification | Description |
|---|---|---|
| P0 | Public-ready | Independent, low-risk material with established publication rights. |
| P1 | Controlled publication | Material requiring additional checks because of dependencies, external services, data or technical exposure. |
| P2 | Restricted review | Material presenting unresolved ownership, security, privacy or confidentiality questions. |
| P3 | Non-publishable | Material that must not enter the public lab environment. |

## 5.2 P0 — Public-ready

Examples:

- Original standalone code.
- Independent technical experiments.
- Publicly licensed examples used within licence terms.
- General technical documentation.
- Self-contained demonstrations without sensitive dependencies.

Required review:

- Basic ownership check.
- Repository inspection.
- Credential and secret scan.
- Documentation review.
- Publication checklist.

## 5.3 P1 — Controlled publication

Examples:

- Experiments using external APIs.
- AI applications interacting with third-party models.
- Projects using external datasets.
- Applications involving user-submitted information.
- Projects containing complex third-party dependencies.
- Demonstrations deployed through external services.

Additional review:

- Data-flow assessment.
- External service and API terms.
- Licence compatibility.
- Privacy implications.
- Security configuration.
- Operational dependencies.
- User-facing limitations.

## 5.4 P2 — Restricted review

Examples:

- Projects containing material with uncertain ownership.
- Experiments derived from confidential development environments.
- Applications involving potentially sensitive datasets.
- Projects with unresolved security concerns.
- Repositories with unexplained third-party material.
- Codebases where separation from proprietary work cannot be established.

P2 material must remain unpublished until the concerns are resolved and the project has been reassessed.

The existence of a P2 classification does not guarantee eventual publication.

## 5.5 P3 — Non-publishable

Examples:

- Confidential commercial source code.
- Unauthorised client data.
- Private credentials.
- Material that cannot legally or contractually be distributed.
- Proprietary implementation details without publication permission.
- Unauthorised personal information.
- Restricted third-party resources.

P3 material is excluded from the public publication process.

It must not be moved into a public repository for convenience, demonstration or partial disclosure.

---

# 06 — PUBLICATION REVIEW PROCESS

All projects must follow the publication workflow.

## 6.1 Standard workflow

**Project identification**

→ Define the material being considered for publication.

**Ownership assessment**

→ Establish authorship, rights and publication permissions.

**Scope assessment**

→ Identify the exact files, assets, documentation and dependencies to be released.

**Risk classification**

→ Assign P0, P1, P2 or P3.

**Content review**

→ Inspect source code, data, configuration, documentation and metadata.

**Technical validation**

→ Test the implementation and review its operational requirements.

**Documentation review**

→ Confirm that the README and supporting documentation accurately describe the project.

**Final approval**

→ Verify that all applicable publication requirements are satisfied.

**Publication**

→ Release the approved material through the intended public channel.

**Post-publication monitoring**

→ Review feedback, defects, security reports and relevant changes.

## 6.2 Review gate

Publication must not proceed if any mandatory requirement remains unresolved.

A project may be technically complete while still being unsuitable for publication.

Similarly, documentation completeness cannot compensate for unresolved ownership or confidentiality concerns.

## 6.3 Scope control

Approval applies only to the reviewed material and its defined publication scope.

Adding new datasets, assets, integrations, major features or external dependencies may trigger another review.

---

# 07 — INTELLECTUAL PROPERTY & OWNERSHIP REVIEW

Before publication, the project maintainer must establish the rights associated with every significant component.

## 7.1 Ownership questions

The review should establish:

- Who created the original work?
- Who owns the relevant intellectual property?
- Was the work created under a contract or employment arrangement?
- Are any third-party components included?
- Are redistribution rights available?
- Are there contractual confidentiality obligations?
- Are there restrictions on derivative works?
- Does the project include generated material subject to external terms?

## 7.2 Original work

Original work may be published when the author has the appropriate rights and no conflicting obligations apply.

## 7.3 Third-party work

Third-party material must be reviewed individually.

Its inclusion must respect the applicable licence, attribution requirements, redistribution permissions and any relevant restrictions.

## 7.4 AI-generated material

AI-generated output must not automatically be assumed to be free of third-party rights or other restrictions.

The relevant model, service and asset-generation terms should be reviewed where material is intended for redistribution.

## 7.5 Ownership uncertainty

Where ownership or permission cannot be established, the material must not be published until the uncertainty is resolved.

---

# 08 — CONFIDENTIALITY & INFORMATION SECURITY REVIEW

Confidentiality review must cover the complete repository, not just the main source files.

## 8.1 Source code

Inspect source files for:

- Proprietary business logic.
- Internal service references.
- Private application integrations.
- Non-public architecture.
- Internal identifiers.
- Confidential algorithms.
- Unreleased implementation details.

## 8.2 Configuration

Inspect:

- Environment files.
- Configuration examples.
- Build settings.
- Deployment configurations.
- Infrastructure references.
- API endpoints.
- Authentication mechanisms.
- Service identifiers.

Sensitive values must never be committed.

Use environment variables and safe configuration examples where appropriate.

## 8.3 Documentation

Inspect:

- README files.
- Technical specifications.
- Architecture documentation.
- Development notes.
- Diagrams.
- Screenshots.
- Generated documentation.
- Commit history where relevant.

Documentation can expose confidential information even when the source code does not.

## 8.4 Git history

The review should consider the repository's full history where relevant.

Sensitive information may remain in:

- Previous commits.
- Deleted files.
- Branches.
- Tags.
- Release assets.
- Historical configuration.
- Git objects.

Removing a file from the current branch does not guarantee that historical copies are no longer accessible.

## 8.5 Repository metadata

Review:

- Repository name.
- Description.
- Topics.
- Branch names.
- Commit messages.
- GitHub Actions.
- Issues.
- Discussions.
- Releases.
- Project URLs.

All visible metadata must be appropriate for public release.

---

# 09 — SECURITY & SECRET DETECTION

Security review must be proportionate to the project's technical scope.

## 9.1 Credential detection

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

## 9.2 Required practices

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

## 9.3 Automated scanning

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

A clean scan does not establish that a repository contains no confidential information or security weaknesses.

## 9.4 Critical exposure

If a live credential is discovered:

1. Stop the publication process.
2. Revoke or rotate the exposed credential.
3. Investigate possible access or misuse.
4. Remove the exposed material from the appropriate locations.
5. Review repository history and copies.
6. Record the remediation where appropriate.

Deleting the visible credential is not a substitute for revocation.

---

# 10 — DATA PROTECTION & PRIVACY REVIEW

Projects involving data must establish an appropriate basis for its use and publication.

## 10.1 Data classification

Where applicable, data should be classified as:

- Public.
- Internal.
- Confidential.
- Personal.
- Sensitive or restricted.

Only appropriately authorised data may be included in public repositories.

## 10.2 Personal information

Public experiments should avoid exposing personal information unless there is a documented and valid reason and an appropriate legal basis.

This includes information contained in:

- Dataset files.
- Logs.
- Screenshots.
- Example inputs.
- Application outputs.
- Error reports.
- Test fixtures.

## 10.3 Synthetic data

Synthetic data is preferred when real information is unnecessary for an experiment.

However, synthetic data must not be assumed to be anonymous or harmless without consideration of its generation method and characteristics.

## 10.4 External AI and data services

Projects using external AI providers or APIs must document relevant data-handling conditions.

This includes:

- What information is transmitted.
- Why it is transmitted.
- Which external service receives it.
- Whether processing is necessary.
- Whether personal or confidential information is involved.
- Any relevant retention or processing conditions.

## 10.5 Privacy claims

Do not claim that a project is privacy-preserving, anonymous or compliant with a regulation without an appropriate basis for that claim.

---

# 11 — THIRD-PARTY DEPENDENCIES & LICENSING

## 11.1 Dependency inventory

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
- External services.
- Documentation resources.

## 11.2 Licence compatibility

Before publication, verify that the intended use is compatible with the relevant terms.

Particular attention should be given to:

- MIT.
- Apache-2.0.
- BSD licences.
- GPL and AGPL licences.
- LGPL.
- Creative Commons licences.
- Proprietary software terms.
- Model and dataset-specific terms.

The presence of an open-source dependency does not automatically make the entire project open source.

## 11.3 Attribution

Required attribution must be included in the appropriate location.

Where substantial third-party material is used, an `ATTRIBUTIONS.md` or equivalent file is recommended.

## 11.4 No implied licensing

A public repository without a licence does not automatically grant open-source reuse permissions.

The repository must communicate its rights position clearly.

## 11.5 Unresolved licensing

Material with unclear licensing conditions must not be distributed until the relevant rights have been clarified.

---

# 12 — TECHNICAL VALIDATION

The technical review establishes that the publication accurately represents the project's implementation and maturity.

## 12.1 Minimum checks

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
- Known limitations.

## 12.2 Reproducibility

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

## 12.3 Validation claims

All claims must be accurate and appropriately qualified.

For example:

- A successful local build does not establish production reliability.
- A passing unit test suite does not prove complete functional correctness.
- A prototype demonstration does not establish scalability.
- A successful AI output does not establish model reliability.

## 12.4 Experimental projects

Experimental projects may be published without satisfying production-grade expectations, provided their maturity and limitations are clear.

---

# 13 — DOCUMENTATION REQUIREMENTS

Documentation must provide enough information for a reader to understand the project and its status.

## 13.1 README

Substantial repositories should include a README containing:

- Project name.
- Purpose.
- Research domain.
- Status.
- Main capabilities.
- Technologies used.
- Installation instructions.
- Usage instructions.
- Limitations.
- Attribution and licensing information.

## 13.2 Technical documentation

Where relevant, include:

- Architecture overview.
- Configuration guide.
- API references.
- Data structures.
- Evaluation methodology.
- Testing procedures.
- Deployment instructions.
- Troubleshooting guidance.

## 13.3 Screenshots and demonstrations

Visual material must accurately represent the published implementation.

Do not include screenshots or diagrams that reveal private infrastructure, confidential interfaces or unapproved content.

## 13.4 Documentation accuracy

Documentation must be updated when significant changes make existing instructions or claims inaccurate.

---

# 14 — RELEASE MANAGEMENT

## 14.1 Release eligibility

A release may be created only after the relevant publication checks have been completed.

## 14.2 Release information

Where appropriate, releases should include:

- Version number.
- Release date.
- Summary of changes.
- Compatibility information.
- Known limitations.
- Migration instructions.
- Relevant dependencies.

## 14.3 Versioning

Projects should use a versioning model appropriate to their maturity.

Semantic Versioning may be used where a project exposes a stable interface or API.

Experimental projects may use alternative version identifiers, provided their meaning is clear.

## 14.4 Release assets

Downloadable binaries, datasets, archives and generated outputs must be reviewed independently.

Approval of source code does not automatically authorise the distribution of every associated asset.

## 14.5 Rollback

Where a release introduces a serious defect or security issue, affected releases should be withdrawn, corrected or superseded.

Users should be informed when the issue materially affects the safety or expected operation of the project.

---

# 15 — POST-PUBLICATION REVIEW

Publication responsibility continues after release.

## 15.1 Monitoring

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

## 15.2 Periodic review

The maintainer should periodically assess whether published projects remain:

- Properly documented.
- Technically understandable.
- Appropriately licensed.
- Free of known sensitive information.
- Consistent with the lab's mission.

The review frequency should reflect project activity and risk.

## 15.3 Issue management

Reported defects, security issues, privacy concerns and licensing questions should be assessed according to their severity and relevance.

Not every report requires an immediate code change, but material concerns must not be ignored.

## 15.4 Abandoned projects

Projects that are no longer maintained should communicate their status.

Where appropriate, mark them as archived or provide a maintenance notice.

---

# 16 — WITHDRAWAL & REMOVAL POLICY

A project or part of a project may be removed from public distribution when continued publication is no longer appropriate.

## 16.1 Reasons for withdrawal

Examples include:

- Accidental disclosure of confidential information.
- Discovery of an ownership or licensing conflict.
- Security vulnerabilities.
- Privacy violations.
- Legal or contractual restrictions.
- Materially inaccurate documentation.
- Unauthorised third-party assets.
- Project scope changes.
- A decision to discontinue public distribution.

## 16.2 Withdrawal actions

Depending on the issue, actions may include:

1. Temporarily disabling access.
2. Removing affected files or releases.
3. Revoking exposed credentials.
4. Correcting repository history where appropriate.
5. Replacing affected assets.
6. Publishing a clarification.
7. Archiving the repository.
8. Permanently removing the project.

## 16.3 Historical copies

Removing material from GitHub does not guarantee removal from forks, caches, downloaded archives or independent copies.

Where sensitive information has been exposed, the response must consider the wider distribution context.

## 16.4 Record keeping

Material publication or withdrawal decisions should be documented internally where appropriate.

The public record should not reproduce the confidential information that caused the withdrawal.

---

# 17 — EXCEPTION MANAGEMENT

Exceptions should be rare and carefully considered.

## 17.1 No exception to fundamental restrictions

This policy does not permit the publication of material that the lab has no right to distribute.

Confidentiality, ownership, legal and contractual restrictions cannot be bypassed through an informal exception.

## 17.2 Scope-specific adjustments

Documentation depth, testing requirements and publication procedures may be adjusted to reflect the nature of a small or experimental project.

Such adjustments must not compromise essential publication controls.

## 17.3 Uncertainty

Where a material publication risk cannot be adequately assessed, the default decision is to withhold publication.

---

# 18 — PUBLICATION APPROVAL

## 18.1 Approval authority

The maintainer is responsible for approving publication under the current founder-led governance model.

The approval process must not be interpreted as an independent legal certification, external security audit or formal quality assurance certification.

## 18.2 Approval criteria

A project may be approved when:

- Its publication purpose is clear.
- Its ownership and publication rights are established.
- Its risk classification is appropriate.
- Confidentiality concerns have been resolved.
- Sensitive information has been checked.
- Dependencies and licences have been reviewed.
- Technical validation is sufficient for the declared status.
- Documentation is accurate.
- Known limitations are disclosed.
- The public release scope is defined.

## 18.3 Approval record

For substantial projects, retain a publication record containing:

- Project name.
- Repository URL.
- Version or commit reference.
- Review date.
- Risk classification.
- Review status.
- Relevant findings.
- Approval decision.
- Outstanding limitations.

The record should not contain credentials, confidential material or sensitive personal information.

---

# 19 — PUBLICATION CHECKLIST

The following checklist must be completed before a public release.

## A. Ownership & Rights

- [ ] Project ownership has been established.
- [ ] Publication rights have been verified.
- [ ] Third-party resources have been identified.
- [ ] Relevant licences and terms have been reviewed.
- [ ] Required permissions and attributions are present.
- [ ] No unauthorised proprietary material is included.

## B. Confidentiality

- [ ] No confidential project code is included.
- [ ] No private commercial architecture is disclosed.
- [ ] No client or internal documentation is included.
- [ ] No sensitive workflows or configurations are exposed.
- [ ] Screenshots and demonstrations have been inspected.
- [ ] Repository metadata has been reviewed.
- [ ] Git history has been considered where relevant.

## C. Security

- [ ] No API keys or credentials are committed.
- [ ] No private certificates or tokens are included.
- [ ] Configuration files have been reviewed.
- [ ] Input validation and relevant security controls have been assessed.
- [ ] Dependencies have been checked.
- [ ] Automated security checks have been considered.
- [ ] Any identified critical issues have been resolved.

## D. Privacy & Data

- [ ] All datasets have been reviewed.
- [ ] Personal information has been excluded or appropriately authorised.
- [ ] Synthetic data is identified where relevant.
- [ ] External data processing has been considered.
- [ ] AI provider and API data handling has been reviewed.
- [ ] Privacy claims are supported and accurate.

## E. Technical Quality

- [ ] Installation instructions have been tested.
- [ ] Dependencies are documented.
- [ ] Build or execution has been validated.
- [ ] Core functionality has been tested.
- [ ] Known issues are documented.
- [ ] Project maturity is accurately described.
- [ ] Reproduction instructions are available where practical.

## F. Documentation

- [ ] README is complete.
- [ ] Project purpose is clear.
- [ ] Technical structure is documented where necessary.
- [ ] Requirements and dependencies are identified.
- [ ] Limitations are disclosed.
- [ ] Attribution information is included.
- [ ] Licensing or rights information is explicit.
- [ ] Screenshots and examples represent the actual implementation.

## G. Final Publication

- [ ] Risk classification has been assigned.
- [ ] All mandatory review items are resolved.
- [ ] Public repository contents have been reviewed.
- [ ] Intended publication channels are confirmed.
- [ ] Maintainer approval has been recorded.
- [ ] Release or publication information is accurate.

**Publication status:** PENDING / APPROVED / REJECTED / WITHDRAWN

---

# 20 — POLICY GOVERNANCE & REVISION

## 20.1 Policy ownership

This policy is maintained by J-ART under the governance principles established in `LAB-CHARTER.md`.

## 20.2 Relationship to the Lab Charter

This policy implements the publication principles established by the Lab Charter.

It does not replace or supersede the Charter.

Where a conflict appears to exist, the Charter's fundamental requirements concerning independence, intellectual property, confidentiality and responsible publication take precedence.

## 20.3 Revisions

Changes to this policy must be reviewed and approved by the maintainer.

Substantive revisions should include:

- Version number.
- Revision date.
- Summary of changes.
- Reason for revision.

Previous versions should remain available in version control where appropriate.

## 20.4 Effective application

This policy applies to new public releases and material updates to existing published projects.

Existing repositories should be progressively reviewed against its requirements.

---

# 21 — FINAL PRINCIPLE

Framing Creativity Lab does not measure success by how much material it can publish.

It measures the value of its public work through the quality of its research, the clarity of its implementation, the integrity of its documentation and the responsibility with which it shares knowledge.

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
**Document:** `PUBLICATION-POLICY.md`  
**Reference:** `LAB-CHARTER.md`

*Publication is not simply making work visible. It is taking responsibility for what becomes public.*
