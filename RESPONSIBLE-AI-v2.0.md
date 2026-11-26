# Responsible AI Policy

**Document ID:** FCL-AI-001  
**Version:** 2.0  
**Status:** Draft for Maintainer Review  
**Effective Date:** Pending approval  
**Maintainer:** J-ART  
**Repository:** Framing Creativity Lab

---

## 1. Purpose

Framing Creativity Lab explores the intersection of artificial intelligence, creative technology, software engineering, digital experiences, and experimental research.

Artificial intelligence offers significant opportunities for exploration, automation, augmentation, and creative expression. It also introduces technical, ethical, legal, security, and societal risks that must be understood and managed.

This policy establishes the principles and requirements governing the research, development, use, evaluation, maintenance, and publication of AI-enabled technologies within the Lab.

Its objectives are to:

- Promote responsible and transparent use of artificial intelligence.
- Encourage meaningful human oversight and accountability.
- Protect personal, confidential, and proprietary information.
- Address risks associated with generative AI, machine learning, and autonomous systems.
- Establish expectations for model selection, evaluation, and documentation.
- Encourage appropriate, reliable, and contextually relevant AI applications.
- Protect intellectual property and respect third-party rights.
- Reduce the risk of harmful, deceptive, or unauthorized AI applications.
- Distinguish experimental capabilities from demonstrated and validated functionality.
- Support responsible publication of AI-related research and implementations.
- Preserve the independence and integrity of the Lab's research activities.

This policy applies both to AI used as a development tool and to systems that incorporate AI functionality.

**Technological capability does not automatically establish responsible use.**

---

## 2. Scope

This policy applies to artificial intelligence technologies used, investigated, developed, integrated, evaluated, or published within Framing Creativity Lab.

It covers, where relevant:

- Generative AI systems.
- Large Language Models (LLMs).
- Multimodal models.
- Image, audio, and video generation.
- Machine learning models.
- Predictive and classification systems.
- Retrieval-Augmented Generation (RAG).
- AI agents and agentic workflows.
- Automated decision-support systems.
- AI-powered interfaces and applications.
- Model APIs and external AI services.
- AI-assisted software development.
- AI-assisted research and documentation.
- AI-generated creative and technical content.
- Local and self-hosted AI systems.
- AI integrations with external tools and services.

The policy applies throughout the project lifecycle, including research, experimentation, development, evaluation, publication, and maintenance.

It applies whether an AI system is operated locally, hosted by a third party, integrated through an API, or accessed through an external platform.

### 2.1 AI as a Development and Research Tool

AI may support activities such as:

- Programming and code review.
- Research and knowledge exploration.
- Technical documentation.
- Design ideation.
- Creative development.
- Data analysis.
- Prototyping.
- Testing and debugging.
- Workflow assistance.
- Content transformation.
- Evaluation and experimentation.

Individuals remain responsible for verifying and reviewing material AI-assisted work.

### 2.2 AI as Part of a Developed System

AI may form part of the functionality of a project, application, or experimental system.

Examples include:

- Conversational interfaces.
- Generative applications.
- Recommendation systems.
- Retrieval and search systems.
- Autonomous agents.
- Automated analysis.
- Intelligent workflow orchestration.
- Multimodal interaction.
- Decision-support systems.
- AI-enabled creative environments.

These systems require additional assessment because their behavior may influence users, process information, access resources, or trigger actions.

### 2.3 Scope of Responsibility

The requirements of this policy apply to the AI-related activities that the Lab develops, controls, integrates, or publishes.

Use of an external provider does not remove the Lab's responsibility to assess whether that provider is appropriate for the intended project.

Likewise, using an AI system as an internal development tool does not authorize the disclosure of confidential information or remove the responsibility to verify its output.

---

## 3. Foundational Principles

The Lab adopts the following principles for responsible AI development and use.

### 3.1 Human Responsibility

AI systems may support reasoning, generate content, automate tasks, and assist with decisions.

They do not assume responsibility for the consequences of their use.

The individuals developing, operating, approving, or publishing an AI-enabled system remain responsible for the decisions and actions under their control.

### 3.2 Meaningful Human Oversight

Human oversight should be proportionate to the potential impact of an AI system.

The more consequential the result or action, the greater the need for meaningful human supervision.

A human approval mechanism must provide sufficient information and actual authority to intervene. A nominal confirmation step is not meaningful oversight if the person cannot understand, evaluate, or control the action.

### 3.3 Transparency

AI involvement should be communicated when it materially affects how a system operates, how content is produced, or how users should interpret its outputs.

Projects must not misrepresent generated content, model capabilities, or the degree of human involvement.

### 3.4 Fairness and Non-Discrimination

AI systems should be evaluated for foreseeable discriminatory or unfair outcomes where their intended use could affect people or groups.

The Lab should avoid systems that make unsupported assumptions about individuals or rely on inappropriate proxies for sensitive characteristics.

### 3.5 Privacy and Data Protection

AI systems should process only the information necessary for their intended purpose.

Personal, sensitive, confidential, and proprietary information must be handled according to applicable requirements and the Lab's confidentiality principles.

### 3.6 Reliability and Safety

AI-enabled systems should be evaluated against their intended use, known limitations, and potential consequences.

A plausible output is not necessarily an accurate output.

A successful demonstration is not proof of reliability.

### 3.7 Intellectual Integrity

AI-generated material must not be presented as verified research, original human work, or established fact without appropriate review and disclosure.

Sources, authorship, rights, and limitations must be respected.

### 3.8 Proportionality

Controls should reflect the system's capabilities, exposure, intended audience, and potential impact.

A private creative experiment does not necessarily require the same level of oversight as a public-facing AI agent with access to sensitive data or external systems.

### 3.9 Reversibility and Control

Where AI systems can perform actions or modify external resources, their design should consider the ability to stop, restrict, reverse, or recover from those actions.

The more autonomous or consequential a system becomes, the more important these controls are.

---

## 4. AI Risk Classification

AI projects must undergo a risk assessment appropriate to their functionality, intended use, operating context, and potential impact.

The following classification is an internal Framing Creativity Lab framework.

It is not a substitute for a legally defined risk classification, regulatory assessment, external certification, or professional risk evaluation.

### 4.1 Canonical Risk Levels

| Level | Classification | Description |
|---|---|---|
| A0 | Minimal Risk | Limited AI assistance with no meaningful impact on users, sensitive data, or external actions. |
| A1 | Low Risk | AI features with constrained functionality and limited foreseeable consequences. |
| A2 | Moderate Risk | Systems processing meaningful information or influencing user interactions and decisions. |
| A3 | High Risk | Systems with significant autonomy, privileged access, sensitive data, or potentially serious consequences. |
| A4 | Restricted Use | Systems or applications presenting unacceptable risks for the intended purpose or lacking essential safeguards. |

These five values are the canonical AI Risk Classification vocabulary owned by this document.

They must not be confused with:

- Lifecycle Stage.
- Project Status.
- Technical Maturity.
- Operational Readiness.
- Publication Classification.
- Publication Status.

AI Risk Classification and Publication Classification are independent assessments.

### 4.2 A0 — Minimal Risk

A0 applies to limited AI assistance or experiments with no meaningful impact on users, sensitive data, or external resources.

Examples may include:

- AI-assisted brainstorming.
- Exploratory prompt experiments.
- Local tests with non-sensitive inputs.
- Low-impact creative generation.
- Non-operational demonstrations.
- Minor AI-assisted content transformations.

Expected controls:

- Appropriate verification of outputs.
- Basic documentation of the experiment.
- No unauthorized confidential or personal data.
- No misrepresentation of results.
- Compliance with applicable tool and provider terms.

A0 does not mean that all possible risks are absent. It indicates that foreseeable consequences are limited within the declared scope.

### 4.3 A1 — Low Risk

A1 applies to AI features with constrained functionality and limited foreseeable consequences.

Examples may include:

- Non-consequential content generation.
- Limited text classification.
- Creative assistance tools.
- Public information summarization.
- Internal productivity experiments using authorized information.
- Non-critical workflow assistance.

Expected controls:

- Defined purpose.
- Documented model or service.
- Input and output review.
- Appropriate disclosure where relevant.
- Basic risk assessment.
- Documented limitations.
- Appropriate data handling.

### 4.4 A2 — Moderate Risk

A2 applies to systems processing meaningful information or influencing user interactions, recommendations, or decisions.

Examples may include:

- Public-facing conversational applications.
- RAG systems using structured information.
- AI-assisted recommendations.
- Systems processing user-submitted content.
- AI workflows connected to restricted application data.
- Applications whose outputs may influence user decisions.
- Automated content processing with material downstream consequences.

Expected controls:

- Documented use case and system boundaries.
- Data and privacy review.
- Access-control assessment.
- Model and output evaluation.
- Appropriate human oversight.
- Error and failure handling.
- Security testing.
- Clear user-facing limitations.
- Documented incident and maintenance considerations.
- Review of publication and distribution risks.

### 4.5 A3 — High Risk

A3 applies to systems with significant autonomy, privileged access, sensitive data, or potentially serious consequences.

Examples may include:

- Agents with access to external tools or operational systems.
- AI applications processing sensitive personal information.
- Systems capable of consequential decisions.
- Autonomous workflows capable of modifying important resources.
- Applications with privileged access to data or infrastructure.
- Systems that could create substantial harm if manipulated or misused.
- AI systems whose outputs directly influence important operational processes.

Expected controls:

- Explicit risk assessment.
- Documented architecture and permissions.
- Strong isolation and least-privilege access.
- Human authorization for consequential actions.
- Adversarial and abuse-case testing.
- Security and privacy review.
- Failure containment.
- Monitoring and auditability where appropriate.
- Defined response and recovery procedures.
- Explicit publication and deployment approval.
- Documented operational limitations.

A3 work requires particular caution. The maintainer must determine whether sufficient expertise, safeguards, and resources exist before the work is pursued or published.

### 4.6 A4 — Restricted Use

A4 applies to a proposed project or use case that presents unacceptable risks or cannot be operated with sufficient safeguards.

Potential reasons include:

- Deliberate facilitation of serious harm.
- Unauthorized access or surveillance.
- Unlawful manipulation or exploitation.
- Unjustifiable processing of highly sensitive information.
- Uncontrolled autonomous execution with serious potential consequences.
- Deceptive impersonation intended to cause harm.
- Harmful synthetic media.
- Circumvention of important security controls.
- Inability to establish legitimate data rights or appropriate safeguards.
- An application whose foreseeable consequences cannot be responsibly controlled.

A restricted classification means the proposed use must not be developed, operated, or published in that form.

A project may be reconsidered only if its purpose, scope, capabilities, or safeguards are materially changed and a new assessment establishes that the restrictions no longer apply.

### 4.7 Risk Reassessment

AI Risk Classification is not permanent.

It should be reviewed when:

- A model or provider changes.
- New data sources are introduced.
- System permissions increase.
- New tools or integrations are added.
- The system becomes publicly accessible.
- Intended users or use cases change.
- New failure modes are discovered.
- The system moves from experimentation to operational deployment.
- Autonomy or execution capabilities expand.
- New evidence changes the understanding of potential harm.

Risk classification should reflect the actual system, not only its original design.

### 4.8 Risk Classification and Publication

AI Risk Classification does not automatically determine Publication Classification.

A project classified A0 may still require P1 review because of external dependencies or data handling.

A project classified A3 may require substantial publication restrictions even when the underlying material has established ownership.

A4 indicates that the intended AI use is restricted. It does not become acceptable merely because publication material receives another classification.

The relationship between AI risk and publication eligibility must be assessed explicitly.

---

## 5. Permitted and Restricted AI Uses

### 5.1 Permitted Uses

Subject to applicable rights, project requirements, and appropriate safeguards, AI may be used for:

- Research and knowledge exploration.
- Creative ideation and experimentation.
- Software development assistance.
- Technical analysis.
- Documentation support.
- Prototyping and simulation.
- Content transformation.
- Data analysis using appropriately authorized data.
- Workflow assistance.
- Accessibility support.
- User-facing assistance.
- Evaluation and testing.
- Experimental autonomous workflows within controlled boundaries.
- Generative and computational creative studies.

The fact that a use is permitted in principle does not remove the need for a project-specific risk assessment.

### 5.2 Restricted or Prohibited Uses

The Lab must not knowingly develop, operate, or publish AI applications intended to:

- Facilitate serious unlawful activity or physical harm.
- Enable unauthorized access, credential theft, or malicious intrusion.
- Conduct covert surveillance without appropriate authorization.
- Exploit vulnerable individuals.
- Generate or distribute deceptive impersonations intended to cause harm.
- Create non-consensual intimate synthetic imagery.
- Circumvent access controls or security restrictions.
- Discriminate unlawfully or make unjustified determinations about individuals.
- Expose protected personal or confidential information.
- Execute consequential actions without appropriate authorization.
- Manipulate users through deceptive or coercive practices.
- Evade safeguards or restrictions intended to prevent serious harm.

These restrictions apply to the intended functionality and foreseeable use of a project, not merely to the label attached to it.

### 5.3 Dual-Use Research

Some technologies may have both beneficial and harmful applications.

When a project has credible dual-use implications, the maintainer should assess:

- Intended purpose.
- Available safeguards.
- Potential misuse pathways.
- Accessibility of dangerous functionality.
- Potential scale of harm.
- Reversibility of resulting actions.
- Whether publication would materially increase misuse risk.

Sensitive implementation details or operational instructions may need to remain unpublished, be restricted, or be omitted entirely.

The Lab's commitment to research openness does not require publishing material that creates disproportionate risks.

### 5.4 Reassessment of Restricted Proposals

A restricted proposal may be reconsidered when meaningful changes are made to its purpose, scope, access model, data, capabilities, or safeguards.

A new assessment must document the changes and establish whether the original reasons for restriction have been adequately addressed.

A change of terminology alone is not sufficient.

---

## 6. Data Governance and Privacy

Data handling is one of the most significant responsibilities in AI development.

Models and external services may process, retain, transform, or transmit information beyond the immediate application context.

The Lab therefore requires deliberate data management.

### 6.1 Canonical Data Classification

Before using data in an AI workflow, its classification and permitted use must be understood.

The Lab uses the following four canonical data classification levels:

| Classification | Description | General treatment |
|---|---|---|
| Public | Information explicitly approved or otherwise authorized for public distribution. | May be used subject to source rights and applicable restrictions. |
| Internal | Non-public working information intended for authorized Lab use. | Use only in approved environments; do not submit to external services without appropriate authorization. |
| Confidential | Information subject to confidentiality obligations, restricted access, or material disclosure risk. | Restricted access; external processing requires explicit authorization and an appropriate basis. |
| Restricted | Highly sensitive, legally or contractually restricted, security-critical, or otherwise unsuitable for ordinary disclosure. | Do not submit to external AI services without an explicitly established basis, authorization, and appropriate safeguards. |

These four values are the Lab's canonical data classification vocabulary.

They must remain consistent with `PUBLICATION-POLICY-v2.0.md`.

Personal information and sensitive information are characteristics of data, not additional values in the four-level classification vocabulary.

### 6.2 Data Minimization

AI workflows should use only the information necessary to perform the intended task.

Avoid:

- Uploading entire datasets when a small subset is sufficient.
- Including unnecessary personal information in prompts.
- Embedding credentials in model context.
- Retaining raw inputs without a justified purpose.
- Sending information to unrelated services.
- Reproducing complete documents when only a limited extract is required.
- Keeping unnecessary intermediate outputs containing sensitive information.

### 6.3 Personal Data

Personal data should be processed only when there is an appropriate purpose and a valid basis for doing so.

Where relevant, projects should consider:

- Transparency.
- Purpose limitation.
- Data minimization.
- Accuracy.
- Storage limitation.
- Security.
- Access and deletion rights.
- Third-party processors.
- Cross-border data transfers.
- Applicable contractual and legal requirements.

Personal information should be classified at least as Confidential under the Lab's internal data classification framework.

Sensitive personal information or information subject to stricter restrictions should be classified as Restricted.

Legal requirements depend on the data, parties, locations, and actual processing activity.

The Lab must not claim compliance with a specific privacy regime solely because general privacy principles have been considered.

### 6.4 Sensitive Information

Sensitive information must not be submitted to AI tools merely because a provider offers a convenient interface.

Before external processing, the responsible person must assess:

- Whether the data may legally be processed.
- Whether the service is authorized for that purpose.
- Whether inputs or outputs may be retained.
- Whether submitted data may be used for model improvement or training.
- Who may access the information.
- Where processing takes place.
- Whether appropriate contractual and technical safeguards exist.
- Whether the information can be minimized or transformed before submission.

When these conditions cannot be established, the information must not be submitted.

### 6.5 Confidential Project Separation

The public Lab must remain independent from private, proprietary, and confidential work.

AI tools must not be used to transfer confidential material into public experiments, examples, prompts, datasets, documentation, or demonstrations without explicit authorization.

This includes:

- Source code.
- Business information.
- Private architecture.
- Internal workflows.
- Private assets.
- Restricted project documentation.
- Client or user information.
- Non-public prompts and system configurations.

Public experiments must be suitable for publication independently of any confidential work that may exist elsewhere.

### 6.6 Data Retention

Projects should avoid retaining prompts, input data, model outputs, or logs longer than necessary for their intended purpose.

Where information is retained, the project should document, as appropriate:

- What is retained.
- Why it is retained.
- Where it is stored.
- Who can access it.
- How long it is retained.
- How deletion is performed.
- Whether external providers retain independent copies.

The Lab must not promise deletion from external systems unless the relevant capability and provider conditions have been verified.

---

## 7. Model and Provider Selection

AI models and services should be selected according to the needs and risk profile of the project.

### 7.1 Selection Criteria

Where relevant, model selection should consider:

- Functional capabilities.
- Accuracy and reliability.
- Model limitations.
- Performance and latency.
- Cost and resource consumption.
- Context and input limitations.
- Provider security practices.
- Data retention and processing policies.
- Licensing and usage conditions.
- Model availability and maintenance.
- Provider transparency.
- Portability and dependency risk.
- Accessibility and language support.
- Suitability for the intended task.

The most capable model is not necessarily the most appropriate choice.

Selection should be based on suitability rather than popularity, benchmark performance, or novelty alone.

### 7.2 Provider Assessment

Before using an external AI service, the project should consider:

- Who operates the service?
- What information is transmitted?
- How are inputs and outputs handled?
- Are interactions retained?
- Can submitted information be used for training or service improvement?
- Are data deletion mechanisms available?
- Where is data processed?
- What contractual or licensing conditions apply?
- What access permissions are required?
- What happens if the service changes or becomes unavailable?

Provider documentation and terms should be reviewed when relevant.

Assumptions about provider data handling must not be treated as verified facts.

### 7.3 Model and Provider Changes

Changes to model versions or service behavior can affect:

- Output quality.
- Reliability.
- Safety behavior.
- Latency.
- Cost.
- Data processing.
- Reproducibility.
- Compatibility with existing prompts and tools.

Material changes should be evaluated before they are adopted in a project that depends on the affected behavior.

### 7.4 Open-Weight and Local Models

Models operated locally or through self-hosted infrastructure may provide greater control over the execution environment.

They do not automatically eliminate:

- Licensing restrictions.
- Security vulnerabilities.
- Data leakage risks.
- Model limitations.
- Misuse potential.
- Infrastructure and operational risks.
- Uncontrolled access to local resources.

The same responsibility and evaluation principles apply.

### 7.5 Provider Dependency

Projects should avoid unnecessary dependence on a single provider when that dependency creates a material continuity or operational risk.

Where appropriate, document:

- The provider-specific functionality.
- The impact of service interruption.
- Available alternatives.
- Migration constraints.
- Data portability limitations.
- The cost of changing providers.

---

## 8. Prompt, Context, and Instruction Management

Prompts and contextual instructions are part of an AI system's behavior.

They should be designed and managed with appropriate care.

### 8.1 Prompt Quality

Where relevant, prompts should:

- Define the intended task.
- Establish clear boundaries.
- Provide appropriate context.
- Identify output expectations.
- Communicate uncertainty requirements.
- Distinguish trusted information from untrusted input.
- Avoid unnecessary sensitive information.
- Avoid unsupported assumptions about the user's identity or intentions.
- Define how missing information should be handled.

### 8.2 Instruction Boundaries

Systems should not assume that user content, retrieved documents, external webpages, or uploaded files are trusted instructions.

Where prompt injection or instruction confusion is relevant, the system should separate:

- System-level instructions.
- Developer-defined behavior.
- Authorized user instructions.
- Retrieved information.
- Untrusted external content.
- Model-generated output.
- Tool results.

Untrusted content must not be allowed to override security boundaries or authorize actions independently.

### 8.3 Prompt Versioning

Important prompts and instruction sets should be versioned or documented when their behavior materially affects the system.

Relevant records may include:

- Prompt identifier.
- Version.
- Intended purpose.
- Model compatibility.
- Important configuration.
- Evaluation results.
- Known limitations.
- Revision date.

Sensitive instructions or confidential context must not be placed in public documentation without authorization.

### 8.4 Prompt Injection and Adversarial Inputs

Applications should consider malicious or unexpected inputs that attempt to:

- Override system instructions.
- Extract protected information.
- Modify agent behavior.
- Trigger unauthorized tools.
- Circumvent access controls.
- Manipulate retrieval or reasoning context.
- Cause unintended external actions.

Mitigation must rely on application-level boundaries and authorization, not solely on prompt wording.

### 8.5 Untrusted Retrieved Material

Documents and information retrieved from external sources should be treated as data, not as automatically authorized instructions.

Where relevant, systems should:

- Preserve source context.
- Enforce access permissions outside the model.
- Avoid mixing restricted information into unauthorized contexts.
- Validate retrieved content.
- Record relevant source references.
- Prevent retrieved instructions from authorizing tool use independently.

---

## 9. Human Oversight and Decision Authority

Human oversight should be meaningful and proportionate to the consequences of an AI system's behavior.

### 9.1 Human-in-the-Loop

Human review may be appropriate when:

- Outputs influence important decisions.
- Personal or sensitive data is involved.
- Results may have legal, financial, or safety consequences.
- The model may make uncertain or consequential classifications.
- The system can publish or distribute content.
- An agent can modify external resources.
- The model can initiate irreversible actions.
- Errors could materially affect a person or organization.

### 9.2 Human-on-the-Loop

Some systems may operate continuously with human monitoring rather than requiring approval for every operation.

This approach is only appropriate where:

- The scope of autonomy is constrained.
- Monitoring is meaningful.
- The system has safe failure behavior.
- Intervention is possible.
- Consequential actions have appropriate safeguards.
- Operators understand the limits of their supervision.

### 9.3 Human-in-Control

The maintainer or authorized operator must retain control over:

- System permissions.
- Tool access.
- Sensitive integrations.
- Deployment.
- Significant policy changes.
- High-impact actions.
- Suspension or shutdown.
- External publication.
- Changes to the system's autonomy.

### 9.4 Accountability

A system must have an identifiable responsible operator or maintainer.

AI-generated decisions and actions must not be treated as unowned events for which no human or organization is accountable.

### 9.5 Effective Oversight

Oversight must provide sufficient information and authority for a person to intervene meaningfully.

Where relevant, the operator should be able to:

- Understand the action proposed by the system.
- Examine the information supporting it.
- Identify uncertainty or limitations.
- Approve, reject, or modify the action.
- Stop execution.
- Escalate an issue.
- Record the decision where appropriate.

A person should not be required to approve actions blindly.

---

## 10. AI Agents and Autonomous Systems

AI agents and agentic workflows require particular attention because they may interpret instructions, invoke tools, access information, and perform actions through connected services.

Their autonomy must be deliberately constrained.

### 10.1 Least Privilege

Agents should receive only the minimum permissions necessary for their intended task.

Avoid:

- Unrestricted file-system access.
- Broad administrative credentials.
- Unnecessary database permissions.
- Unrestricted network access.
- Persistent access to unrelated resources.
- Unrestricted execution of system commands.
- Access to unrelated repositories or projects.
- Access to confidential data outside the defined task.

### 10.2 Tool Authorization

Tools should enforce their own permissions and validation.

An AI model's request to invoke a tool must not itself establish authorization.

Applications should independently verify:

- User permissions.
- Tool permissions.
- Resource ownership.
- Allowed operations.
- Input validity.
- Expected side effects.
- Relevant approval requirements.

### 10.3 Consequential Actions

Human confirmation should be required where appropriate before an agent:

- Deletes or overwrites important information.
- Publishes external content.
- Sends communications on behalf of a user.
- Modifies access permissions.
- Executes financial or contractual operations.
- Changes infrastructure.
- Performs irreversible actions.
- Accesses or transfers sensitive information.
- Modifies production systems.
- Creates external commitments.

The required level of confirmation should reflect the consequences and reversibility of the operation.

### 10.4 Execution Isolation

Where agents execute code or interact with files and infrastructure, appropriate isolation should be considered.

Possible controls include:

- Sandboxed execution.
- Restricted file access.
- Network restrictions.
- Resource limits.
- Temporary credentials.
- Timeouts.
- Explicit permission boundaries.
- Execution logging.
- Controlled working directories.
- Separate development and production environments.

### 10.5 Agent Failure and Recovery

Agent-based systems should account for:

- Repeated tool calls.
- Unexpected action sequences.
- Infinite loops.
- Incorrect assumptions.
- Conflicting instructions.
- Partial execution.
- Duplicate operations.
- External service failure.
- Unexpected changes to files or resources.
- Unintended escalation of permissions.

Where relevant, the system should provide execution limits, stop mechanisms, rollback options, and recovery procedures.

### 10.6 No Delegation of Accountability

An agent must not be treated as an independent authority that can assume responsibility for the consequences of its actions.

The operator and responsible maintainer remain accountable for the system's design, permissions, and deployment.

---

## 11. AI Output Quality and Reliability

AI outputs should be evaluated in relation to their intended use.

A response that appears coherent or convincing may still be inaccurate, incomplete, biased, or misleading.

### 11.1 Verification

Where factual accuracy matters, relevant outputs should be verified against appropriate sources.

This may include:

- Independent source checking.
- Cross-validation.
- Structured test cases.
- Human review.
- Domain-specific evaluation.
- Comparison with trusted reference data.
- Verification of calculations or structured outputs.
- Examination of relevant source documents.

The method should reflect the importance of the claim or action.

### 11.2 Hallucinations

Projects should identify where a model may generate unsupported information.

Depending on the use case, appropriate controls may include:

- Source grounding.
- Retrieval-based verification.
- Confidence or uncertainty communication.
- Human review.
- Restricted answer formats.
- Explicit refusal when evidence is insufficient.
- Separation of verified facts from generated interpretation.

The Lab recognizes that model confidence and linguistic fluency do not establish factual correctness.

### 11.3 Output Validation

Generated outputs should be validated before they are:

- Executed.
- Published.
- Stored as authoritative information.
- Used to modify important resources.
- Transmitted to external systems.
- Used as input to other automated processes.
- Used to make consequential decisions.

The required validation depends on the potential impact.

### 11.4 Automated Decisions

Where an AI system influences a decision about an individual, the project should assess:

- The legitimacy of the use case.
- The accuracy and limitations of the model.
- The consequences of errors.
- Potential discrimination.
- The possibility of human review.
- Appropriate transparency and contestability.
- Whether the decision should be automated at all.

High-impact uses require particular caution and may be inappropriate for the Lab.

### 11.5 Output Integrity

AI-generated material should not be treated as authoritative solely because it is structured, detailed, or presented confidently.

Projects should distinguish:

- Model-generated content.
- Retrieved source material.
- Human-verified information.
- Human interpretation.
- Automated actions.
- Unresolved uncertainty.

### 11.6 Output Persistence

Where outputs are stored or reused, projects should consider whether they may become outdated, be mistaken for verified information, or influence later decisions.

Important generated records should retain sufficient context to understand their origin and verification state where practical.

---

## 12. Fairness, Bias, and Representation

AI systems may reproduce or amplify limitations and biases present in their training data, evaluation processes, or operating context.

### 12.1 Potential Sources of Bias

Relevant sources may include:

- Historical training data.
- Underrepresented populations.
- Incomplete datasets.
- Proxy variables.
- Subjective labeling.
- Evaluation bias.
- Model design choices.
- Contextual assumptions.
- Language and cultural limitations.
- Unequal access to relevant data.
- User-interface choices.

### 12.2 Evaluation

Where a system may materially affect people or groups, its behavior should be evaluated for foreseeable unfair or discriminatory outcomes.

Evaluation should consider the intended population and context.

A model performing well on one benchmark or population does not establish fairness in every context.

### 12.3 Representation

Creative and generative systems should also consider how they represent people, cultures, identities, and communities.

The Lab should avoid presenting generated stereotypes or unsupported representations as authoritative or culturally representative.

### 12.4 Limitations

The Lab recognizes that fairness is context-dependent and cannot be established by a single universal metric.

Where meaningful fairness evaluation is not possible, that limitation should be documented.

### 12.5 High-Impact Contexts

AI systems that influence access to services, opportunities, employment, financial resources, education, healthcare, or other important outcomes require particular caution.

The Lab must not assume that a general-purpose model is appropriate for these contexts without sufficient domain expertise, safeguards, and evaluation.

Where the required expertise or controls are unavailable, the project should be restricted, redesigned, or not pursued.

---

## 13. Intellectual Property, Authorship, and AI-Generated Material

AI-generated material raises questions concerning authorship, ownership, attribution, licensing, and permitted use.

These questions must be considered before publication or distribution.

### 13.1 Human Responsibility for AI-Assisted Work

Individuals using AI-generated or AI-assisted material remain responsible for reviewing it before submission or publication.

This includes:

- Code.
- Documentation.
- Research summaries.
- Images.
- Audio.
- Video.
- Written content.
- Design assets.
- Data transformations.
- Technical configurations.
- Generated examples.
- Model-generated instructions.

The use of AI does not remove the obligation to verify rights, accuracy, and suitability.

### 13.2 No Assumption of Rights-Free Output

AI-generated content must not automatically be considered free of copyright, third-party rights, or licensing restrictions.

Before publication, relevant questions include:

- Does the output reproduce protected material?
- Are the model or platform terms compatible with the intended use?
- Are input materials properly authorized?
- Are third-party assets incorporated?
- Are attribution requirements applicable?
- Are there restrictions on commercial or public distribution?
- Are there contractual restrictions on generated outputs?
- Has the material been sufficiently reviewed?

Unclear rights should be resolved before release.

### 13.3 AI-Assisted Code

AI-generated code must be reviewed for:

- Correctness.
- Security.
- Maintainability.
- Dependencies.
- Licensing implications.
- Hidden assumptions.
- Potential reproduction of third-party code.
- Compatibility with the project architecture.
- Unintended side effects.

Generated code should not be accepted solely because it compiles or passes a demonstration.

### 13.4 Authorship and Attribution

Contributions should be attributed accurately.

AI tools must not be listed as human authors, project owners, or accountable decision-makers.

Where AI materially contributed to research, implementation, or published content, the nature of that assistance should be disclosed where appropriate.

Routine assistance, such as minor grammar corrections, does not necessarily require a separate disclosure unless a project defines otherwise.

### 13.5 Third-Party Rights

The Lab must respect the rights and licence conditions associated with:

- Training datasets.
- Reference images.
- Source code.
- Textual material.
- Music and audio.
- Video.
- Model weights.
- Generated assets.
- External libraries.
- Provider services.
- User-submitted content.

A model's ability to process or generate material does not establish that the underlying use is authorized.

### 13.6 Confidential Material

AI systems must not be used to transfer proprietary or confidential material into public projects or demonstrations without explicit authorization.

This applies to both inputs and outputs. A generated summary or transformed extract may still reveal protected information.

---

## 14. Transparency and Disclosure

AI involvement should be communicated when it materially affects a project, a user interaction, or the interpretation of published results.

### 14.1 User-Facing Transparency

Where relevant, users should be able to understand:

- Whether they are interacting with an AI system.
- What role AI performs.
- What information may be processed.
- Whether outputs are generated or automatically derived.
- Whether a human reviews important results.
- What important limitations apply.
- Whether an external provider is involved.
- What actions the system can perform.

Disclosure should be clear and meaningful rather than hidden in technical documentation.

### 14.2 Research Disclosure

Research documentation should identify material AI involvement.

Relevant details may include:

- Model and provider.
- Version or model identifier.
- Experimental configuration.
- Relevant prompts or instruction sets.
- Data sources.
- Human review procedures.
- Evaluation methods.
- Important limitations.
- Relevant external dependencies.

### 14.3 AI-Assisted Contributions

Contributors should disclose substantial AI assistance when it materially affects the contribution or where a project explicitly requires disclosure.

This is particularly important for:

- Generated code.
- Research conclusions.
- Substantial documentation.
- Creative assets.
- Data analysis.
- Technical configurations.
- Model-generated content included in public deliverables.

Routine assistance does not necessarily require a separate disclosure unless a project specifies otherwise.

### 14.4 Avoiding Misrepresentation

The Lab must not present:

- Synthetic content as authentic documentary evidence.
- Generated research results as independently verified findings.
- AI-generated testimonials as genuine human experiences.
- Simulated capabilities as operational functionality.
- Model outputs as expert conclusions without appropriate validation.
- Automated actions as human-reviewed actions when no such review occurred.

### 14.5 Disclosure Proportionality

Disclosure should be sufficient for the intended audience to understand the role of AI.

It need not reveal confidential prompts, proprietary configurations, credentials, or protected implementation details.

Transparency must remain compatible with intellectual property, security, privacy, and publication restrictions.

---

## 15. Evaluation and Testing of AI Systems

AI systems require evaluation beyond conventional software testing.

Their behavior may vary across prompts, users, datasets, model versions, and operating conditions.

### 15.1 Evaluation Objectives

Before testing, projects should identify:

- Intended functionality.
- Expected behavior.
- Relevant failure conditions.
- Evaluation criteria.
- Test inputs and datasets.
- Performance expectations.
- Known limitations.
- Acceptable risk boundaries.
- Human review requirements.
- Relevant security and privacy considerations.

### 15.2 Evaluation Dimensions

Depending on the application, evaluation may include:

| Dimension | Evaluation focus |
|---|---|
| Accuracy | Correctness of outputs |
| Relevance | Alignment with the requested task |
| Consistency | Stability across comparable inputs |
| Robustness | Behavior under unusual or adversarial inputs |
| Safety | Risk of harmful or inappropriate outputs |
| Privacy | Protection against unintended data exposure |
| Instruction Adherence | Compliance with intended system boundaries |
| Reliability | Predictability under expected operating conditions |
| Latency | Response time |
| Cost Efficiency | Resource consumption relative to value |
| Human Usability | Clarity and usefulness for the intended audience |
| Fairness | Potential unequal or discriminatory outcomes where relevant |

### 15.3 Testing Scenarios

Where relevant, evaluation should include:

- Typical inputs.
- Edge cases.
- Invalid inputs.
- Ambiguous requests.
- Adversarial inputs.
- Unexpected context.
- External service failures.
- Model refusal behavior.
- Tool execution boundaries.
- Sensitive data exposure attempts.
- Malformed or malicious retrieved content.
- Unexpected model output formats.

### 15.4 Evaluation Records

Meaningful evaluations should record:

- Model and version.
- Configuration.
- Relevant test inputs.
- Evaluation procedure.
- Test environment.
- Observed results.
- Limitations.
- Known failure modes.
- Date of evaluation.
- Relevant changes since the previous evaluation.

Sensitive prompts, confidential information, and restricted datasets must not be included in public records without authorization.

### 15.5 Benchmark Limitations

Benchmark results should be interpreted in context.

A model's benchmark score does not establish that it is suitable for a specific application.

Evaluation should reflect the actual task, operating environment, user population, and consequences of failure.

### 15.6 Evaluation Against Intended Use

The evaluation criteria must reflect what the system is intended to do.

A conversational model used for creative assistance should not automatically be assessed using the same criteria as an information-retrieval application or a system that performs external actions.

The evaluation must be meaningful for the actual use case.

---

## 16. Reproducibility and Experimental Records

AI research often involves variables that make exact reproduction difficult.

These may include model updates, changing provider behavior, nondeterministic inference, and differences in runtime configuration.

### 16.1 Documentation

Where possible, experiments should document:

- Model identifier.
- Provider.
- Model version.
- Prompt version.
- Relevant parameters.
- Sampling or generation settings.
- Retrieval configuration.
- Dataset characteristics.
- Tool integrations.
- Test environment.
- Evaluation date.
- Relevant external conditions.

### 16.2 Reproducibility Limits

Where exact reproduction cannot be guaranteed, the project should state which conditions are uncontrolled.

For example:

- The provider may update the model without preserving the previous version.
- Outputs may vary even under nominally identical settings.
- External retrieval results may change.
- Service behavior may depend on hidden provider-side configurations.
- Sampling or generation processes may be nondeterministic.
- External data may change after the original experiment.

### 16.3 Research Integrity

Experimental findings must not be selectively reported to create a misleading impression of performance.

Failed tests, relevant anomalies, and important limitations should be documented where they materially affect the conclusions.

### 16.4 Reproduction and Protected Material

Reproducibility does not authorize the publication of confidential prompts, restricted datasets, proprietary code, or protected provider information.

Where an experiment cannot be reproduced publicly in full, document the limitation and provide the information that can legitimately be shared.

---

## 17. Creative AI and Human Expression

Framing Creativity Lab recognizes creative experimentation as a legitimate area of AI research and development.

AI may be used as:

- A creative instrument.
- A generative medium.
- A collaborative assistant.
- A transformation tool.
- A source of alternative perspectives.
- A system for exploring interaction and perception.
- A component of audiovisual or multimodal experiences.
- A means of investigating computational creativity.

### 17.1 Human Creative Direction

The Lab encourages clear creative intent and human judgment in AI-assisted work.

The use of generative tools should not erase responsibility for the selection, transformation, interpretation, and presentation of the resulting material.

### 17.2 Creative Attribution

Where relevant, documentation should distinguish between:

- Human-created material.
- AI-generated material.
- AI-assisted transformations.
- Third-party source material.
- Human-edited or curated outputs.

The exact level of attribution depends on the project and applicable rights.

### 17.3 Authenticity and Representation

Projects must not knowingly misrepresent synthetic images, audio, video, or text as genuine recordings or documentary evidence where that distinction materially affects interpretation.

Synthetic media involving identifiable people requires particular care, including consideration of consent, privacy, attribution, and potential harm.

### 17.4 Creative Experimentation

Creative freedom does not exempt a project from security, privacy, intellectual property, or publication requirements.

Experiments should remain within the Lab's general responsibility framework.

### 17.5 Creative Evaluation

Creative AI outcomes may require qualitative evaluation rather than exclusively numerical metrics.

Relevant dimensions may include:

- Expressive intention.
- Coherence.
- Originality within the declared scope.
- Interaction quality.
- Perceptual effect.
- Consistency with the intended creative direction.
- Human interpretation and curation.

Creative assessments should distinguish subjective judgment from objectively measured technical behavior.

---

## 18. Security of AI-Enabled Systems

AI applications introduce attack surfaces that may differ from conventional software systems.

Relevant risks may include:

- Prompt injection.
- Data exfiltration.
- Retrieval access-control failures.
- Unauthorized tool execution.
- Model manipulation.
- Insecure output handling.
- Credential exposure.
- Malicious file content.
- Untrusted generated code.
- Agent privilege escalation.
- Denial of service through excessive inference or tool usage.
- Unsafe handling of external content.
- Unauthorized access through connected services.

### 18.1 Application-Level Controls

Security boundaries must be enforced outside the model.

Examples include:

- Server-side authorization.
- Strict input validation.
- Output validation.
- Restricted tool interfaces.
- Secure secret management.
- Isolated execution environments.
- Resource limits.
- Network restrictions.
- Appropriate logging.
- Rate limiting.
- Explicit action permissions.
- Restricted data access.

### 18.2 Retrieval and Knowledge Systems

RAG and other retrieval-based applications should enforce authorization before information is provided to the model.

The system must not rely on the model to independently determine whether a user is allowed to access a document.

Document-level permissions, user identity, and retrieval boundaries should be enforced by the application.

### 18.3 Generated Code and Commands

Model-generated code, scripts, queries, and commands must be treated as untrusted until reviewed and validated.

They must not be executed in privileged environments without appropriate controls.

### 18.4 Tool and Integration Security

AI tools must enforce independent permission checks.

An instruction generated by a model must not be sufficient to:

- Bypass authentication.
- Increase privileges.
- Access unrelated resources.
- Publish restricted information.
- Perform unauthorized external actions.

### 18.5 Security Incidents

AI-related security vulnerabilities should be managed according to `SECURITY-v2.0.md`.

Potential confidentiality or publication consequences must also be assessed under `PUBLICATION-POLICY-v2.0.md`.

---

## 19. Monitoring, Maintenance, and Incident Management

AI systems may change behavior over time due to new models, updated providers, changing data, or evolving usage patterns.

Projects with ongoing operation should consider how material changes and incidents are detected.

### 19.1 Monitoring

Where appropriate, monitoring may include:

- Error rates.
- Output quality.
- Latency.
- Resource consumption.
- Unexpected tool activity.
- Policy violations.
- Access-control failures.
- Model or provider changes.
- User feedback.
- Unusual usage patterns.
- Repeated failed operations.
- Unintended data exposure.

Monitoring must respect privacy, data minimization, and confidentiality principles.

### 19.2 Model Changes

Material model or provider updates may require:

- Regression testing.
- Output comparison.
- Security reassessment.
- Performance reassessment.
- Prompt or workflow adjustments.
- Documentation updates.
- Reassessment of the AI Risk Classification.

A provider's change to model behavior should not automatically be assumed to preserve the original evaluation results.

### 19.3 AI Incidents

An AI-related incident may include:

- Unintended disclosure of protected information.
- Harmful or materially misleading output.
- Unauthorized agent actions.
- Incorrect access to restricted information.
- Security boundary failures.
- Significant model misuse.
- Uncontrolled resource consumption.
- A failure affecting an important workflow.
- Unauthorized publication or distribution.
- Materially incorrect automated decisions.

### 19.4 Incident Response

Depending on severity, a response may involve:

1. Restricting or disabling the affected functionality.
2. Preventing further unauthorized access or actions.
3. Protecting affected data and systems.
4. Identifying the source and scope of the incident.
5. Assessing potential impact.
6. Correcting the underlying weakness.
7. Testing the remediation.
8. Reassessing project risk and permissions.
9. Documenting the incident and relevant lessons.
10. Communicating material information where appropriate.

The appropriate response depends on the incident and applicable obligations.

### 19.5 Suspension

The maintainer may suspend or withdraw an AI-enabled project when its operation presents an unacceptable risk.

The ability to pause, disable, or restrict a system should be considered during design where the system has meaningful operational impact.

### 19.6 Post-Incident Reassessment

Following a material incident, the project should be reassessed before affected functionality is restored.

The reassessment should consider:

- Whether the original risk classification remains appropriate.
- Whether the relevant safeguards are effective.
- Whether permissions need to be reduced.
- Whether the architecture needs modification.
- Whether additional testing is required.
- Whether publication approval or operational conditions are affected.

---

## 20. Third-Party AI Services and External Integrations

External AI providers introduce dependencies outside the direct control of the Lab.

Projects should consider:

- Provider availability.
- API changes.
- Model retirement.
- Service pricing.
- Data handling.
- Usage restrictions.
- Licensing.
- Geographic processing.
- Security practices.
- Terms of service.
- Long-term dependency risk.
- Provider-specific limitations.

### 20.1 Provider Responsibility

The Lab does not control the internal operation of third-party models or platforms.

Provider behavior should not be represented as a guarantee made by Framing Creativity Lab.

### 20.2 Service Failure

Projects should consider what happens when an external AI service becomes unavailable, changes its behavior, or returns unexpected outputs.

Where appropriate, the application should provide:

- Clear failure communication.
- Safe fallback behavior.
- Retry limits.
- Appropriate timeouts.
- The ability to disable the integration.
- A defined response to partial execution.

### 20.3 Provider Claims

Claims about model capabilities, privacy, data retention, security, or performance should be based on relevant provider documentation or independently available evidence.

Unverified provider claims must not be presented as established facts.

### 20.4 External Processing

Before sending data to an external AI provider, the responsible person must assess the data classification, purpose, authorization, provider terms, and applicable safeguards.

Internal, Confidential, and Restricted information must not be transmitted merely because an API permits it technically.

### 20.5 Provider Changes and Portability

Material provider changes may trigger a new technical, security, privacy, or publication review.

Where practical, projects should document provider-specific dependencies and consider the consequences of changing or discontinuing the service.

---

## 21. Environmental and Resource Considerations

AI systems may require substantial computational resources.

The Lab encourages awareness of the resource implications of model selection, inference, training, and deployment.

Where relevant, projects should consider:

- Model size.
- Inference frequency.
- Computational requirements.
- Energy consumption.
- Storage requirements.
- Network usage.
- API costs.
- Redundant processing.
- Opportunities for smaller or more efficient models.
- The proportionality of resource consumption to the value of the result.

Resource efficiency should be evaluated in relation to the quality and usefulness of the result.

The Lab does not require a formal environmental impact assessment for every small experiment.

However, material resource implications should be considered for large-scale or continuously operating systems.

### 21.1 Cost and Resource Limits

Projects using paid services or computationally expensive models should consider appropriate usage limits.

Where relevant, this may include:

- Request quotas.
- Rate limits.
- Execution limits.
- Budget thresholds.
- Alerts.
- Model selection rules.
- Restrictions on repeated generation.
- Controls against unbounded agent execution.

Resource consumption should not be allowed to grow without a reasonable understanding of the resulting cost and operational consequences.

---

## 22. Documentation Requirements for AI Projects

AI-enabled projects should document their behavior and limitations sufficiently for others to understand and evaluate them.

The documentation level should remain proportionate to the project's risk, complexity, maturity, and intended use.

### 22.1 Project Information

Where relevant, document:

- Project purpose.
- Intended users.
- Intended use cases.
- Out-of-scope uses.
- AI functionality.
- Current Project Status.
- Lifecycle Stage.
- Technical Maturity.
- Operational Readiness.
- AI Risk Classification.
- Publication Classification and Publication Status.

The six canonical project fields must follow their respective authoritative documents. AI Risk Classification remains separate.

### 22.2 Model Information

Where relevant, document:

- Model name.
- Provider or source.
- Version or identifier.
- Relevant configuration.
- Important limitations.
- Date of evaluation.
- Model update or versioning assumptions.

### 22.3 Data Information

Where relevant, document:

- Data sources.
- Data classification.
- Processing purpose.
- Retention considerations.
- External processing dependencies.
- Data-use restrictions.
- Relevant authorization.
- Personal or sensitive information considerations.

### 22.4 System Information

Where relevant, document:

- Architecture.
- Retrieval components.
- Tool integrations.
- Permission boundaries.
- Human oversight mechanisms.
- External dependencies.
- Execution isolation.
- Relevant failure and recovery behavior.

### 22.5 Evaluation Information

Where relevant, document:

- Testing approach.
- Evaluation criteria.
- Test conditions.
- Results.
- Known failure modes.
- Limitations.
- Reproducibility constraints.
- Risk reassessment.

### 22.6 User Information

Where relevant, document:

- AI disclosure.
- Expected behavior.
- Important limitations.
- Privacy information.
- Human review conditions.
- Available support or reporting channels.
- Actions the system can perform.
- Relevant restrictions.

Not every project requires a separate technical dossier.

The documentation level should remain proportionate to the project's purpose and risks.

### 22.7 Public Documentation Boundary

Public documentation must not expose:

- Confidential prompts.
- Private instructions.
- Credentials.
- Restricted datasets.
- Proprietary architecture.
- Sensitive model configurations.
- Internal provider information.
- Unauthorised source material.

Where a full technical description is restricted, use a safe abstraction or state the limitation.

---

## 23. Roles and Responsibilities

Responsibilities follow the Lab's founder-led governance model as defined in `GOVERNANCE-v2.0.md`.

### 23.1 Founder and Maintainer

The Founder and Maintainer is responsible for:

- Approving AI-related projects and public releases.
- Reviewing relevant risk assessments.
- Establishing appropriate project boundaries.
- Ensuring that data and licensing concerns are considered.
- Assessing significant security and privacy risks.
- Reviewing material AI claims.
- Ensuring appropriate documentation.
- Determining whether an AI application may be published or should be restricted.
- Suspending or withdrawing projects where necessary.
- Reviewing material changes to AI capabilities or permissions.

### 23.2 Contributors

Contributors are expected to:

- Use AI systems responsibly.
- Verify material AI-generated outputs.
- Protect confidential and personal information.
- Respect intellectual property.
- Document material AI assistance where appropriate.
- Avoid unauthorized automated actions.
- Identify and report significant risks.
- Follow project-specific AI requirements.
- Disclose material limitations in work they submit.

AI-assisted development does not transfer responsibility for submitted work to the model or provider.

### 23.3 Collaborators

Collaborators must respect the agreed scope of AI-related activities.

They must not submit restricted data, introduce unapproved integrations, or publish AI-generated material on behalf of the Lab without appropriate authorization.

Specific responsibilities may be established through project agreements.

### 23.4 External Providers

Third-party providers remain subject to their own terms, services, and responsibilities.

Their presence does not remove the Lab's responsibility to assess whether their use is appropriate for a particular project.

### 23.5 Delegated Responsibilities

Where responsibilities are delegated, the scope and decision authority must be documented in accordance with `GOVERNANCE-v2.0.md`.

Technical expertise or participation in an AI project does not automatically confer publication, deployment, or governance authority.

---

## 24. High-Impact and Specialist Applications

Certain projects may require additional requirements because of their domain, audience, data, or operational environment.

Examples include:

- Healthcare-related experimentation.
- Financial applications.
- Systems affecting employment or access to services.
- Biometric technologies.
- Applications involving children.
- Systems processing sensitive personal information.
- Autonomous infrastructure operations.
- Large-scale generative systems.
- Systems making consequential recommendations or decisions.
- Applications involving high levels of autonomy or privileged access.

Such projects may require specialist assessment, legal review, external expertise, or additional safeguards.

The Lab should not assume that its general policies alone are sufficient for high-impact or regulated applications.

Where the required expertise or controls are unavailable, the project should be restricted, redesigned, or not pursued.

An exception to ordinary documentation or testing requirements must never be used to bypass fundamental security, privacy, rights, or safety obligations.

### 24.1 Specialist Review

Where a project requires expertise beyond the Lab's available capabilities, the maintainer should identify that limitation before the project proceeds to a consequential operating or publication stage.

Possible actions include:

- Restricting the scope to research or non-operational experimentation.
- Seeking appropriate external expertise.
- Obtaining a specialist evaluation.
- Redesigning the intended functionality.
- Withholding publication.
- Discontinuing the project.

### 24.2 No Unsupported Compliance Claims

The Lab must not claim that an AI system is legally compliant, certified, clinically validated, or independently audited unless the relevant assessment has actually been performed and the claim is supported.

---

## 25. Relationship with Other Lab Documents

This document is part of the Lab's technical and governance framework.

It should be read alongside:

| Document | Purpose |
|---|---|
| `README.md` | Lab identity, mission, and scope |
| `LAB-CHARTER-v2.0.md` | Foundational principles and institutional direction |
| `GOVERNANCE-v2.0.md` | Decision-making authority and responsibilities |
| `PROJECT-LIFECYCLE-v2.0.md` | Lifecycle stages and canonical Project Status definitions |
| `PROJECT-TEMPLATE-v2.0.md` | Standard project documentation and assessment fields |
| `QUALITY-STANDARDS-v2.0.md` | Technical Maturity, Operational Readiness, and engineering quality |
| `PUBLICATION-POLICY-v2.0.md` | Publication Classification, Publication Status, and release requirements |
| `RESEARCH-METHODOLOGY-v2.0.md` | Research and experimental practices |
| `SECURITY-v2.0.md` | Security practices and vulnerability reporting |
| `CONTRIBUTING-v2.0.md` | Contribution process and contributor responsibilities |
| `CODE-OF-CONDUCT-v2.0.md` | Collaboration and behavioral expectations |

Where AI-specific risks overlap with security, privacy, research, quality, or publication requirements, the relevant policies apply together.

The authoritative ownership of the relevant subjects remains with their respective documents:

| Subject | Authoritative document |
|---|---|
| Lifecycle Stage | `PROJECT-LIFECYCLE-v2.0.md` |
| Project Status | `PROJECT-LIFECYCLE-v2.0.md` |
| Technical Maturity | `QUALITY-STANDARDS-v2.0.md` |
| Operational Readiness | `QUALITY-STANDARDS-v2.0.md` |
| Publication Classification | `PUBLICATION-POLICY-v2.0.md` |
| Publication Status | `PUBLICATION-POLICY-v2.0.md` |
| AI Risk Classification | This document |
| Data Classification | `PUBLICATION-POLICY-v2.0.md` |

AI Risk Classification must not be used as a substitute for Publication Classification.

This document does not replace applicable laws, contractual obligations, professional standards, or third-party licence requirements.

---

## 26. Policy Review and Updates

This policy may be revised as AI technologies, research practices, and relevant requirements evolve.

The Founder and Maintainer is responsible for reviewing and approving revisions in accordance with `GOVERNANCE-v2.0.md`.

Updates should consider:

- Emerging AI capabilities.
- New attack methods.
- Changes in model and provider practices.
- Research and evaluation findings.
- Relevant legal and regulatory developments.
- Data protection requirements.
- Contributor feedback.
- Experience from incidents and experiments.
- Changes to the Lab's technical and operational capacity.

### 26.1 Revision Requirements

Substantive changes should:

- Identify the revised version.
- Record the effective date after approval.
- Explain the principal changes.
- Preserve the distinction between AI Risk Classification and publication classifications.
- Remain consistent with the Lab's other policies.
- Avoid unsupported legal, technical, or compliance claims.

### 26.2 Reassessment of Existing Projects

A policy revision does not automatically validate or invalidate an existing project.

However, projects should be reassessed where a policy change materially affects:

- Their intended use.
- Data handling.
- AI Risk Classification.
- Human oversight.
- External integrations.
- Permissions.
- Publication eligibility.
- Operational conditions.

---

## 27. Closing Principle

Artificial intelligence expands what can be created, explored, automated, and imagined.

It also expands the consequences of technical decisions.

The Lab therefore approaches AI not as an authority to be followed, but as a powerful technology to be understood, evaluated, and directed.

Human judgment remains essential. Technical capability must be matched by responsibility, and experimentation must remain bounded by respect for people, information, and legitimate rights.

**Explore intelligently. Automate responsibly. Keep humans accountable.**

---

**FRAMING CREATIVITY LAB**  
Independent Research · Applied AI · Creative Technology · Digital Innovation

**Maintainer:** J-ART  
**Document:** `RESPONSIBLE-AI-v2.0.md`  
**Reference:** `LAB-CHARTER-v2.0.md`

*Artificial intelligence can extend human capability. Responsibility determines how that capability is used.*
