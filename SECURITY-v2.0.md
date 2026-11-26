# Framing Creativity Lab — Security Policy

**Document ID:** FCL-SEC-001  
**Version:** 2.0  
**Status:** Draft for Maintainer Review  
**Effective Date:** Pending approval  
**Maintainer:** J-ART  
**Repository:** Framing Creativity Lab

---

## 1. Purpose

Framing Creativity Lab (the Lab) considers security an integral part of research, experimentation, software development, and publication.

Security must be considered throughout the lifecycle of a project, from initial design and development to evaluation, release, maintenance, and withdrawal.

This policy establishes the principles, responsibilities, and procedures governing the identification, reporting, assessment, remediation, and disclosure of security vulnerabilities affecting work published under the Framing Creativity Lab identity.

Its objectives are to:

- Establish responsible vulnerability reporting and disclosure practices.
- Protect users, contributors, maintainers, and third parties.
- Reduce the risk of unauthorized access, data exposure, and system compromise.
- Define appropriate security assessment and incident-handling practices.
- Address risks associated with AI-enabled systems and emerging technologies.
- Clarify the security responsibilities of the maintainer, contributors, and users.
- Support proportionate security controls for research, experiments, prototypes, and operational systems.
- Preserve confidentiality, privacy, intellectual property, and publication boundaries.

Security is a continuous responsibility. A successful build, technical demonstration, or publication review does not establish that a system is free from vulnerabilities.

---

## 2. Scope

This policy applies to software, technical resources, and systems developed, maintained, or published under the Framing Creativity Lab identity, to the extent that they are under the Lab's control.

Depending on the project, this may include:

- Source code and application logic.
- Web applications and APIs.
- Development scripts and command-line tools.
- Build, deployment, and automation workflows.
- Infrastructure definitions and project configuration.
- Authentication and authorization mechanisms.
- Data storage and processing components.
- Third-party dependencies and packages.
- AI integrations, agents, and experimental workflows.
- Connected tools and external service integrations.
- Documentation containing operational or security-sensitive information.
- Public demonstrations and deployed prototypes.

The policy covers vulnerabilities introduced by the Lab's own work or by configurations and integrations for which the Lab is responsible.

### 2.1 External Services and Providers

The policy does not give the Lab authority over services, platforms, providers, models, or infrastructure operated by third parties.

Vulnerabilities affecting an external provider should normally be reported to the provider or its designated security team.

The Lab may assess the consequences for its own implementation, suspend an affected integration, or take other proportionate protective measures.

It cannot guarantee remediation by an external provider.

### 2.2 Project-Specific Requirements

Individual projects may establish additional security requirements according to their architecture, exposure, data, intended use, and risk.

Project-specific requirements may be stricter than this policy.

They must not be used to bypass the Lab's fundamental security, privacy, confidentiality, or publication requirements.

---

## 3. Security Support and Project Maturity

Security support must be understood in the context of each project's lifecycle and technical maturity.

Unless a project-specific policy states otherwise, the following expectations apply:

| Project state or release | Security expectations |
|---|---|
| Default branch | Primary development and maintenance target |
| Latest published release | Security review and remediation considered where the project remains maintained |
| Older releases | No guarantee of continued security updates |
| Archived projects | Not actively maintained unless explicitly stated |
| Discontinued projects | No ongoing maintenance commitment |
| Experimental projects | Proportionate security review; no production security guarantee |
| Demonstrations and prototypes | Limited assurance; unsuitable for sensitive workloads unless explicitly assessed and authorized |

The presence of publicly accessible code does not imply that a project is:

- Production-ready.
- Security-certified.
- Independently audited.
- Suitable for processing sensitive information.
- Guaranteed to receive ongoing maintenance.
- Free from known or unknown vulnerabilities.

Technical maturity, operational readiness, project status, and publication status are separate assessments.

They must not be treated as interchangeable security assurances.

---

## 4. Security Principles

Security decisions and implementation practices should follow these principles.

### 4.1 Confidentiality, Integrity, and Availability

Security controls should protect:

- **Confidentiality** — Information must be accessible only to appropriately authorized parties.
- **Integrity** — Systems and data must be protected against unauthorized or improper modification.
- **Availability** — Systems and services should remain available according to their intended operating requirements.

### 4.2 Least Privilege

Users, services, applications, agents, and integrations should receive only the permissions necessary for their defined responsibilities.

Unnecessary permissions should be avoided.

### 4.3 Defence in Depth

Security should not depend on a single control.

Where appropriate, systems should combine authentication, authorization, input validation, isolation, logging, monitoring, and recovery measures.

### 4.4 Secure Defaults

Configurations should favour restricted access and safe behaviour by default.

Unsafe or privileged functionality should require explicit configuration or authorization.

### 4.5 Data Minimization

Systems should collect, process, retain, and expose only the information necessary for their defined purpose.

### 4.6 Transparency and Accountability

Security limitations, assumptions, relevant dependencies, and material incidents should be documented appropriately.

Transparency does not authorize disclosure of credentials, vulnerabilities, confidential information, or protected implementation details.

### 4.7 Proportionality

Security controls should reflect the actual risk and intended use of the project.

A small experiment does not require the same controls as a public-facing operational service. However, an experimental status does not justify avoidable exposure or unsafe handling of protected information.

---

## 5. What Qualifies as a Security Vulnerability?

A security vulnerability is a weakness that could compromise the confidentiality, integrity, or availability of a system, its information, or its users.

The following examples are not exhaustive.

### 5.1 Application and Software Security

Examples include:

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
- Insecure session management.
- Improper validation of security-critical inputs.

### 5.2 Infrastructure and Configuration

Examples include:

- Hardcoded credentials or API keys.
- Exposed environment variables or secrets.
- Misconfigured repository or service permissions.
- Insecure deployment configurations.
- Unprotected administrative interfaces.
- Insecure network or storage configurations.
- Vulnerable or improperly configured dependencies.
- Weak cryptographic practices.
- Unsafe automation or CI/CD workflows.
- Public exposure of private storage or administrative resources.

### 5.3 Data and Privacy

Examples include:

- Unauthorized access to personal or confidential information.
- Accidental disclosure of private datasets.
- Improper data retention or deletion.
- Exposure of authentication tokens.
- Leakage through application logs or error messages.
- Insecure handling of uploaded files.
- Data leakage across users, sessions, or environments.
- Unauthorized transmission to external services.
- Failure to enforce data access restrictions.

### 5.4 AI and Emerging Technologies

AI-enabled applications introduce additional security considerations.

Potential vulnerabilities include:

- Prompt injection that compromises security boundaries.
- Leakage of confidential context or protected information.
- Unauthorized tool execution by AI agents.
- Inadequate isolation between users, sessions, or agent tasks.
- Retrieval-augmented generation (RAG) access-control failures.
- Unsafe execution of model-generated code or commands.
- Improper validation of model-generated outputs.
- Exposure of model credentials or service tokens.
- Insecure handling of uploaded files or untrusted model inputs.
- Manipulation of agent workflows through external content.
- Abuse of connected tools, integrations, or services.
- Unauthorized external actions initiated through model-mediated workflows.

AI-related behaviour should be assessed according to its actual security impact.

Unexpected, inaccurate, or low-quality model output is not necessarily a security vulnerability. It becomes a security concern when it causes or enables an unauthorized action, access violation, disclosure, or other material security consequence.

AI security requirements are further defined in `RESPONSIBLE-AI-v2.0.md`.

---

## 6. Issues Outside the Scope of This Policy

The following are generally not considered security vulnerabilities unless they create a demonstrable security impact:

- Ordinary software defects without a security consequence.
- Visual or usability inconsistencies.
- Feature requests.
- Performance issues without an availability or security impact.
- Theoretical weaknesses without a credible attack path.
- Model hallucinations without a security consequence.
- General requests for security hardening.
- Issues affecting third-party products that are not caused by the Lab's implementation.
- Findings requiring access to systems or data outside the reporter's authorization.

These matters may still be relevant to normal project maintenance or quality review.

Third-party vulnerabilities should be reported to the relevant provider.

---

## 7. Vulnerability Reporting

Security vulnerabilities must be reported privately.

They must not be disclosed through public GitHub issues, discussions, pull requests, comments, or other publicly accessible channels.

### 7.1 Preferred Reporting Channel

The preferred reporting method is GitHub Private Vulnerability Reporting for the Framing Creativity Lab repository, provided that the feature has been enabled and verified by the maintainer.

When available, reporters should use the repository's Security area and the private vulnerability reporting function.

The feature must not be described as operational merely because GitHub provides it as a platform capability.

**Operational status:** Availability and configuration of GitHub Private Vulnerability Reporting for this repository have not yet been verified by the maintainer. Until verified, this policy does not claim that an operational private reporting channel is available.

### 7.2 Alternative Contact

An alternative private security contact may be used only when it has been explicitly published by the maintainer in this policy or through another official Lab channel.

No unpublished email address, private contact method, or personal communication channel should be assumed.

If no verified private reporting route is available, the maintainer must establish and publish one before inviting external security reports.

Reporters should not disclose vulnerability details through a public issue as a substitute for private reporting.

### 7.3 Information to Include

A useful security report should include, where possible:

1. A concise description of the suspected vulnerability.
2. The affected repository, project, component, or version.
3. The conditions required to reproduce the issue.
4. A step-by-step explanation of the reproduction process.
5. The potential impact and affected security properties.
6. Supporting evidence, such as sanitized logs or screenshots.
7. A suggested mitigation, if known.
8. Relevant technical context or environmental requirements.
9. Whether the issue may affect other versions or deployments.

A report should contain enough information to support assessment without exposing unnecessary personal, confidential, or third-party data.

A complete exploit or proof of compromise is not required.

### 7.4 Good-Faith Reporting

Reporters are expected to:

- Report suspected vulnerabilities privately.
- Act within the scope of their authorization.
- Avoid accessing data that does not belong to them.
- Avoid modifying or deleting third-party information.
- Avoid disrupting systems or services.
- Avoid testing against real users.
- Share only the minimum technical evidence necessary.
- Stop testing when unauthorized access or sensitive information is encountered.
- Respect applicable laws and third-party terms.

The Lab does not authorize security testing against unrelated systems, external services, or infrastructure operated by third parties.

### 7.5 No Bug Bounty Commitment

This policy does not establish a paid bug bounty programme.

It does not promise financial rewards, compensation, employment, or formal recognition for vulnerability reports.

Any such arrangement would require a separate, explicit authorization.

---

## 8. Responsible and Coordinated Disclosure

Framing Creativity Lab supports responsible and coordinated vulnerability disclosure.

The objective is to reduce harm while enabling vulnerabilities to be investigated and addressed.

Reporters should avoid public disclosure while a reasonable remediation process is underway, particularly where public details could enable exploitation.

The maintainer will make reasonable efforts to:

- Assess legitimate reports.
- Request additional information where necessary.
- Determine the affected scope.
- Coordinate remediation where appropriate.
- Communicate material findings to the reporter where possible.
- Consider coordinated public disclosure after the relevant risks have been addressed.

### 8.1 Disclosure Timing

The appropriate disclosure timeline depends on:

- Severity and exploitability.
- The affected systems and users.
- Availability of a reliable correction.
- Whether active exploitation is suspected.
- Third-party dependencies.
- Legal or contractual obligations.
- The risk of continued exposure.

No fixed acknowledgement, response, remediation, or disclosure deadline is guaranteed.

### 8.2 Researcher Recognition

A reporter may be acknowledged in a security advisory or release note where appropriate.

Public identification requires the reporter's consent.

A report does not automatically establish authorship of the affected project or ownership of the vulnerability information.

---

## 9. Vulnerability Severity Assessment

Reported vulnerabilities should be assessed according to their practical impact, exploitability, affected assets, and potential consequences.

The following categories provide an internal assessment framework.

| Severity | General interpretation |
|---|---|
| Critical | A vulnerability enabling severe compromise, such as remote code execution, broad unauthorized access, or major exposure of sensitive data. |
| High | A vulnerability that could lead to significant unauthorized access, privilege escalation, or compromise of important functionality or information. |
| Medium | A weakness with meaningful but constrained security impact, often requiring specific conditions or additional access. |
| Low | A limited security weakness with restricted impact or difficult exploitation. |
| Informational | A security observation, hardening recommendation, or issue without a demonstrated vulnerability. |

### 9.1 Assessment Factors

The maintainer may consider:

- Ease of exploitation.
- Required access or privileges.
- User interaction.
- Confidentiality impact.
- Integrity impact.
- Availability impact.
- Scope of affected systems.
- Sensitivity of exposed information.
- Potential for further compromise.
- Availability of mitigations.
- Existing safeguards.
- Exposure of third-party systems or data.

### 9.2 Supporting Frameworks

Where appropriate, the Common Vulnerability Scoring System (CVSS) may be used as a supporting assessment framework.

A numerical score does not replace contextual analysis.

The final classification should reflect the actual risk within the affected project and its intended operating environment.

### 9.3 AI Risk Is Separate

The AI Risk Classification defined in `RESPONSIBLE-AI-v2.0.md` uses the values A0–A4.

It assesses the risk associated with an AI system or application.

It is not a vulnerability severity scale and must not replace the Critical, High, Medium, Low, or Informational severity assessment defined in this policy.

Both assessments may be relevant to the same project.

---

## 10. Vulnerability Handling Process

Security reports should be handled through a structured process.

### Stage 1 — Receipt

The maintainer receives the private report through an established reporting channel.

The report may be acknowledged and additional evidence requested where necessary.

### Stage 2 — Triage

The issue is assessed to determine:

- Whether it is reproducible.
- Whether it falls within the Lab's scope.
- Which components and versions are affected.
- Whether the issue has been publicly exposed.
- Its likely severity and practical impact.
- Whether immediate containment is required.
- Whether third-party systems or services are involved.

### Stage 3 — Investigation

The maintainer investigates the reported weakness in a controlled environment.

The investigation should:

- Preserve relevant evidence.
- Avoid unnecessary access to sensitive information.
- Limit testing to authorized systems.
- Identify the likely root cause.
- Determine the scope of affected components.
- Assess the possibility of active exploitation.

Investigation must not extend into third-party systems without authorization.

### Stage 4 — Containment and Mitigation

Where a vulnerability is confirmed or a credible risk requires immediate action, mitigation may include:

- Restricting or disabling vulnerable functionality.
- Revoking or rotating exposed credentials.
- Removing affected integrations.
- Restricting repository or service access.
- Updating vulnerable dependencies.
- Changing configuration or permissions.
- Temporarily withdrawing a release or prototype.
- Restricting access to affected data.
- Disabling external actions or agent capabilities.

Containment should prioritize preventing further unauthorized access or harm.

### Stage 5 — Remediation

The underlying weakness should be corrected where practical.

Remediation may involve:

- Correcting affected code.
- Strengthening authorization.
- Improving input validation.
- Implementing additional isolation.
- Removing unnecessary permissions.
- Updating dependencies.
- Revising deployment configurations.
- Improving logging and monitoring.
- Updating security documentation.

### Stage 6 — Validation

The proposed correction should be reviewed and tested.

Validation should consider whether:

- The original vulnerability has been addressed.
- The corrective change introduces an obvious regression.
- Related components have been assessed.
- Relevant security assumptions remain valid.
- The mitigation is effective under the affected conditions.
- Documentation has been updated.

Validation must not be described as comprehensive if only limited testing was performed.

### Stage 7 — Disclosure and Closure

When appropriate, the Lab may publish a security advisory or release note describing:

- The affected component.
- The vulnerability category.
- The practical impact.
- The versions or configurations affected.
- The corrective action.
- Recommended user steps.
- Relevant acknowledgements, where authorized.

Sensitive exploit details, credentials, personal information, and unnecessary technical material must not be disclosed.

The outcome and relevant decisions should be recorded appropriately.

---

## 11. Security Incidents

A security incident is an event that has caused, or may reasonably cause, unauthorized access, disclosure, modification, disruption, or compromise of a system, its data, or its users.

An incident may involve a confirmed vulnerability, exposed credentials, unauthorized access, a data leak, or an unsafe external integration.

### 11.1 Examples

Security incidents may include:

- Exposure of API keys or access tokens.
- Unauthorized access to a repository or deployment.
- Public disclosure of confidential information.
- Compromise of an account or service.
- Unauthorized modification of code or configuration.
- Data leakage between users or environments.
- Abuse of an AI agent or connected tool.
- Unauthorized access to retrieved or stored information.
- Malicious modification of a dependency.
- Compromise of a deployment or automation workflow.

### 11.2 Incident Response

The response should be proportionate to the nature and severity of the incident.

Depending on the circumstances, it may include:

1. Identifying and containing the incident.
2. Preventing further unauthorized access or actions.
3. Revoking or rotating affected credentials.
4. Protecting affected data and systems.
5. Preserving relevant evidence.
6. Identifying the source and scope of the incident.
7. Assessing potential impact.
8. Correcting the underlying weakness.
9. Testing the remediation.
10. Reassessing affected permissions and risks.
11. Documenting the incident and relevant lessons.
12. Communicating material information where appropriate.

### 11.3 Personal Data and Confidentiality Incidents

Where an incident involves personal, confidential, or restricted information, the response must also consider:

- Applicable data-protection obligations.
- Contractual confidentiality requirements.
- The classification of affected information.
- The number and type of affected individuals.
- Potential harm resulting from disclosure.
- Whether notification or other protective action is required.
- Relevant third-party or provider obligations.

Any required notification must be assessed according to the applicable legal and contractual framework.

This policy does not replace legal advice or establish a universal notification deadline.

### 11.4 Suspension

Where a system presents an unacceptable or uncontrolled risk, the maintainer may:

- Disable affected functionality.
- Restrict access.
- Suspend an integration.
- Pause a deployment.
- Withdraw a release.
- Suspend publication.
- Discontinue an affected project.

The ability to pause or restrict consequential functionality should be considered during system design where appropriate.

### 11.5 Post-Incident Review

Following a material incident, the affected project should be reassessed before normal operation resumes.

The review should consider:

- Root cause.
- Scope and impact.
- Effectiveness of the response.
- Adequacy of existing safeguards.
- Required architectural or configuration changes.
- Permission and access changes.
- Relevant documentation updates.
- Whether publication approval remains appropriate.
- Lessons for other Lab projects.

---

## 12. Exposed Credentials and Secrets

Credentials and secrets must never be intentionally committed to public repositories.

Examples include:

- API keys.
- Access tokens.
- Passwords.
- Private keys.
- Database credentials.
- Session secrets.
- Cloud provider credentials.
- Webhook secrets.
- Service account credentials.
- Private certificates.
- Sensitive environment configuration.

### 12.1 Immediate Response

If a credential is accidentally exposed, the credential must be treated as compromised.

The appropriate response is to:

1. Revoke or disable the exposed credential immediately.
2. Generate a replacement through the relevant provider.
3. Review available logs for suspicious activity.
4. Identify affected systems, integrations, and environments.
5. Remove the exposed value from the repository.
6. Assess whether Git history cleanup is necessary.
7. Review related configurations and deployment processes.
8. Update relevant records and documentation.

Credential rotation takes priority over repository cleanup.

Deleting the visible file or commit is not sufficient.

A credential that has been published must be treated as compromised even if the commit is later deleted or the repository becomes private.

### 12.2 Investigation Restrictions

Contributors must not attempt to reuse, validate, or investigate exposed credentials unless explicitly authorized.

Credential exposure should be handled through a controlled process.

---

## 13. Data Protection and Information Classification

Security and data protection must be considered together.

The Lab's canonical data classification framework is defined in `PUBLICATION-POLICY-v2.0.md` and `RESPONSIBLE-AI-v2.0.md`.

The four classifications are:

| Classification | General security treatment |
|---|---|
| Public | Information explicitly approved or otherwise authorized for public distribution. |
| Internal | Non-public working information intended for authorized Lab use. |
| Confidential | Information subject to confidentiality obligations, restricted access, or material disclosure risk. |
| Restricted | Highly sensitive, legally or contractually restricted, security-critical, or otherwise unsuitable for ordinary disclosure. |

### 13.1 Personal and Sensitive Information

Personal information should be classified at least as Confidential under the Lab's internal framework.

Sensitive personal information, security-critical information, or information subject to stricter restrictions should be classified as Restricted.

Personal and sensitive information are characteristics of data, not additional values in the four-level classification vocabulary.

### 13.2 Handling Requirements

Projects should:

- Minimize the collection and processing of personal information.
- Use synthetic or public data where practical.
- Restrict access to authorized users and services.
- Protect information in transit and at rest where appropriate.
- Avoid unnecessary retention.
- Review external processing and storage arrangements.
- Apply appropriate deletion and retention practices.
- Avoid exposing sensitive information in logs, prompts, documentation, or demonstrations.

### 13.3 External Services

Information must not be transmitted to an external provider merely because an API or integration permits it technically.

The responsible person must assess:

- Data classification.
- Purpose of processing.
- Authorization and legal basis.
- Provider terms.
- Data retention and processing conditions.
- Geographic processing where relevant.
- Applicable safeguards.
- Confidentiality and contractual restrictions.

Confidential and Restricted information require particular care and must not be transferred without an explicitly established basis, appropriate authorization, and safeguards.

---

## 14. Dependency and Supply Chain Security

Third-party libraries, packages, models, plugins, services, and development tools may introduce security risks.

Projects should consider the following practices where applicable:

- Prefer dependencies with identifiable maintainers and a credible maintenance history.
- Review dependency permissions and licensing conditions.
- Avoid unnecessary packages and integrations.
- Monitor relevant security advisories.
- Update vulnerable dependencies where appropriate.
- Review package installation and build scripts.
- Avoid executing untrusted code during development or deployment.
- Protect CI/CD secrets and deployment credentials.
- Pin or constrain dependency versions where reproducibility and risk management require it.
- Review transitive dependencies where relevant.
- Assess model and artifact provenance where practical.

### 14.1 GitHub Security Features

GitHub provides security capabilities that may support repository security, depending on repository configuration and platform availability.

These may include:

- Dependabot alerts.
- Dependabot security updates.
- Secret scanning.
- Push protection.
- Code scanning.
- Dependency review.
- Private vulnerability reporting.
- Security advisories.

The existence of a GitHub feature does not mean that it is enabled or configured for this repository.

**Configuration status:** The activation and configuration of these controls must be verified by the maintainer. This policy does not represent any unverified feature as active.

### 14.2 Security Configuration Review

The maintainer should periodically assess which GitHub security features are appropriate for the repository.

Where a feature is enabled, its operation and notifications should be checked.

Where a feature is unavailable or unsuitable, alternative controls should be considered where appropriate.

---

## 15. AI Security and Model Supply Chains

AI-enabled systems may process untrusted inputs, retrieve protected information, invoke external tools, and generate outputs that are not inherently safe.

AI security requirements are defined in greater detail in `RESPONSIBLE-AI-v2.0.md`.

### 15.1 Input and Context Security

Where relevant:

- Treat user-provided content as untrusted input.
- Separate trusted instructions from untrusted content.
- Validate uploaded files and external data.
- Prevent external content from overriding security boundaries.
- Avoid exposing confidential context unnecessarily.
- Control how retrieved information enters model context.

### 15.2 Prompt Injection and Adversarial Inputs

Systems should consider malicious or unexpected inputs that attempt to:

- Override system or developer instructions.
- Change agent behaviour.
- Trigger unauthorized tools.
- Circumvent access restrictions.
- Manipulate retrieval or reasoning context.
- Exfiltrate protected information.
- Cause unintended external actions.

Security boundaries must be enforced by the application and its supporting systems, not by relying solely on the model to follow instructions.

### 15.3 Agent and Tool Security

AI agents and connected tools should:

- Use least-privilege permissions.
- Enforce independent authorization checks.
- Validate tool arguments.
- Restrict access to sensitive operations.
- Require confirmation for consequential actions where appropriate.
- Separate user sessions and execution contexts.
- Limit the impact of unexpected model behaviour.
- Avoid executing untrusted generated code in privileged environments.

A model-generated response must not independently authorize a sensitive operation.

### 15.4 Retrieval and Knowledge Systems

Retrieval-augmented systems should enforce access controls independently of model behaviour.

Projects should consider:

- Document-level permissions.
- User and session isolation.
- Retrieval scope.
- Source validation.
- Data classification.
- Protection against unauthorized context disclosure.
- Retention and deletion requirements.

### 15.5 Model and Provider Security

Where relevant, projects should assess:

- Provider security practices.
- Model and service access permissions.
- API credential protection.
- Model and artifact provenance.
- Data retention and processing terms.
- External tool permissions.
- Provider changes and dependencies.
- Known model limitations.

Provider security claims should be based on relevant provider documentation or independently available evidence.

Unverified claims must not be presented as established facts.

### 15.6 AI Security Incidents

AI-related security incidents should be managed under this policy.

Potential confidentiality, privacy, AI risk, and publication consequences must also be assessed under `RESPONSIBLE-AI-v2.0.md` and `PUBLICATION-POLICY-v2.0.md`.

---

## 16. Security Responsibilities

### 16.1 Founder and Maintainer

Under the current founder-led governance model, the founder and maintainer is responsible for:

- Reviewing and assessing received vulnerability reports.
- Determining whether an issue falls within the Lab's scope.
- Coordinating investigation and remediation where appropriate.
- Protecting sensitive details during investigation.
- Assessing relevant security and publication implications.
- Managing repository access and security configuration.
- Reviewing security implications before publication.
- Updating relevant security documentation.
- Communicating material security findings where appropriate.
- Deciding whether functionality or publication should be restricted, suspended, or withdrawn.

These responsibilities are performed on a best-effort basis.

They do not imply the existence of a dedicated security operations team or guaranteed response capacity.

### 16.2 Contributors

Contributors are expected to:

- Follow secure development practices.
- Avoid committing secrets or confidential information.
- Review dependencies and external integrations.
- Validate untrusted inputs.
- Avoid introducing unnecessary permissions.
- Protect sensitive information.
- Report suspected vulnerabilities privately.
- Refrain from unauthorized testing.
- Address security feedback before changes are integrated.
- Disclose relevant security assumptions and limitations.

AI-assisted development does not remove contributor responsibility for reviewing code, dependencies, generated configurations, or execution behaviour.

### 16.3 Users

Users are responsible for evaluating the suitability of a project before deployment or use with sensitive information.

They should:

- Review the project's documentation and stated maturity.
- Understand known limitations.
- Apply appropriate configuration.
- Protect credentials and access permissions.
- Test experimental software in suitable environments.
- Avoid connecting prototypes to critical infrastructure without appropriate assessment.
- Monitor relevant updates and security advisories.

Project-specific documentation may impose additional security requirements.

---

## 17. Experimental and Prototype Security

Framing Creativity Lab publishes research, experiments, prototypes, and other work that may not have reached production maturity.

Such projects may have incomplete security controls, limited testing, or dependencies on external experimental services.

Unless explicitly documented otherwise:

- Experimental projects must not be assumed to be production-ready.
- Demonstrations must not use real sensitive data without appropriate safeguards.
- Credentials must be managed outside public source code.
- External integrations must use appropriately restricted credentials.
- Public deployments should be reviewed for unintended access.
- Known security limitations should be documented.
- Security risks should be assessed before public release.
- Operational use should remain within the project's stated readiness.

An experimental status does not justify publishing exposed credentials, private information, or avoidable security weaknesses.

### 17.1 Proportionate Assessment

The level of security assessment should reflect:

- Intended use.
- External exposure.
- Data sensitivity.
- User population.
- Available permissions.
- Connected services.
- Potential impact of failure.
- Technical maturity.
- Operational readiness.

Projects handling sensitive information or enabling consequential external actions require more rigorous assessment than isolated demonstrations.

---

## 18. Security Advisories and Public Updates

When a vulnerability has been confirmed and appropriately addressed, the Lab may publish a security advisory or relevant project update.

Disclosure should balance transparency with the need to avoid enabling further exploitation.

Depending on the issue, a public advisory may include:

- Affected project and versions.
- Vulnerability category.
- Severity assessment.
- Impact description.
- Remediation details.
- Upgrade or mitigation instructions.
- Relevant limitations.
- Reporter acknowledgement, where authorized.

### 18.1 Sensitive Details

Public advisories must not disclose:

- Active credentials.
- Personal information.
- Confidential implementation details.
- Unnecessary exploit instructions.
- Restricted datasets.
- Third-party confidential information.
- Details that materially increase the risk of further exploitation.

### 18.2 Unresolved Vulnerabilities

If a vulnerability cannot be fully corrected, the Lab may:

- Document the remaining risk.
- Restrict access to the affected project.
- Disable vulnerable functionality.
- Withdraw an affected release.
- Suspend publication.
- Discontinue the affected project.

The public explanation should be accurate without disclosing additional sensitive information.

### 18.3 Reporter Acknowledgement

Reporters will not be publicly identified without their consent.

Recognition must not imply a formal security research partnership or financial arrangement unless explicitly agreed.

---

## 19. Security Records and Documentation

Security-related decisions should be documented to an appropriate level.

Records may include:

- Report reference.
- Affected project and version.
- Date received and assessed.
- Severity classification.
- Investigation findings.
- Relevant containment actions.
- Remediation decisions.
- Validation results.
- Disclosure status.
- Relevant follow-up actions.

Records should be proportionate to the incident and its consequences.

### 19.1 Confidentiality of Records

Sensitive exploit details, credentials, personal information, and restricted material must not be placed in public documentation.

Access to non-public security records should be limited to individuals with an authorized need.

### 19.2 Retention

Security records should be retained only as necessary for legitimate maintenance, accountability, security, contractual, or legal purposes.

Retention should consider applicable obligations and the sensitivity of the records.

---

## 20. Policy Limitations

This policy describes the Lab's intended security practices and reporting expectations.

It does not constitute:

- A guarantee that all vulnerabilities will be detected.
- A guarantee of a particular response or remediation time.
- A dedicated security operations service.
- A paid bug bounty programme.
- A security certification or compliance statement.
- A warranty that published software is free from vulnerabilities.
- Authorization to test third-party systems.
- A guarantee that every historical release will be maintained indefinitely.
- A guarantee that third-party providers will remediate their vulnerabilities.

Project-specific documentation may define additional requirements or limitations.

---

## 21. Policy Review and Maintenance

This policy should be reviewed when:

- The Lab's governance model changes.
- The security reporting process changes.
- New security capabilities or controls are introduced.
- Material changes are made to the repository or deployment environment.
- New technologies introduce additional attack surfaces.
- Relevant legal, contractual, or platform requirements change.
- A material incident identifies a necessary improvement.

The founder and maintainer is responsible for approving revisions under the current governance model.

Substantive revisions should update the document version and be recorded in version control.

Changes should be checked for consistency with the Lab Charter, Governance, Publication Policy, Responsible AI Policy, and Contribution Guidelines.

---

## 22. Related Documents

This policy should be read alongside:

| Document | Relevance |
|---|---|
| `LAB-CHARTER-v2.0.md` | Foundational principles and operating boundaries |
| `GOVERNANCE-v2.0.md` | Security responsibilities, access, and decision authority |
| `PUBLICATION-POLICY-v2.0.md` | Confidentiality, data classification, security review, and publication withdrawal |
| `RESPONSIBLE-AI-v2.0.md` | AI-specific risk, data handling, agent security, and incident management |
| `QUALITY-STANDARDS-v2.0.md` | Engineering quality, validation, and technical assessment |
| `RESEARCH-METHODOLOGY-v2.0.md` | Research and experimental practices |
| `CONTRIBUTING-v2.0.md` | Contributor responsibilities and development workflow |
| `CODE-OF-CONDUCT-v2.0.md` | Behavioural expectations and conduct procedures |

Where a specialist policy governs a specific subject, its detailed requirements apply.

Applicable laws, contractual obligations, third-party rights, and platform procedures remain controlling where relevant.

---

## 23. Closing Principle

Security is not a claim of absolute protection.

It is a continuous responsibility involving design, development, evaluation, maintenance, and responsible publication.

Framing Creativity Lab aims to identify meaningful weaknesses, reduce avoidable exposure, respond responsibly, and learn from the process.

**Build with care. Protect what matters. Disclose responsibly. Maintain with accountability.**

---

**Framing Creativity Lab**  
Independent Research · Applied AI · Creative Technology · Digital Systems

**Maintainer:** J-ART  
**Document:** `SECURITY-v2.0.md`\
**Version:** 2.0  
**Status:** Draft for Maintainer Review
