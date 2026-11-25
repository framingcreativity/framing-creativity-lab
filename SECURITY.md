# Security Policy

**Document ID:** FCL-SEC-001  
**Version:** 1.0  
**Status:** Initial  
**Effective Date:** 25 November 2026  
**Maintainer:** J-ART  
**Repository:** Framing Creativity Lab

---

## 1. Purpose

Framing Creativity Lab is committed to maintaining a responsible approach to software security, data protection, and the safe development of digital systems.

This policy establishes the principles and procedures for identifying, reporting, assessing, addressing, and disclosing security vulnerabilities affecting projects published within the Lab.

Security is treated as an integral part of research and development, not as a final validation step.

The policy aims to:

- Provide a clear channel for reporting potential vulnerabilities.
- Encourage responsible and coordinated disclosure.
- Protect users, contributors, maintainers, and third parties.
- Reduce the risk of credential exposure, data leakage, and unauthorized access.
- Establish consistent expectations for security-related contributions.
- Address security considerations specific to AI-enabled systems and experimental technologies.

This policy applies alongside the Lab Charter, Publication Policy, Research Methodology, and Contribution Guidelines.

---

## 2. Scope

This policy applies to publicly maintained software, tools, prototypes, and technical resources published under Framing Creativity Lab.

Depending on the project, this may include:

- Source code and application logic.
- Web applications and APIs.
- Development scripts and command-line tools.
- Build, deployment, and automation workflows.
- Project configurations and infrastructure definitions.
- Third-party dependencies and packages.
- Authentication and authorization mechanisms.
- Data storage and processing components.
- AI integrations, agents, and experimental workflows.
- Documentation containing operational or security-sensitive instructions.

The policy covers security weaknesses introduced by the Lab's own published work and its maintained configuration.

It does not automatically extend to external services, platforms, providers, models, or systems operated by third parties.

---

## 3. Supported Versions

Unless a project-specific security policy states otherwise, the following support expectations apply:

| Version or branch | Security support |
|---|---|
| Default branch | Maintained target |
| Latest published release | Supported where applicable |
| Older releases | No guarantee of security updates |
| Archived projects | Not actively maintained |
| Experimental prototypes | Best-effort review, no production security guarantee |

A project may define a different support lifecycle in its own documentation.

The presence of publicly accessible code does not imply that the project is production-ready, security-certified, or suitable for sensitive workloads.

---

## 4. What Qualifies as a Security Vulnerability?

A security vulnerability is a weakness that could compromise the confidentiality, integrity, or availability of a system, its data, or its users.

Examples include, but are not limited to:

### 4.1 Application and Software Security

- Authentication or authorization bypasses.
- Insecure direct object references.
- Injection vulnerabilities.
- Cross-site scripting (XSS).
- Cross-site request forgery (CSRF).
- Server-side request forgery (SSRF).
- Unsafe file uploads or file handling.
- Path traversal.
- Insecure deserialization.
- Remote code execution.
- Privilege escalation.
- Inadequate access controls.
- Exposure of sensitive application data.

### 4.2 Infrastructure and Configuration

- Hardcoded credentials or API keys.
- Exposed environment variables or secrets.
- Misconfigured permissions.
- Insecure deployment configurations.
- Unprotected administrative interfaces.
- Insecure network or storage configurations.
- Vulnerable or improperly configured dependencies.
- Weak cryptographic practices.
- Unsafe automation or CI/CD workflows.

### 4.3 Data and Privacy

- Unauthorized access to personal or confidential information.
- Accidental disclosure of private datasets.
- Improper data retention or deletion.
- Insecure handling of authentication tokens.
- Exposure of internal logs or operational information.
- Data leakage across users, sessions, or environments.

### 4.4 AI and Emerging Technologies

AI-enabled applications introduce additional security considerations.

Relevant vulnerabilities may include:

- Prompt injection that compromises system boundaries or intended behavior.
- Leakage of system prompts, confidential context, or protected information.
- Unauthorized tool execution by AI agents.
- Inadequate isolation between users, sessions, or agent tasks.
- Retrieval-augmented generation (RAG) access-control failures.
- Unsafe execution of model-generated code or commands.
- Improper validation of model-generated outputs.
- Exposure of model credentials or service tokens.
- Insecure handling of uploaded files or untrusted model inputs.
- Abuse of external tools, integrations, or connected services.

AI-related behavior should be assessed according to its actual security impact. Unexpected, inaccurate, or low-quality model output is not necessarily a security vulnerability.

---

## 5. Issues Outside the Scope of This Policy

The following are generally not considered security vulnerabilities unless they create a demonstrable security impact:

- Ordinary software defects without a security consequence.
- Visual or usability inconsistencies.
- Feature requests.
- Performance issues without an availability or security impact.
- Theoretical vulnerabilities without a credible attack path.
- Model hallucinations that do not expose protected information or compromise a system.
- Findings concerning third-party products that are not caused by the Lab's implementation.
- Issues requiring access to systems or data outside the reporter's authorization.

Third-party vulnerabilities should be reported to the relevant provider or responsible security team.

The Lab may assist in identifying the affected integration or dependency, but it cannot guarantee remediation by an external provider.

---

## 6. Reporting a Vulnerability

### 6.1 Preferred Reporting Channel

Security vulnerabilities must be reported privately.

The preferred channel is GitHub's **Private Vulnerability Reporting** feature for the Framing Creativity Lab repository, provided that the feature has been enabled.

Reporters should use the repository's Security tab and select the private vulnerability reporting option when available.

Security vulnerabilities must not be submitted through:

- Public GitHub issues.
- Public discussion threads.
- Pull requests containing exploit details.
- Public comments or social media posts.
- Other publicly accessible communication channels.

**Operational requirement:** The repository maintainer must enable GitHub Private Vulnerability Reporting before presenting this channel as available to reporters.

If private reporting is unavailable, reporters should use a security contact method explicitly published by the maintainer. No unpublished email address or private contact channel should be assumed.

### 6.2 Information to Include

A useful security report should include, where possible:

1. A concise description of the suspected vulnerability.
2. The affected repository, project, component, or version.
3. The conditions required to reproduce the issue.
4. A step-by-step explanation of the reproduction process.
5. The potential impact and affected security properties.
6. Supporting evidence, such as sanitized logs or screenshots.
7. A suggested mitigation, if known.
8. Any relevant technical context or environmental requirements.

Reports should include enough information to understand and assess the issue without exposing unnecessary personal, confidential, or third-party data.

A report does not need to contain a complete exploit or proof of compromise.

---

## 7. Responsible Disclosure

Framing Creativity Lab supports coordinated vulnerability disclosure.

Reporters are expected to:

- Make a good-faith effort to report vulnerabilities privately.
- Avoid accessing, modifying, or deleting data that does not belong to them.
- Avoid disrupting systems or services.
- Refrain from testing against real users or unauthorized environments.
- Avoid public disclosure while a reasonable remediation process is underway.
- Share only the minimum technical evidence necessary.
- Respect applicable laws and third-party terms of service.

The Lab will make reasonable efforts to assess legitimate reports, communicate with reporters where possible, and coordinate disclosure when remediation is required.

The exact disclosure timeline depends on the severity, complexity, affected components, and availability of a reliable fix.

No fixed response or remediation deadline is guaranteed by this policy.

---

## 8. Severity Classification

Reported vulnerabilities are assessed according to their practical impact, exploitability, affected assets, and potential consequences.

The following categories provide a consistent starting point.

| Severity | General interpretation |
|---|---|
| Critical | A vulnerability enabling severe compromise, such as remote code execution, broad unauthorized access, or major exposure of sensitive data. |
| High | A vulnerability that could lead to significant unauthorized access, privilege escalation, or compromise of important functionality or information. |
| Medium | A vulnerability with a meaningful but constrained security impact, often requiring specific conditions or additional access. |
| Low | A limited security weakness with restricted impact or difficult exploitation. |
| Informational | A security observation, hardening recommendation, or issue without a demonstrated vulnerability. |

Where appropriate, the Common Vulnerability Scoring System (CVSS) may be used as a supporting assessment framework.

A numerical score does not replace contextual analysis. The final classification should reflect the actual risk within the affected project.

---

## 9. Vulnerability Handling Process

Security reports are handled through a structured process.

### Stage 1 — Receipt

The maintainer receives the private report and reviews the initial information.

The report may be acknowledged and additional evidence requested where necessary.

### Stage 2 — Triage

The issue is assessed to determine:

- Whether it is reproducible.
- Whether it falls within the Lab's scope.
- Which components or versions are affected.
- Whether the issue has been publicly exposed.
- Its likely severity and practical impact.
- Whether immediate containment is required.

### Stage 3 — Investigation

The maintainer investigates the reported weakness in a controlled environment.

The investigation should avoid unnecessary access to sensitive information and should not extend into systems operated by third parties without authorization.

### Stage 4 — Mitigation

Where a vulnerability is confirmed, appropriate mitigation may include:

- Correcting the affected code.
- Restricting or disabling vulnerable functionality.
- Revoking or rotating exposed credentials.
- Updating affected dependencies.
- Changing configuration or access permissions.
- Removing exposed data or files.
- Temporarily withdrawing an affected release or prototype.

### Stage 5 — Remediation and Validation

The proposed correction is reviewed and tested.

Validation should confirm that:

- The original vulnerability has been addressed.
- The corrective change does not introduce an obvious regression.
- Related components have been considered.
- Relevant documentation has been updated.

### Stage 6 — Disclosure and Closure

When appropriate, the Lab may publish a security advisory or release note describing:

- The affected component.
- The nature of the vulnerability.
- Its practical impact.
- The versions or configurations affected.
- The corrective action.
- Any recommended user steps.

Sensitive exploit details, personal information, credentials, and unnecessary technical material should not be disclosed.

---

## 10. Exposed Credentials and Secrets

Credentials and secrets must never be committed intentionally to public repositories.

This includes:

- API keys.
- Access tokens.
- Passwords.
- Private keys.
- Database credentials.
- Session secrets.
- Cloud provider credentials.
- Webhook secrets.
- Service account credentials.
- Private environment configuration.

If a credential is accidentally exposed, deleting the visible file or commit is not sufficient.

The appropriate response is to:

1. Revoke or disable the exposed credential immediately.
2. Generate a replacement through the relevant provider.
3. Review available logs for suspicious use.
4. Identify affected systems, integrations, and environments.
5. Remove the exposed value from the repository and, where appropriate, its Git history.
6. Review related configuration and deployment processes.
7. Update relevant documentation and incident records.

Credential rotation takes priority over repository cleanup.

A token that has been published must be treated as compromised, even if the commit is later deleted or the repository is made private.

Contributors must not attempt to reuse, validate, or investigate exposed credentials unless explicitly authorized.

---

## 11. Data Protection and Confidential Information

Security reports, investigations, and remediation work must respect the Lab's confidentiality and data-protection principles.

The following must not be published in issues, pull requests, documentation, or public demonstrations:

- Personal data without an appropriate legal basis.
- Private user information.
- Confidential research material.
- Private project source code.
- Proprietary implementation details.
- Internal credentials or access tokens.
- Non-public business or operational information.
- Third-party materials without appropriate authorization.

This requirement applies even when the information was discovered during a legitimate security investigation.

Public accessibility is not equivalent to publication authorization.

The Lab's public research activities must remain separate from proprietary or confidential work. A security investigation must not become a route for transferring private project material into the public repository.

---

## 12. Dependency and Supply Chain Security

Third-party libraries, packages, models, plugins, services, and development tools can introduce security risks into otherwise well-designed systems.

Projects should consider the following practices where applicable:

- Prefer dependencies with an identifiable maintainer and active maintenance history.
- Review dependency permissions and licensing conditions.
- Avoid unnecessary packages and integrations.
- Monitor relevant security advisories.
- Update vulnerable dependencies when appropriate.
- Review package installation and build scripts.
- Avoid executing untrusted code during development or deployment.
- Protect CI/CD secrets and deployment credentials.
- Pin or constrain dependency versions where reproducibility and risk management require it.

GitHub security features may be used to support these practices, including:

- Dependabot alerts and security updates.
- Secret scanning.
- Code scanning.
- Dependency review.
- Private vulnerability reporting.

The availability of these features does not mean they are automatically enabled or configured for every repository.

Their use should be evaluated and configured according to project needs.

---

## 13. AI Security and Model Supply Chains

Projects involving artificial intelligence must consider risks beyond conventional application security.

The Lab recognizes that AI systems may process untrusted inputs, invoke external tools, retrieve protected information, and generate outputs that are not inherently safe.

Where relevant, AI-enabled projects should consider:

### Input and Context Security

- Treat user-provided content as untrusted input.
- Separate trusted instructions from untrusted content.
- Avoid allowing external content to override security boundaries.
- Validate files, documents, and external data before processing.

### Agent and Tool Security

- Apply least-privilege access to tools and integrations.
- Restrict sensitive operations behind explicit authorization.
- Validate tool arguments before execution.
- Require confirmation for consequential operations where appropriate.
- Prevent model output from becoming executable instructions without validation.

### Data and Retrieval Security

- Enforce access permissions independently of model behavior.
- Avoid placing secrets or unnecessary sensitive information in prompts.
- Separate user sessions and data contexts.
- Review retrieval permissions and document-level access controls.
- Avoid exposing internal context through generated responses.

### Model and Provider Security

- Protect API credentials and model access tokens.
- Review provider data-handling policies.
- Evaluate model and dependency provenance where relevant.
- Monitor changes to external model behavior and interfaces.
- Document important model limitations and security assumptions.

No AI model should be treated as a security boundary or as a substitute for application-level access control.

---

## 14. Security Responsibilities

### 14.1 Maintainer

The maintainer is responsible for:

- Reviewing and assessing received vulnerability reports.
- Determining whether an issue falls within the Lab's scope.
- Coordinating remediation where appropriate.
- Protecting sensitive details during investigation.
- Reviewing security implications before publication.
- Updating relevant documentation.
- Communicating material security findings when appropriate.

These responsibilities are maintained on a best-effort basis and do not imply a dedicated security operations team.

### 14.2 Contributors

Contributors are expected to:

- Follow secure development practices.
- Avoid committing secrets or confidential information.
- Review dependencies and external integrations.
- Validate untrusted inputs.
- Avoid introducing unnecessary permissions.
- Report suspected vulnerabilities privately.
- Refrain from unauthorized testing.
- Address security feedback before changes are merged.

AI-assisted development does not remove contributor responsibility for reviewing code, dependencies, generated configurations, or execution behavior.

### 14.3 Users

Users are responsible for evaluating the suitability of a project before deploying it in production or using it to process sensitive information.

Experimental software should be tested in an appropriate environment before being connected to critical infrastructure, confidential datasets, or operational services.

Project-specific documentation may impose additional security requirements.

---

## 15. Security in Experimental and Prototype Projects

Framing Creativity Lab publishes research, experiments, and prototypes that may not have reached production maturity.

Such projects may have incomplete security controls, limited testing, or dependencies on external experimental services.

Unless explicitly documented otherwise:

- Experimental projects must not be assumed to be production-ready.
- Demonstrations must not use real sensitive data without appropriate safeguards.
- Credentials must be managed outside public source code.
- External integrations must use appropriately restricted credentials.
- Public deployments should be reviewed for unintended access.
- Known limitations should be documented.
- Security-relevant risks should be considered before public release.

A prototype's experimental status does not justify publishing exposed credentials, private data, or avoidable security weaknesses.

---

## 16. Public Advisories and Security Updates

When a vulnerability has been confirmed and addressed, the Lab may publish a security advisory or relevant project update.

Disclosure should balance transparency with the need to avoid enabling further exploitation.

Depending on the issue, a public advisory may include:

- Affected project and versions.
- Vulnerability category.
- Severity assessment.
- Impact description.
- Remediation details.
- Upgrade or mitigation instructions.
- Acknowledgment of the reporter, where appropriate and authorized.

Reporters will not be publicly identified without their consent.

If a vulnerability cannot be fully corrected, the Lab may document the remaining risk, restrict access to the affected project, withdraw the affected release, or discontinue the project.

---

## 17. Security Records and Documentation

Security-related decisions should be documented to an appropriate level.

Records may include:

- Report reference.
- Affected project and version.
- Date received and assessed.
- Severity classification.
- Investigation findings.
- Remediation decisions.
- Validation results.
- Disclosure status.

Sensitive exploit details, credentials, and personal information must not be placed in public documentation.

Security records should be retained only as necessary for maintenance, accountability, and legitimate operational purposes.

---

## 18. Policy Limitations

This policy describes the Lab's intended security practices and reporting expectations.

It does not constitute:

- A guarantee that all vulnerabilities will be detected.
- A guarantee of a particular response or remediation time.
- A security certification or compliance statement.
- A warranty that published software is free from vulnerabilities.
- Authorization to test third-party systems.
- A commitment to maintain every historical release indefinitely.

Project-specific documentation may define additional requirements or limitations.

---

## 19. Policy Review and Updates

This policy may be updated as the Lab evolves, adopts new technologies, or changes its development and publication practices.

Changes should preserve the following principles:

- Responsible disclosure.
- Protection of users and contributors.
- Confidentiality of non-public information.
- Proportionate risk assessment.
- Clear accountability.
- Transparency about security limitations.

The maintainer is responsible for approving changes to this policy.

---

## 20. Related Documents

This policy should be read alongside:

- `README.md` — Lab identity, scope, and operating principles.
- `LAB-CHARTER.md` — Governance, independence, and foundational principles.
- `PUBLICATION-POLICY.md` — Public release, confidentiality, and intellectual property requirements.
- `RESEARCH-METHODOLOGY.md` — Research and experimental practices.
- `CONTRIBUTING.md` — Contributor responsibilities and development workflow.

---

## 21. Closing Principle

Security is not a claim of absolute protection. It is a continuous responsibility.

Framing Creativity Lab aims to develop and publish work with an appropriate level of care, technical discipline, and transparency.

The objective is not to eliminate every possible risk, but to identify meaningful weaknesses, reduce avoidable exposure, respond responsibly, and learn from the process.

**Build with curiosity. Publish with care. Maintain with responsibility.**
