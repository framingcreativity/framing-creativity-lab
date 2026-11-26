# Quality Standards

**Document ID:** FCL-STD-001  
**Version:** 2.0  
**Status:** Draft for Maintainer Review  
**Effective Date:** Pending approval  
**Maintainer:** J-ART  
**Repository:** Framing Creativity Lab

---

## 1. Purpose

Framing Creativity Lab combines technical experimentation, creative exploration, research, and software development. The quality of its work depends not only on whether an implementation functions, but also on whether it is understandable, appropriately tested, secure within its intended context, maintainable, and accurately represented.

This document establishes the Lab's engineering and quality expectations for work that is developed, evaluated, maintained, or prepared for publication under the Framing Creativity Lab identity.

Its objectives are to:

- establish a shared and proportionate quality framework;
- encourage clear, maintainable, and technically sound implementations;
- define expectations for testing, evaluation, and evidence;
- improve reliability, performance, accessibility, and usability;
- reduce avoidable security, privacy, and operational risks;
- support reproducible technical work and honest reporting;
- distinguish technical maturity from operational readiness;
- prevent publication approval from being mistaken for technical or operational validation; and
- provide practical completion criteria for projects and changes.

These standards are intended to guide decisions, not to impose identical engineering processes on every project. Requirements must be proportionate to the project's purpose, complexity, intended audience, operating context, and potential impact.

A small research experiment does not require the same infrastructure as a public application. It must, however, describe its limitations honestly and avoid preventable harm.

---

## 2. Scope

These standards apply to work developed, maintained, evaluated, or published within Framing Creativity Lab.

They may be applied to:

- software applications and services;
- web applications, interfaces, and digital experiences;
- APIs and backend services;
- developer tools, utilities, and supporting scripts;
- technical prototypes and proofs of concept;
- research implementations and experimental systems;
- artificial intelligence and machine-learning applications;
- autonomous or semi-autonomous workflows;
- data processing and automation systems;
- creative technology and interactive media;
- design systems and reusable components;
- infrastructure and deployment configurations; and
- technical documentation and reference implementations.

The requirements may be adapted for non-software work, research-only projects, short-lived experiments, and exploratory studies.

Where a project has additional quality requirements, those requirements should be recorded in its project documentation. Project-specific requirements may be stricter than this document where justified, but they must not be used to weaken the Lab's fundamental security, privacy, confidentiality, intellectual-property, or publication obligations.

These standards do not replace specialist policies. Their relationship to the Lab's other documents is defined in Section 22.

---

## 3. Quality Philosophy

The Lab treats quality as a set of related properties rather than a single score or visual impression.

A project may be technically functional while remaining difficult to understand or maintain. An interface may be visually refined while being inaccessible. An AI demonstration may appear convincing while producing inconsistent or unsupported outputs. A successful prototype may still be unsuitable for sustained operational use.

Quality must therefore be assessed against the project's declared purpose and the evidence available.

### 3.1 Core Quality Dimensions

| Dimension | Primary concern |
|---|---|
| Correctness | Does the implementation behave as intended? |
| Reliability | Does it behave consistently under its expected conditions? |
| Maintainability | Can it be understood, modified, and maintained? |
| Security | Are systems, data, and users protected appropriately? |
| Privacy | Is personal or sensitive information handled responsibly? |
| Performance | Are resources used efficiently for the intended workload? |
| Usability | Can the intended audience use it effectively? |
| Accessibility | Can people with different abilities access and operate it? |
| Reproducibility | Can important results or behaviours be repeated or independently examined? |
| Documentation | Can readers understand what the work does and what its limitations are? |
| Integrity | Are claims, results, and representations supported by evidence? |

The relative importance of each dimension depends on the project.

A short visual experiment may place greater emphasis on interaction quality, technical feasibility, and clear documentation of limitations. A public API requires more attention to compatibility, input validation, security, reliability, and operational behaviour.

### 3.2 Quality Is Not Surface Polish

Presentation, visual coherence, and interaction design matter, particularly in creative technology and digital experiences.

They must not conceal technical weaknesses, missing functionality, inaccessible interactions, or unverified claims.

The reverse is also true. Technical complexity does not automatically make a project useful, coherent, or well designed.

The Lab aims for alignment between intention, implementation, observed behaviour, evaluation, and published claims.

### 3.3 Quality Is Contextual

A project must be assessed against its declared purpose, scope, audience, and intended use.

An exploratory prototype is not expected to satisfy every requirement of a production system. It is expected to make its experimental status clear, handle relevant risks responsibly, and avoid presenting incomplete capabilities as established results.

A project should not be penalised simply because it is experimental. It should be assessed honestly against the quality expectations appropriate to that experiment.

### 3.4 Evidence Over Assumption

A quality claim must be supported by evidence appropriate to the claim.

Examples:

- A successful local launch demonstrates that the application started in that environment; it does not prove production reliability.
- A passing unit test supports the behaviour covered by that test; it does not prove that the whole system is correct.
- A demonstration supports the existence of a demonstrable workflow; it does not establish scalability.
- A limited evaluation may support a bounded validation claim; it does not establish universal suitability.
- A public release indicates that publication was authorised; it does not establish production readiness.

The level of confidence communicated must remain proportional to the scope and quality of the evidence.

---

## 4. Technical Maturity and Operational Readiness

Technical Maturity and Operational Readiness are separate assessment dimensions. Publication is a third, independent decision governed by `PUBLICATION-POLICY-v2.0.md`.

These dimensions answer different questions:

- **Technical Maturity:** What has been implemented and demonstrated through evidence?
- **Operational Readiness:** For what operating context has the work been assessed?
- **Publication Classification and Status:** What publication scrutiny applies, and what is the current publication decision?

They must not be combined into one scale or inferred from one another.

### 4.1 Technical Maturity

Use the following values to record the project's technical maturity assessment.

#### Not Assessed

No maturity assessment has been recorded, or the available evidence is insufficient to assign a meaningful level.

This value describes the state of the assessment. It does not indicate that the project has failed or that the work has no maturity.

#### Exploratory

Intended for early investigation, technical feasibility checks, and short experiments.

A project at this level may include temporary implementation choices, incomplete functionality, or changing assumptions.

Expected practices:

- a clear experimental or technical objective;
- a sufficiently understandable method or implementation;
- basic implementation discipline appropriate to the work;
- appropriate handling of credentials and private data;
- identification of major dependencies and constraints;
- minimal but useful documentation;
- recording of significant observations and limitations; and
- honest communication of what has and has not been demonstrated.

Exploratory work must not be represented as completed, validated, or operationally reliable merely because it produces a successful result once.

#### Prototype

Intended for a demonstrable implementation used to test a concept, evaluate an approach, or explore a proposed system.

Expected practices:

- defined scope and intended behaviour;
- an understandable project structure;
- demonstrable core functionality;
- basic functional testing;
- appropriate input validation;
- relevant error handling;
- documented setup requirements and dependencies;
- identification of significant technical limitations;
- review of relevant security and privacy risks; and
- clear communication that the implementation is a prototype.

A prototype may be incomplete or unstable. Its behaviour must nevertheless be understood well enough to support meaningful evaluation.

#### Validated

Intended for work that has undergone structured testing or evaluation against defined objectives and acceptance criteria.

Expected practices:

- documented objectives and acceptance criteria;
- a suitable validation method;
- recorded test or evaluation results;
- relevant unit, integration, system, or user-facing tests;
- examination of significant failure conditions;
- documented limitations and unresolved issues;
- maintainable implementation appropriate to the project;
- documented architecture and dependencies where relevant;
- security and privacy review proportionate to risk; and
- evidence supporting the claims being made.

Validation applies only to the scope, conditions, configurations, and test cases actually evaluated.

A validated project must not be presented as universally reliable, secure, scalable, compliant, or suitable for every environment unless those distinct claims have been separately assessed.

### 4.2 Operational Readiness

Record Operational Readiness separately from Technical Maturity.

| Readiness | Meaning |
|---|---|
| Not Assessed | No operational-readiness assessment has been recorded, or available evidence is insufficient to assign a meaningful value. |
| Research or Experimental Use Only | Intended for controlled research, testing, or experimentation. It is not represented as suitable for real-world operational use. |
| Demonstration Only | Suitable for a bounded demonstration or evaluation context. No production use is implied. |
| Limited Operational Use | Suitable only for a defined and constrained operating context with documented limitations, responsibilities, safeguards, and usage conditions. |
| Production-Oriented | Designed and assessed against sustained operational requirements, including appropriate security, reliability, monitoring, recovery, maintenance, and support considerations. |

An Operational Readiness assessment should consider, where relevant:

- the intended users and operating environment;
- the importance and consequences of system failure;
- authentication, authorisation, and permission boundaries;
- data sensitivity and data-handling requirements;
- expected availability and performance;
- monitoring, logging, and incident detection;
- backup, recovery, and continuity;
- dependency and infrastructure maintenance;
- deployment, configuration, and rollback;
- support responsibilities and maintenance capacity; and
- known operational limitations.

A **Production-Oriented** assessment requires explicit evidence proportionate to the system's intended impact and operating environment. It must not be inferred from a successful demonstration, public deployment, polished interface, technical maturity label, or publication approval.

Production-Oriented is an internal readiness descriptor. It is not a certification, warranty, guarantee of uninterrupted operation, or claim that a system is suitable for every production environment.

### 4.3 Publication Is a Separate Decision

Publication Classification and Publication Status are not Technical Maturity or Operational Readiness values.

- **Publication Classification (`P0`–`P3`)** is defined in `PUBLICATION-POLICY-v2.0.md` and determines the applicable publication scrutiny and restrictions.
- **Publication Status (`PENDING`, `APPROVED`, `REJECTED`, or `WITHDRAWN`)** records the current publication review state or final decision under `PUBLICATION-POLICY-v2.0.md`.
- A public release does not automatically establish Validated Technical Maturity or Production-Oriented Operational Readiness.
- Publication approval does not itself mean that the material has already been released.
- A project must not be described as Published until the approved material has actually been made publicly available.

The Quality Standards document does not redefine P0–P3 or the publication decision process. Use `PUBLICATION-POLICY-v2.0.md` as the authoritative source for publication classification, approval, release, and withdrawal.

### 4.4 Recording and Reassessing Assessments

Where these assessments are relevant, the project record should identify:

- the assigned Technical Maturity;
- the assigned Operational Readiness;
- the evidence supporting each assessment;
- the scope and conditions covered;
- significant limitations and outstanding risks;
- the assessment date; and
- the person responsible for the assessment.

Assessments should be revisited when the project scope, architecture, data, dependencies, intended users, operating environment, or material risks change.

A previous assessment must not be treated as permanently valid after a material change.

---

## 5. Engineering and Code Quality

### 5.1 General Principles

Code developed within the Lab should be:

- understandable;
- consistent;
- purposeful;
- appropriately modular;
- maintainable;
- testable;
- secure within its intended context; and
- free of unnecessary complexity.

The implementation should express its intended behaviour clearly and avoid relying on hidden assumptions.

Engineering choices should reflect the project's purpose and expected evolution. A simple implementation is preferable when it adequately addresses the problem.

### 5.2 Readability

Implementations should use clear names, logical structure, and consistent formatting.

Where relevant:

- use meaningful identifiers;
- keep functions and components focused;
- avoid unnecessary nesting and deeply coupled logic;
- separate unrelated responsibilities;
- remove obsolete code and unused dependencies;
- document non-obvious behaviour and important constraints;
- avoid unexplained constants and configuration values; and
- prefer explicit behaviour over unnecessarily clever implementation.

Comments should explain intent, constraints, or non-obvious decisions rather than simply restating the code.

### 5.3 Modularity and Separation of Concerns

Where appropriate, implementations should separate concerns into logical units.

Examples include:

- presentation and application logic;
- data access and business rules;
- configuration and runtime behaviour;
- external integrations and internal functionality;
- reusable components and project-specific components; and
- infrastructure and application code.

Modularity should solve an actual organizational or maintenance problem.

Excessive abstraction can make a small project harder to understand without providing meaningful benefit. Reusable structures should be introduced when their responsibilities and interfaces can be defined clearly.

### 5.4 Reusability

Reusable components, functions, tools, and modules should have:

- a clear purpose;
- a defined interface;
- documented assumptions;
- predictable behaviour;
- appropriate input and output handling; and
- a maintenance approach proportionate to their expected use.

Reuse should not be pursued at the expense of clarity.

A component should not become a generic abstraction merely because two implementations share superficial similarities.

### 5.5 Error Handling

Projects should handle expected error conditions deliberately.

Depending on the application, this may include:

- invalid or incomplete input;
- missing resources;
- network failures;
- authentication or authorisation failures;
- service timeouts;
- API errors;
- file access problems;
- database failures;
- unavailable dependencies; and
- unexpected external responses.

Errors should be handled at appropriate boundaries.

Where possible, an error should provide enough information to support diagnosis without exposing credentials, private data, internal paths, sensitive configuration, or other restricted information.

Silent failure should be avoided where it could mislead users or conceal data loss, incomplete operations, or unsafe conditions.

### 5.6 Configuration Management

Configuration should be separated from application logic where appropriate.

Projects should distinguish between:

- public configuration;
- environment-specific configuration;
- sensitive configuration;
- build-time settings; and
- runtime settings.

Secrets must not be committed to public source code.

Required configuration variables should be documented without publishing their sensitive values. Example configuration files should use clearly identified placeholders.

### 5.7 Code Consistency

Projects should use consistent conventions for formatting, naming, file organisation, and error handling.

Automated formatters, linters, type checkers, and static analysis tools may be used where they provide practical value.

Tooling should be proportionate. Introducing a tool must have a clear benefit relative to its configuration and maintenance cost.

### 5.8 Safe Changes

Changes should be scoped and understandable.

Where a change affects existing behaviour, relevant compatibility expectations should be considered. Unrelated refactoring should not be bundled into a narrowly scoped correction unless there is a clear reason.

A change should not silently remove important functionality, alter data semantics, weaken security controls, or invalidate documented behaviour.

---

## 6. Architecture and Technical Design

### 6.1 Architectural Clarity

Architecture should reflect the project's purpose, complexity, constraints, and expected evolution.

A technical design should avoid unnecessary dependencies, tightly coupled components, unexplained implementation decisions, and hidden operational assumptions.

Architecture should remain understandable to someone other than the original author, to the degree appropriate for the project's scope.

### 6.2 Appropriate Complexity

The Lab favours solutions that are sufficiently robust without being unnecessarily complex.

Architectural decisions should consider:

- functional requirements;
- technical constraints;
- project scope and maturity;
- expected scale and usage;
- maintainability;
- security and privacy;
- external dependencies;
- resource requirements; and
- foreseeable changes.

A simple architecture is preferable when it adequately addresses the problem.

Complexity should be justified by actual requirements, not by novelty or the availability of a particular technology.

### 6.3 Architecture Documentation

For projects with meaningful architectural complexity, documentation should identify, where relevant:

- main components and their responsibilities;
- important data flows;
- external integrations;
- significant dependencies;
- configuration boundaries;
- security-sensitive components;
- storage and persistence mechanisms;
- relevant execution or deployment environments; and
- important design decisions.

Architecture Decision Records (ADRs) may be used for decisions with significant long-term implications.

Documentation should record the reason for a consequential decision and relevant alternatives considered. It need not formalise every minor implementation choice.

### 6.4 Dependency Management

Dependencies should be introduced deliberately.

Projects should:

- avoid unnecessary packages and services;
- prefer established and maintained dependencies where appropriate;
- review licensing and usage conditions;
- consider security history and maintenance activity;
- avoid unnecessary duplication of functionality;
- document important external dependencies;
- use lockfiles or version constraints where appropriate; and
- update vulnerable or obsolete dependencies when justified.

The introduction of a dependency should provide a clear benefit relative to its maintenance, security, compatibility, and resource costs.

### 6.5 Technical Debt

Technical debt is an accepted part of experimentation, provided it remains visible and understood.

Temporary workarounds, incomplete abstractions, and architectural compromises should be documented when they materially affect future work.

Where useful, technical debt may be described by:

- impact;
- reason for introduction;
- affected components;
- known consequences;
- recommended resolution; and
- priority.

Experimental debt should not silently become permanent architecture.

### 6.6 Architecture and Project Maturity

Architectural expectations should reflect the project's Technical Maturity and Operational Readiness.

An exploratory experiment may use a temporary architecture where that choice is safe and documented. A system intended for Limited Operational Use or Production-Oriented use requires greater attention to maintainability, resilience, security boundaries, and operational dependencies.

A project must not describe an architecture as scalable, secure, resilient, or production-ready merely because it follows a recognised pattern.

---

## 7. Testing and Validation

### 7.1 Testing Philosophy

Testing should provide meaningful evidence that a project behaves as intended.

The level and type of testing must correspond to the project's functionality, Technical Maturity, Operational Readiness, and potential impact.

Testing is not limited to checking whether an application starts successfully.

The purpose of testing is to examine expected behaviour, identify failures, verify important constraints, and provide evidence for claims.

### 7.2 Testing Categories

Depending on the project, relevant tests may include:

**Unit Testing**

Tests focused on individual functions, modules, or components.

**Integration Testing**

Tests verifying interactions between internal components or external services.

**System Testing**

Tests evaluating the behaviour of the complete application or system.

**End-to-End Testing**

Tests covering important user journeys or complete workflows.

**Regression Testing**

Tests ensuring that changes do not unintentionally break previously functioning behaviour.

**Performance Testing**

Tests evaluating response time, throughput, resource consumption, or behaviour under load.

**Security Testing**

Tests examining vulnerabilities, permission boundaries, input handling, and unsafe behaviour.

**Accessibility Testing**

Tests evaluating whether relevant interfaces and interactions are accessible to the intended audience.

**User or Expert Evaluation**

Structured evaluation by representative users, reviewers, or subject-matter experts where the project requires it.

### 7.3 Test Expectations

Where tests are applicable, they should:

- have a clear purpose;
- cover relevant behaviour and important edge cases;
- be repeatable where practical;
- use appropriate test data;
- avoid exposing confidential information;
- provide understandable results;
- distinguish expected from observed outcomes; and
- be updated when relevant functionality changes.

Tests should be proportionate to the potential consequences of failure.

### 7.4 Test Coverage

Code coverage may be used as an indicator of which code has been exercised. It is not a complete measure of quality.

A high coverage percentage does not guarantee meaningful assertions, adequate edge-case handling, correct system behaviour, or reliability.

The relevance and quality of tests matter more than the metric alone.

### 7.5 Known Failures

Unresolved test failures should be:

- investigated;
- documented;
- corrected where necessary; or
- explicitly accepted as limitations where appropriate.

A known failure must not be concealed to make a project appear more mature than it is.

Where a failure prevents a reliable assessment, the relevant maturity or readiness claim should be withheld or qualified.

### 7.6 Validation Records

For material validation work, retain a record of:

- what was evaluated;
- the environment and configuration;
- test inputs or relevant conditions;
- the method used;
- expected and observed results;
- failures or deviations;
- limitations; and
- the conclusion supported by the evidence.

A validation record should make it possible to understand what the evaluation actually established.

---

## 8. Reliability and Resilience

Systems should behave predictably under their intended operating conditions.

Where relevant, projects should consider:

- network interruptions;
- external service failures;
- timeouts;
- invalid or incomplete responses;
- resource exhaustion;
- concurrent operations;
- unexpected user inputs;
- partial system failures; and
- recovery behaviour.

Reliability requirements must be proportionate to the consequences of failure and the project's intended use.

### 8.1 Graceful Failure

Where practical, failures should be handled without unnecessarily affecting unrelated functionality.

The system should communicate failures clearly while avoiding disclosure of sensitive technical details.

A fallback mechanism should not conceal a failure when the user or operator needs to know that the system is operating with reduced capability.

### 8.2 External Service Failures

Projects depending on external APIs, models, databases, or platforms should consider provider availability and failure behaviour.

Where appropriate, implementations should include:

- timeouts;
- deliberate error handling;
- rate-limit handling;
- bounded retry policies;
- safe fallback behaviour;
- clear dependency documentation; and
- user or operator feedback when a dependency is unavailable.

Retries should be designed carefully to avoid duplicated operations, resource exhaustion, or unintended side effects.

### 8.3 State and Data Integrity

Projects that modify or store data should consider how data integrity is preserved.

Depending on the implementation, this may include:

- input and schema validation;
- transactional operations;
- consistency checks;
- idempotency where relevant;
- backup strategies;
- recovery procedures;
- protection against partial writes; and
- explicit handling of failed or interrupted operations.

Data integrity requirements should reflect the importance of the information and the consequences of corruption or loss.

### 8.4 Recovery and Continuity

Where a project is intended for sustained operational use, recovery expectations should be documented.

Depending on the context, this may include restoration procedures, backup frequency, recovery objectives, rollback procedures, and responsibility for maintaining recovery mechanisms.

Do not claim that a system is recoverable merely because backups are configured. Relevant restoration procedures should be tested where practical.

---

## 9. Performance and Resource Efficiency

Performance should be evaluated in relation to the intended use, workload, and operating environment.

Relevant considerations may include:

- response time;
- initial loading time;
- memory consumption;
- CPU and GPU usage;
- network usage;
- database operations;
- asset size;
- rendering performance;
- API latency;
- model inference time; and
- infrastructure or provider cost.

### 9.1 Performance Practices

Projects should avoid unnecessary resource consumption.

Where appropriate, this may involve:

- efficient data access;
- optimised asset delivery;
- appropriate caching;
- lazy loading;
- avoiding unnecessary network requests;
- reducing redundant computations;
- efficient rendering and state management;
- appropriate background processing; and
- sensible request, concurrency, and timeout limits.

Optimisation should be guided by observed behaviour rather than premature assumptions.

### 9.2 Performance Claims

Performance claims should identify their measurement conditions.

Where possible, documentation should indicate:

- test environment;
- workload;
- dataset or input characteristics;
- measurement method;
- sample size or duration where relevant; and
- important limitations.

Statements such as "fast", "scalable", or "low latency" should be supported by appropriate evidence when used as technical claims.

### 9.3 Resource Awareness

Where projects rely on paid APIs, cloud infrastructure, computationally expensive models, or large data transfers, relevant cost implications should be considered.

Experimental configurations should not unintentionally create uncontrolled resource consumption.

Where costs can vary significantly with usage, limits, quotas, or alerts may be appropriate.

### 9.4 Performance and User Experience

Performance should be evaluated from the perspective of the intended user or downstream system.

A technically efficient implementation may still provide a poor experience if important interactions are delayed, loading states are unclear, or system behaviour is inconsistent.

Performance optimisation should preserve correctness, accessibility, and comprehensibility.

---

## 10. Security and Privacy Quality

Security and privacy are fundamental quality dimensions. They must be considered throughout development rather than added only before publication.

This section defines quality expectations. Detailed vulnerability reporting, incident response, and security handling procedures remain governed by `SECURITY-v2.0.md`. Publication and confidentiality decisions remain governed by `PUBLICATION-POLICY-v2.0.md`.

### 10.1 Secure Development

Projects should consider, where relevant:

- input validation;
- authentication;
- authorisation;
- session management;
- secure configuration;
- dependency vulnerabilities;
- access control;
- error handling;
- logging practices;
- data protection; and
- secure deployment.

Security requirements should reflect the actual capabilities, permissions, data, and risks of the system.

### 10.2 Privacy by Design

Projects processing personal or sensitive information should consider:

- data minimisation;
- purpose limitation;
- appropriate access restrictions;
- data retention;
- secure storage;
- secure transmission;
- deletion and disposal;
- third-party processing; and
- user transparency.

Data should not be collected or retained without a justified purpose.

Privacy claims must reflect actual system behaviour and should not be inferred from the absence of obvious identifying fields.

### 10.3 Secrets Management

Credentials, API keys, tokens, private keys, certificates, and other secrets must be stored through appropriate secret-management mechanisms.

Public examples should use placeholders or documented environment variables rather than real credentials.

Secrets must not appear in source code, issue examples, logs, screenshots, test fixtures, or public documentation.

### 10.4 Security Review

Security reviews should be proportionate to the project's risk.

Public-facing systems, privileged integrations, data-processing applications, automation with external permissions, and AI agents with tool access require particular attention.

Where practical, review should consider trust boundaries, permissions, authentication, data flows, exposed interfaces, and dependency risks.

### 10.5 Confidentiality

Technical quality does not justify the disclosure of proprietary or confidential material.

Public projects must remain separate from private projects, internal implementations, client information, and unauthorised third-party material.

A project must not include confidential details merely to make a technical explanation more complete. Use a safe abstraction or omit the material where publication rights are uncertain.

### 10.6 Security Limitations

Experimental status does not justify publishing exposed credentials, unauthorised personal information, or avoidable security weaknesses.

Where relevant security controls are incomplete, the limitation should be documented and the permitted use restricted accordingly.

Do not represent an experimental system as secure or production-ready solely because no vulnerability has yet been reported.

---

## 11. User Experience and Interaction Quality

For projects with a user-facing interface, usability and interaction quality are part of technical quality.

### 11.1 Functional Clarity

Interfaces should communicate:

- what users can do;
- what the system is doing;
- what has succeeded or failed;
- what information is required; and
- what happens after an action.

Controls should behave consistently and provide meaningful feedback.

### 11.2 Interaction Design

Interactions should be:

- predictable;
- responsive;
- understandable;
- consistent; and
- appropriate to the intended context.

Unexpected movement, unnecessary animation, ambiguous controls, and inconsistent interaction patterns should be avoided.

### 11.3 Visual Consistency

Visual systems should use coherent layout, spacing, typography, colour, and component behaviour.

Where a project uses a design system, components and design tokens should be applied consistently.

Visual polish should support comprehension and interaction rather than interfere with them.

### 11.4 Responsive Design

Interfaces intended for different screen sizes should be tested across relevant viewport dimensions and input methods.

Responsive behaviour should preserve:

- content readability;
- navigation clarity;
- interaction accessibility;
- functional completeness; and
- appropriate visual hierarchy.

Responsive design must not be limited to shrinking desktop layouts.

### 11.5 User Feedback

Important actions should provide appropriate confirmation, progress indication, error feedback, or recovery guidance.

Loading states, empty states, and error states should be considered where relevant.

The interface should avoid implying that an operation succeeded when the underlying action is incomplete or has failed.

### 11.6 Content and Interface Accuracy

Interface text, screenshots, demonstrations, and documentation should accurately represent implemented functionality.

A mock-up, prototype, or simulated interaction must not be presented as a working capability unless it actually operates as described.

---

## 12. Accessibility

Accessibility should be considered during interface design and implementation, not treated solely as a final check.

For user-facing applications, relevant practices include:

- semantic HTML and appropriate document structure;
- meaningful heading hierarchy;
- keyboard navigation;
- visible focus states;
- descriptive labels;
- accessible form instructions;
- text alternatives for meaningful images;
- sufficient colour contrast;
- avoidance of colour-only communication;
- appropriate screen-reader behaviour;
- respect for reduced-motion preferences; and
- understandable error messages.

### 12.1 Accessibility Evaluation

Where appropriate, accessibility may be evaluated against recognised standards such as the Web Content Accessibility Guidelines (WCAG).

When a project makes a formal accessibility or conformance claim, the applicable standard version, conformance target, scope, and evaluation method should be identified.

A project must not claim full accessibility or WCAG conformance solely because an automated tool reports no errors.

Automated checks should be complemented by manual evaluation where practical, including keyboard and assistive-technology testing appropriate to the interface.

### 12.2 Motion and Animation

Animation should have a clear interaction, communication, or expressive purpose.

Excessive or unnecessary movement may reduce usability and accessibility.

Projects should consider:

- reduced-motion preferences;
- animation duration;
- repetition;
- movement intensity;
- interaction feedback; and
- potential distraction.

Creative experimentation should remain compatible with reasonable accessibility considerations.

### 12.3 Accessibility Limitations

Where a project has known accessibility limitations, they should be documented accurately.

A limitation should not be hidden by broad claims that an interface is accessible. The project should identify the affected experience and, where practical, provide an alternative way to access essential information or functionality.

---

## 13. AI and Machine-Learning Quality

AI-enabled projects require additional technical evaluation because their outputs may be variable, probabilistic, context-dependent, or difficult to predict.

This section addresses technical quality and evaluation. The Lab's broader AI principles, risk classifications, human oversight requirements, and restrictions are defined in `RESPONSIBLE-AI-v2.0.md`.

### 13.1 Clear AI Functionality

Documentation should explain where AI is used and what role it performs.

Examples include:

- text generation;
- image, audio, or video generation;
- classification;
- search and retrieval;
- recommendation;
- decision support;
- agent-based workflows;
- tool orchestration;
- data extraction; and
- predictive analysis.

Users and reviewers should not be misled about which capabilities are automated, model-generated, deterministic, or human-reviewed.

### 13.2 Model and Configuration Documentation

Where relevant, experiments should record:

- model name and version;
- provider or source;
- relevant configuration;
- model parameters;
- prompt or instruction version;
- retrieval configuration;
- tools and integrations;
- dataset or evaluation inputs;
- date of evaluation; and
- important environmental conditions.

Credentials, access tokens, confidential provider information, and restricted prompts must not be included in public documentation.

The level of detail should be sufficient to understand the experiment without exposing protected information or violating applicable terms.

### 13.3 Output Evaluation

AI outputs should be assessed according to the intended task.

Potential evaluation dimensions include:

- accuracy;
- relevance;
- consistency;
- completeness;
- instruction adherence;
- robustness;
- latency;
- resource consumption;
- safety; and
- human-perceived quality.

The evaluation method should be appropriate to the application.

For creative tasks, qualitative expert or user assessment may be more meaningful than a single numerical score. For factual or structured tasks, reference data and explicit evaluation criteria may be appropriate.

### 13.4 Hallucinations and Unsupported Claims

Projects that generate factual information should consider how unsupported statements are detected, communicated, or mitigated.

Where appropriate, the system should:

- identify uncertainty;
- preserve source attribution;
- distinguish retrieved information from generated interpretation;
- avoid presenting unverified outputs as established facts; and
- support human review for consequential decisions.

### 13.5 Variability and Reproducibility

AI outputs may change due to model updates, provider behaviour, configuration changes, sampling, and nondeterministic inference.

Exact reproducibility should not be claimed unless the relevant conditions can reasonably be controlled.

Where exact reproduction is impossible, the project should document the factors that influence variation and provide a practical method for repeating the evaluation.

### 13.6 Human Review and Output Boundaries

Where AI outputs influence important decisions or actions, the project should define the relevant review and permission boundaries in accordance with `RESPONSIBLE-AI-v2.0.md`.

Model-generated code, scripts, queries, configurations, and commands should be treated as untrusted until reviewed and validated.

Security, data access, and operational permissions must be enforced independently of model-generated content.

### 13.7 AI Quality Does Not Establish Responsible Use

A technically accurate or high-performing AI system is not automatically appropriate to deploy.

Technical quality evaluation does not replace the AI-specific governance, risk assessment, and restrictions defined in `RESPONSIBLE-AI-v2.0.md`.

---

## 14. Research Integrity and Reproducibility

Research quality depends on the reliability of its methods, evidence, interpretation, and reporting.

Detailed research design, experimental methodology, and the Lab's internal evidence framework are governed by `RESEARCH-METHODOLOGY-v2.0.md`. This section establishes the quality expectations that apply to research outputs.

Projects involving research or structured experimentation should:

- define their objectives clearly;
- document relevant methods;
- identify assumptions and limitations;
- preserve relevant experimental configurations where permitted;
- distinguish observations from interpretations;
- avoid selectively presenting results;
- report significant negative or inconclusive findings where relevant; and
- support reproduction of important experiments where feasible.

### 14.1 Evidence-Based Claims

Claims should not exceed the available evidence.

A successful test under limited conditions does not establish universal reliability.

A demonstration does not prove scalability.

A promising preliminary result does not establish a general conclusion.

The level of confidence should correspond to the quality, scope, and limitations of the evidence.

### 14.2 Methodological Limitations

Relevant limitations should be communicated.

These may include:

- small sample sizes;
- limited test environments;
- incomplete datasets;
- known measurement bias;
- model variability;
- external service dependencies;
- uncontrolled experimental conditions; and
- incomplete validation.

Limitations should be specific enough for readers to understand their effect on the interpretation of the results.

### 14.3 Reproducibility

Where practical, projects should preserve the information needed to repeat important experiments.

This may include code versions, configuration, dependencies, test inputs, model identifiers, and measurement methods.

Reproducibility must remain subject to privacy, confidentiality, intellectual-property, licensing, and data-access restrictions.

The inability to publish a complete experimental configuration must not be concealed. Document the limitation without disclosing protected material.

### 14.4 Negative and Inconclusive Results

Failed, negative, or inconclusive experiments may provide useful technical knowledge.

They should not be selectively omitted where their exclusion would materially misrepresent the experiment or its conclusions.

The purpose of reporting is to preserve an accurate account of what was tested and observed, not to make every project appear successful.

---

## 15. Documentation Standards

Documentation is part of the deliverable, not an optional addition.

It should help readers understand what a project does, how to use or evaluate it, what dependencies it requires, and what limitations apply.

### 15.1 General Documentation Requirements

Where relevant, project documentation should include:

- project purpose and scope;
- current Project Status and Lifecycle Stage;
- Technical Maturity and Operational Readiness;
- main functionality;
- installation or setup instructions;
- configuration requirements;
- dependencies;
- usage examples;
- limitations and known issues;
- licensing and attribution information; and
- relevant security and privacy considerations.

Use the canonical Project Status and Lifecycle Stage values defined in `PROJECT-LIFECYCLE-v2.0.md`.

Use the Technical Maturity and Operational Readiness values defined in this document.

Publication Classification and Publication Status must follow `PUBLICATION-POLICY-v2.0.md`.

### 15.2 Technical Documentation

Complex projects may require:

- architecture descriptions;
- component responsibilities;
- API references;
- data structures;
- configuration references;
- integration instructions;
- testing procedures;
- deployment guidance; and
- maintenance notes.

The documentation depth should reflect the complexity and expected use of the project.

### 15.3 Documentation Accuracy

Documentation must reflect the current implementation.

Instructions must not claim functionality that has not been implemented or validated.

Known limitations should be visible and understandable. Screenshots, diagrams, examples, and demonstrations should represent the actual implementation or be clearly identified as conceptual material.

### 15.4 Writing Quality

Technical documentation should be:

- clear;
- accurate;
- structured;
- consistent;
- specific; and
- free of unnecessary ambiguity.

Use terminology consistently. Distinguish requirements from recommendations and examples.

Examples should be relevant, valid, and safe to execute.

### 15.5 Documentation Maintenance

Material changes to functionality, interfaces, dependencies, configuration, or operating assumptions should trigger a review of affected documentation.

Obsolete instructions should be corrected or clearly marked as historical.

Documentation should not imply that a project is maintained, supported, or available beyond what the Lab can reasonably provide.

---

## 16. Dependency, Tooling, and Environment Standards

Projects should document their relevant development and runtime requirements.

Where applicable, this may include:

- programming language and version;
- framework and version;
- package manager;
- major dependencies;
- operating system requirements;
- environment variables;
- external services;
- build requirements;
- testing commands;
- deployment assumptions; and
- required access permissions.

### 16.1 Reproducible Environments

Where practical, projects should use dependency lockfiles, version constraints, containers, environment files, or other mechanisms that support consistent setup.

The chosen approach should reflect the project architecture and the level of reproducibility required.

Do not introduce environment tooling solely for appearance or without a practical maintenance benefit.

### 16.2 Tooling Consistency

Formatting, linting, type checking, build validation, and automated testing may be used to improve consistency.

Tooling should support development rather than introduce unnecessary complexity.

The project documentation should identify important commands and required tooling where readers are expected to reproduce the development or test environment.

### 16.3 Build and Deployment

Projects intended for distribution or deployment should document the relevant build and deployment process.

Where appropriate, this includes:

- build commands;
- required configuration;
- output artefacts;
- deployment environment;
- release procedure; and
- rollback or recovery considerations.

A successful local build does not by itself establish that the project can be deployed safely or reliably in another environment.

### 16.4 Environment Separation

Where projects use multiple environments, distinguish development, testing, staging, and production configurations as applicable.

Sensitive credentials and data must not be copied into less protected environments without an appropriate basis and safeguards.

Environment-specific assumptions should be documented where they materially affect behaviour.

---

## 17. External Integrations and Third-Party Services

Projects may depend on external models, APIs, frameworks, services, libraries, datasets, or platforms.

Such dependencies introduce technical, security, privacy, intellectual-property, licensing, and operational considerations.

Before adoption, relevant questions include:

- Is the provider or source sufficiently documented?
- Are the terms of use compatible with the project?
- Are data-handling practices understood?
- Are there rate limits or usage restrictions?
- Could the provider change or discontinue the service?
- What happens when the service is unavailable?
- Does the integration require sensitive permissions?
- Are costs or resource requirements significant?
- Is the integration maintainable within the Lab's available capacity?

### 17.1 Integration Boundaries

External integrations should have clear interfaces and responsibilities.

Where appropriate, projects should isolate provider-specific behaviour so that failures, changes, or replacements do not unnecessarily affect unrelated functionality.

The project should document significant assumptions about provider availability, versioning, configuration, and data handling.

### 17.2 Provider and Service Claims

Projects should not imply that an external service is controlled, endorsed, supported, or maintained by Framing Creativity Lab unless this is actually the case.

Provider names, logos, and service descriptions should be used accurately and in accordance with applicable terms.

### 17.3 Third-Party Technologies and Assets

Third-party libraries, models, datasets, media, and other assets must be identified and used within applicable rights and usage conditions.

Attribution should be provided where required.

Unresolved licensing, ownership, or usage questions must be referred to the applicable publication and contribution procedures. This document does not grant permission to use third-party material.

---

## 18. Code Review and Quality Assurance

Where review is applicable, proposed changes should be evaluated according to their scope and impact.

A review may consider:

- correctness;
- readability;
- architecture;
- consistency;
- test coverage and relevance;
- security;
- performance;
- accessibility;
- documentation;
- backward compatibility; and
- licensing and dependencies.

### 18.1 Review Expectations

Review feedback should be specific, constructive, and technically relevant.

Material issues should be addressed before acceptance or clearly documented as accepted limitations by the responsible maintainer.

A review should distinguish defects that prevent acceptance from recommendations that improve maintainability or future evolution.

### 18.2 Proportionate Review

Small documentation corrections may require a simple review.

Changes affecting authentication, sensitive data, architecture, external integrations, privileged execution, or consequential AI behaviour should receive greater scrutiny.

The review method should reflect the actual risk and complexity of the change.

### 18.3 Acceptance

The maintainer determines whether a contribution meets the relevant project requirements in accordance with `GOVERNANCE-v2.0.md` and `CONTRIBUTING-v2.0.md`.

Acceptance into a repository does not automatically establish Validated Technical Maturity, Production-Oriented Operational Readiness, publication approval for separate material, or authorisation for commercial or external use.

### 18.4 Review Records

For material changes, retain an appropriate record of:

- the change reviewed;
- the relevant files or components;
- tests or checks performed;
- material findings;
- accepted limitations; and
- the acceptance or rejection decision.

A record may be concise where the change is small. It should be sufficient to understand the basis for a material decision.

---

## 19. Quality Gates and Definition of Done

A project or change should have a clear definition of completion appropriate to its purpose, Technical Maturity, Operational Readiness, and potential impact.

The following checklists provide a general reference. They should be adapted to the actual work rather than applied mechanically.

Passing a checklist does not replace project-specific risk assessment or professional judgment.

### 19.1 Exploratory Completion

- [ ] The research or experimental objective is documented.
- [ ] The method or implementation is sufficiently understandable.
- [ ] Relevant dependencies are identified.
- [ ] Significant assumptions and limitations are recorded.
- [ ] Sensitive information is handled appropriately.
- [ ] Findings and observations are documented.
- [ ] The work is not represented as more mature than the evidence supports.

### 19.2 Prototype Completion

- [ ] Intended functionality and scope are defined.
- [ ] Core interactions or workflows are demonstrable.
- [ ] Relevant functional tests have been conducted.
- [ ] Important error conditions have been considered.
- [ ] Setup and usage instructions are available where needed.
- [ ] Known limitations are documented.
- [ ] Relevant security and privacy concerns are reviewed.
- [ ] Prototype status is clearly communicated.
- [ ] Operational limitations are not concealed.

### 19.3 Validated Completion

- [ ] Objectives and acceptance criteria are defined.
- [ ] Relevant tests or evaluation methods have been conducted.
- [ ] Results and limitations are documented.
- [ ] Material defects are addressed or disclosed.
- [ ] Dependencies and architecture are sufficiently documented.
- [ ] Claims are supported by evidence.
- [ ] Relevant quality dimensions have been evaluated.
- [ ] The validation scope and conditions are clear.
- [ ] The validation claim does not exceed the available evidence.

### 19.4 Public Release Readiness

This checklist concerns the technical quality of a proposed public release. Publication Classification, publication approval, and release authorisation remain governed by `PUBLICATION-POLICY-v2.0.md`.

- [ ] Publication has been explicitly reviewed and approved through the applicable process.
- [ ] No unauthorised confidential material is included.
- [ ] No secrets or credentials are exposed.
- [ ] Ownership, licensing, and attribution have been reviewed.
- [ ] Dependencies and external assets have been checked.
- [ ] Documentation is accurate and usable.
- [ ] Technical Maturity and limitations are clearly communicated.
- [ ] Relevant security and privacy concerns have been addressed.
- [ ] Known issues and external requirements are disclosed.
- [ ] Release information is prepared where appropriate.
- [ ] The material being released matches the approved scope.

### 19.5 Production-Oriented Readiness

This checklist supports an Operational Readiness assessment. It is not a certification or guarantee of operational suitability.

- [ ] Operational requirements and intended users are defined.
- [ ] Authentication and authorisation are appropriate.
- [ ] Relevant security testing has been completed.
- [ ] Monitoring and logging are considered.
- [ ] Failure and recovery behaviour is understood.
- [ ] Performance has been evaluated under representative conditions.
- [ ] Backup and recovery arrangements exist where needed.
- [ ] Dependencies and infrastructure have maintenance owners.
- [ ] Support and incident procedures are defined where applicable.
- [ ] Deployment and rollback procedures are documented where relevant.
- [ ] Data handling and retention practices are understood.
- [ ] Operational limitations and responsibilities are documented.
- [ ] The available maintenance capacity is compatible with the intended use.

### 19.6 Acceptance and Remaining Work

A project or change may be accepted with known limitations where those limitations are understood, proportionate, documented, and compatible with the intended use.

Acceptance must not be used to conceal unresolved critical risks, unauthorised material, exposed credentials, or publication restrictions.

Where remaining work affects Technical Maturity or Operational Readiness, the relevant assessment must reflect that limitation.

---

## 20. Quality Exceptions

Exceptions may be necessary for experimental, constrained, or short-lived projects.

Examples include:

- a short-lived proof of concept;
- a prototype with known architectural limitations;
- a research implementation that prioritises evaluation over maintainability;
- a demonstration dependent on an external service;
- an experiment using temporary infrastructure; or
- a project for which full automation would be disproportionate.

Exceptions should be:

- intentional;
- limited in scope;
- understood by the responsible maintainer;
- documented when materially relevant; and
- consistent with fundamental security, privacy, intellectual-property, confidentiality, and publication obligations.

Where an exception materially affects intended use, Technical Maturity, or Operational Readiness, the limitation should be reflected in the project record.

An exception does not justify exposing credentials, unauthorised data, confidential material, or unsafe privileged functionality.

Exceptions should be reconsidered when project scope, risk, or usage changes.

---

## 21. Continuous Improvement

Quality standards should evolve as the Lab's projects, tools, and technical practices develop.

The maintainer may review and improve these standards based on:

- project experience;
- technical findings;
- recurring defects;
- security incidents;
- evaluation results;
- contributor feedback;
- changes in relevant technologies; and
- new accessibility or engineering requirements.

Quality improvement should focus on practical outcomes.

The objective is not to maximise the number of tools, tests, or processes used. It is to improve the reliability, clarity, maintainability, accessibility, and integrity of the work produced.

Changes to quality expectations should be communicated through the applicable documentation and project records.

---

## 22. Relationship with Other Documents

This document establishes the Lab's general engineering and quality expectations. It should be read alongside the specialist documents that define related responsibilities and procedures.

| Document | Primary responsibility |
|---|---|
| `README.md` | Lab identity, mission, scope, and public overview |
| `LAB-CHARTER-v2.0.md` | Foundational principles and institutional direction |
| `GOVERNANCE-v2.0.md` | Decision-making authority and responsibilities |
| `PROJECT-LIFECYCLE-v2.0.md` | Lifecycle stages and canonical Project Status definitions |
| `PROJECT-TEMPLATE-v2.0.md` | Standard structure for project records and assessment fields |
| `RESEARCH-METHODOLOGY-v2.0.md` | Research design, experimental methods, and evidence practices |
| `PUBLICATION-POLICY-v2.0.md` | Publication Classification, publication decisions, confidentiality, and release approval |
| `CONTRIBUTING-v2.0.md` | Contribution workflow and contributor responsibilities |
| `SECURITY-v2.0.md` | Security practices, vulnerability reporting, and incident handling |
| `CODE-OF-CONDUCT-v2.0.md` | Collaboration expectations and conduct reporting |
| `RESPONSIBLE-AI-v2.0.md` | AI-specific principles, risk classification, oversight, and restrictions |

The authoritative ownership of a subject remains with its specialist document.

Where this document summarises a subject covered by another policy, the summary must not be interpreted as replacing or modifying that policy.

If a project-specific document appears to conflict with a Lab policy, the conflict should be raised with the maintainer rather than resolved by silently adopting a weaker requirement.

---

## 23. Policy Review and Amendments

This document may be revised as the Lab's technical practices, project scope, and operating model evolve.

The Founder and Maintainer is responsible for approving and documenting changes in accordance with `GOVERNANCE-v2.0.md`.

Revisions should:

- preserve the distinction between Technical Maturity, Operational Readiness, Project Status, Lifecycle Stage, and publication decisions;
- maintain clear ownership boundaries with specialist policies;
- remain proportionate to the Lab's actual operating capacity;
- avoid unsupported legal, security, or compliance claims;
- identify material changes to requirements; and
- preserve an appropriate revision history.

A revision to this document does not automatically change the status, maturity, readiness, or publication decision of an existing project. Relevant project records should be reassessed where the change materially affects them.

---

## 24. Closing Principle

Quality is not a single technical achievement.

It is the coherence between what a project intends to do, how it is built, how it behaves, how it is evaluated, how it is maintained, and how its results are presented.

A rigorous prototype can be valuable without being production-ready. A polished release can still have technical limitations. An ambitious system can remain unfinished despite its sophistication.

The Lab therefore aims to make quality visible through deliberate engineering, meaningful evaluation, responsible use of technology, clear documentation, and honest communication.

**Build with intention. Test with rigor. Document with clarity. Improve continuously.**
