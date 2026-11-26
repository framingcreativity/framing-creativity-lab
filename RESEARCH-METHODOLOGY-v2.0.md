# Framing Creativity Lab — Research Methodology

**Document ID:** FCL-METH-001  
**Version:** 2.0  
**Status:** Draft for Maintainer Review  
**Effective Date:** Pending approval  
**Maintainer:** J-ART  
**Repository:** Framing Creativity Lab  
**Applies to:** Research, experiments, technical investigations, prototypes, and evaluation activities conducted under Framing Creativity Lab.

---

## 1. Purpose

This document establishes the research methodology used by Framing Creativity Lab.

It defines the principles, processes, methods, and evaluation practices used to investigate questions, formulate hypotheses, conduct experiments, analyse results, interpret findings, and document conclusions.

Its purpose is to establish a consistent approach to research while allowing sufficient flexibility for different disciplines, technologies, and experimental objectives.

The methodology supports:

- Independent technical research.
- Artificial intelligence experimentation.
- Software and systems investigation.
- Creative technology research.
- Computational and generative experimentation.
- Digital product exploration.
- Technical prototyping.
- Comparative technology evaluation.
- Methodological research.
- Interdisciplinary investigation.
- Qualitative and quantitative studies.
- Experimental design and evaluation.

The document provides a common framework rather than prescribing a single research technique.

Individual investigations may require different methods depending on their objectives, complexity, uncertainty, risks, and available resources.

**The objective is not to standardise every experiment. It is to make every substantial investigation understandable, purposeful, evaluable, traceable, and appropriately documented.**

---

## 2. Research Philosophy

Framing Creativity Lab approaches research as a structured process of exploration and evaluation.

Research begins with a question, not with an assumption that a particular technology is the right solution.

The Lab recognises that meaningful investigation may require combining different perspectives:

- Scientific and technical reasoning.
- Creative and exploratory thinking.
- Engineering and implementation.
- Human interpretation and evaluation.
- Comparative and critical analysis.
- Empirical observation.
- Methodological reflection.

Technology should be examined through both its capabilities and its limitations.

A successful experiment is not necessarily one that confirms its initial hypothesis. An experiment that reveals an incorrect assumption, exposes a limitation, or demonstrates the inadequacy of an approach may produce equally valuable knowledge.

### 2.1 Core Principles

#### Curiosity Before Conclusion

Research should begin with a genuine question and remain open to unexpected findings.

#### Hypothesis Before Implementation

Where appropriate, establish what is being investigated before selecting tools or writing code.

#### Evidence Before Claims

Conclusions should be supported by observations, measurements, tests, sources, or clearly identified reasoning.

#### Exploration Before Commitment

Promising approaches should be examined before they become fixed technical, methodological, or architectural decisions.

#### Reproducibility Before Assumption

Methods and configurations should be documented sufficiently for results to be understood and repeated where practical.

#### Limitations as Findings

Failures, constraints, anomalies, and inconclusive outcomes must be recognised as part of the research record.

#### Documentation as Part of Research

Documentation should accompany the investigation rather than being reconstructed only after implementation.

#### Human Judgement Remains Essential

Automated tools, AI systems, and quantitative measurements support research. They do not eliminate the need for critical interpretation.

#### Intellectual Honesty

The research record must distinguish what is known, what has been observed, what has been inferred, and what remains uncertain.

### 2.2 Research Is Not Product Development Alone

A research investigation may produce a product, prototype, demonstration, technical report, experimental dataset, methodological framework, or no functional artefact at all.

The value of the investigation is not determined exclusively by whether it produces a finished application.

A negative result may be more informative than an implementation that works under narrow conditions but does not support the original hypothesis.

---

## 3. Research Scope and Classification

Before beginning an investigation, its nature and scope should be established.

Research activities may fall into one or more of the following categories.

### 3.1 Exploratory Research

Exploratory research investigates a subject where the relevant questions, approaches, or possibilities have not yet been sufficiently established.

Objectives may include:

- Understanding an emerging technology.
- Identifying potential applications.
- Discovering relevant technical constraints.
- Investigating unfamiliar methods.
- Identifying knowledge gaps.
- Formulating questions for future experiments.
- Exploring relationships between different disciplines.

Exploratory research does not necessarily require a formal hypothesis.

Its findings should distinguish observations from speculation.

### 3.2 Experimental Research

Experimental research tests a defined proposition through a structured implementation or controlled investigation.

Objectives may include:

- Evaluating a particular technique.
- Comparing implementation approaches.
- Testing model behaviour.
- Measuring performance.
- Investigating system responses.
- Examining cause-and-effect relationships where the design supports such conclusions.

Experimental research should define its variables, conditions, and evaluation criteria as precisely as reasonably possible.

### 3.3 Applied Research

Applied research investigates how existing knowledge or technologies can address a practical problem.

Examples include:

- Developing an AI-assisted workflow.
- Improving an interaction pattern.
- Evaluating an automation strategy.
- Testing an application architecture.
- Investigating a practical implementation of a technical concept.
- Evaluating a proposed digital experience.

The intended application should not predetermine the research conclusion.

### 3.4 Comparative Research

Comparative research compares multiple technologies, methods, models, or implementations under defined conditions.

The comparison should establish:

- What is being compared.
- Why the comparison is relevant.
- Which conditions are shared.
- Which variables differ.
- How results are measured.
- Which constraints affect comparability.
- Which conclusions the comparison can legitimately support.

Comparisons should avoid declaring one approach universally superior when results only support a narrower conclusion.

### 3.5 Methodological Research

Methodological research investigates how a process, framework, or research method can be designed, improved, or evaluated.

Examples include:

- AI evaluation methodologies.
- Prompt testing frameworks.
- Documentation standards.
- Development workflows.
- Human-in-the-loop validation methods.
- Design-to-development processes.
- Reproducibility methods.
- Technical evaluation frameworks.

### 3.6 Creative and Interdisciplinary Research

Creative and interdisciplinary research investigates the relationship between computation, interaction, perception, creative practice, and emerging technologies.

Examples include:

- Generative visual systems.
- Algorithmic composition.
- Interactive narratives.
- Computational typography.
- AI-assisted creative processes.
- Experimental interfaces.
- Human–machine collaboration.
- Procedural and generative environments.
- Multimodal creative systems.

Not every creative investigation requires quantitative measurement.

Qualitative observations, documented behaviours, interaction studies, comparative visual evaluation, and critical interpretation may be more appropriate.

### 3.7 Research Category Versus Project Classification

Research categories describe the nature of an investigation.

They do not replace the canonical project fields defined by the Lab.

In particular, a research category must not be treated as:

- A Lifecycle Stage.
- A Project Status.
- A Technical Maturity level.
- An Operational Readiness level.
- A Publication Classification.
- A Publication Status.
- An AI Risk Classification.

The six project fields remain governed by their respective documents. AI Risk Classification remains independently governed by `RESPONSIBLE-AI-v2.0.md`.

---

## 4. The Research Lifecycle

The standard Framing Creativity Lab research process follows nine stages.

**Question → Context → Hypothesis → Design → Experiment → Evaluation → Interpretation → Documentation → Review**

The stages provide a common structure. Some may be repeated, combined, or adapted according to the nature of the research.

This research lifecycle is distinct from the project lifecycle defined in `PROJECT-LIFECYCLE-v2.0.md`.

The research lifecycle describes how an investigation is conducted. The project lifecycle describes the broader progression and state of a Lab project.

### 4.1 Stage 01 — Identify the Research Question

Every substantial investigation should begin with a clearly formulated question.

A useful research question should:

- Identify the subject being investigated.
- Establish the relevant context.
- Define the problem or uncertainty.
- Be sufficiently specific to guide an investigation.
- Be appropriate to the available resources and methods.
- Allow a meaningful form of evaluation.

Weak research question:

> Can artificial intelligence improve digital products?

More focused research question:

> Under which conditions can an LLM-based interface reduce the time required to complete a structured information-retrieval task without significantly reducing answer accuracy?

The second formulation identifies an observable task and introduces evaluation criteria.

The research question may evolve when the initial investigation reveals that the problem was incorrectly framed.

A material change to the question should be documented rather than silently substituted after results have been observed.

### 4.2 Stage 02 — Establish the Research Context

Before designing an experiment, establish what is already known.

Relevant activities include:

- Reviewing technical documentation.
- Examining relevant scientific literature.
- Investigating existing implementations.
- Comparing established methods.
- Identifying relevant standards.
- Examining known limitations.
- Identifying conflicting findings.
- Assessing the reliability of available sources.
- Identifying knowledge gaps.

#### Source Quality

Sources should be evaluated according to their relevance, authority, recency, methodology, and verifiability.

Preferred sources may include:

- Peer-reviewed scientific publications.
- Academic research institutions.
- Official technical documentation.
- Standards organisations.
- Original technical specifications.
- Reputable research reports.
- Public implementation repositories.
- Reproducible experimental studies.
- Official datasets and technical benchmarks.

Community discussions and informal publications may provide useful observations, but should not automatically be treated as authoritative evidence.

#### Source Traceability

Important factual claims should be traceable to their original source.

Research notes should record, where applicable:

- Author or organisation.
- Title.
- Publication or release date.
- Source URL or identifier.
- Access date.
- Relevant section or page.
- Reason for including the source.
- Relevant methodological limitations.

Unverified claims must be labelled accordingly.

#### Source Interpretation

A source should not be cited as support for a claim that it does not actually establish.

Research should distinguish:

- What the source explicitly states.
- What the source demonstrates.
- What the researcher infers.
- What remains unverified.
- Whether the source is current enough for the relevant claim.

The existence of a citation does not automatically establish the validity of an interpretation.

### 4.3 Stage 03 — Formulate the Hypothesis

Where appropriate, translate the research question into a testable proposition.

A useful hypothesis should identify:

- The expected relationship or behaviour.
- The relevant conditions.
- The expected outcome.
- The means by which the outcome will be evaluated.

Example:

> Under identical input and evaluation conditions, structured prompting will produce a higher proportion of valid outputs than an unstructured instruction.

The experiment must define what constitutes a valid output before testing begins.

#### Hypothesis Types

Depending on the investigation, a project may use:

- A directional hypothesis.
- A non-directional hypothesis.
- A comparative hypothesis.
- A technical feasibility hypothesis.
- A design hypothesis.
- An exploratory proposition.

Not every investigation needs a null hypothesis or formal statistical testing.

The methodology should reflect the type of question being asked.

#### Hypothesis Discipline

The initial hypothesis should be recorded before results are interpreted.

This reduces the risk of changing the research question retrospectively to fit observed outcomes.

Where the hypothesis changes materially, record:

- The original proposition.
- The revised proposition.
- The reason for the change.
- The evidence or observation that prompted the revision.
- The stage at which the change occurred.

Exploratory changes are legitimate when they are documented honestly.

### 4.4 Stage 04 — Design the Experiment

The experiment design translates the hypothesis into a practical investigation.

The design should establish:

- Objective.
- Scope.
- Method.
- Variables.
- Tools and technologies.
- Test conditions.
- Input data.
- Expected outputs.
- Evaluation criteria.
- Known constraints.
- Risks and limitations.
- Repetition requirements.
- Relevant data permissions.

#### Variables

Where relevant, distinguish between:

**Independent Variables**

Factors deliberately changed during the experiment.

**Dependent Variables**

Outcomes being observed or measured.

**Controlled Variables**

Conditions maintained consistently to support meaningful comparison.

**External Variables**

Factors that may influence results but cannot necessarily be controlled.

For qualitative or creative research, these categories may be adapted to reflect the nature of the investigation.

#### Baselines

Comparative experiments should establish an appropriate baseline whenever practical.

A baseline provides a reference against which the proposed approach can be evaluated.

The baseline should be documented, including why it is relevant and what limitations affect the comparison.

#### Evaluation Criteria

Evaluation criteria must be selected before analysing the results whenever possible.

Criteria may include:

- Accuracy.
- Completion rate.
- Response time.
- Resource consumption.
- Output consistency.
- Functional correctness.
- Usability.
- Accessibility.
- Visual coherence.
- Reproducibility.
- Human preference.
- Qualitative observations.
- Error frequency.
- Cost.
- Reliability.

The selected criteria should correspond to the original research question.

### 4.5 Stage 05 — Conduct the Experiment

The experiment should be carried out according to the documented design.

Record relevant information such as:

- Execution date.
- Environment.
- Software versions.
- Model versions.
- Configuration.
- Inputs.
- Test cases.
- Outputs.
- Observations.
- Deviations from the original plan.
- Unexpected behaviour.
- Manual interventions.
- Relevant external conditions.

Where practical, preserve the original experimental conditions and distinguish exploratory adjustments from formal test runs.

Do not silently discard unexpected results or unsuccessful attempts when they materially affect interpretation.

### 4.6 Stage 06 — Evaluate the Results

Results should be evaluated against the defined criteria.

This may involve:

- Quantitative analysis.
- Qualitative analysis.
- Comparative evaluation.
- Functional testing.
- Performance measurements.
- Human assessment.
- Visual or behavioural inspection.
- Statistical analysis where justified.

The evaluation should identify:

- What worked.
- What failed.
- What changed.
- What was unexpected.
- Whether the hypothesis was supported.
- Which limitations remain.
- Whether additional testing is required.
- Whether the results are sufficiently reliable to support a conclusion.

A successful implementation does not automatically establish that the original hypothesis was correct.

### 4.7 Stage 07 — Interpret the Findings

Interpretation connects the observations to the original research question.

It should distinguish between:

- Directly observed results.
- Measured results.
- Reasonable interpretations.
- Assumptions.
- Speculation.
- Unresolved questions.
- External explanations that have not been tested.

Conclusions must remain proportionate to the evidence.

A small experimental sample should not be presented as proof of general behaviour.

A single successful AI response should not be interpreted as evidence of model reliability.

A visual prototype should not be presented as proof of production feasibility.

A measured correlation should not automatically be presented as a causal relationship.

### 4.8 Stage 08 — Document the Research

Document the process while relevant information remains available.

The research record should explain:

- Why the investigation was conducted.
- How it was designed.
- What was implemented.
- Which conditions were used.
- What was observed.
- How results were evaluated.
- What conclusions were reached.
- What remains uncertain.
- Which limitations affect interpretation.

Documentation must preserve methodological context, not merely final outcomes.

### 4.9 Stage 09 — Review and Next Steps

The investigation should conclude with a review.

Possible outcomes include:

- Accept the findings.
- Reject the original hypothesis.
- Refine the hypothesis.
- Repeat the experiment.
- Expand the investigation.
- Change the method.
- Develop a prototype.
- Conduct further validation.
- Discontinue the approach.
- Archive the research.

The final decision should be documented.

These research decisions do not create additional Project Status values.

---

## 5. Experiment Design Standards

The quality of an experiment depends on the suitability of its design.

### 5.1 Research Objective

The objective must be clearly stated.

Avoid combining multiple unrelated questions into a single experiment unless their relationship is part of the investigation.

A substantial investigation should identify what it intends to establish and what would count as an informative result.

### 5.2 Scope Definition

Define what the investigation includes and excludes.

Scope should identify:

- Subjects or systems under examination.
- Relevant technical environment.
- Included functionality.
- Excluded functionality.
- Assumptions.
- Resource constraints.
- Expected depth of investigation.
- Intended audience or context.
- Important ethical or publication boundaries.

### 5.3 Test Conditions

Conditions should be documented sufficiently to interpret the results.

For software experiments, this may include:

- Operating system.
- Runtime environment.
- Programming language version.
- Framework versions.
- Hardware configuration.
- Network conditions.
- External services.
- Relevant environment variables.
- Database or storage configuration.

For AI experiments, additional model-specific conditions are required.

### 5.4 Input Definition

Input data and test cases should be characterised.

Document:

- Origin.
- Structure.
- Format.
- Relevant characteristics.
- Selection criteria.
- Known limitations.
- Permissions or licence conditions.
- Relevant transformations.
- Exclusions and filtering rules.

Inputs must be appropriate for the research question.

### 5.5 Repetition

Repeat experiments when necessary to assess consistency.

The appropriate number of repetitions depends on the research question, the variability of the system, the evaluation method, and the cost of testing.

For non-deterministic systems, a single run is generally insufficient to characterise output consistency.

Where repetition is not practical, the limitation should be recorded.

### 5.6 Deviations

Any material deviation from the experiment design must be recorded.

This includes:

- Modified test conditions.
- Changed inputs.
- Updated model versions.
- Different evaluation criteria.
- Failed execution.
- Environmental changes.
- Manual interventions.
- Changes to the hypothesis.
- Excluded observations.
- Changes to the experimental population or sample.

The original plan and the actual execution should remain distinguishable.

### 5.7 Experiment Separation

Where practical, distinguish exploratory runs from formal evaluation runs.

Exploratory runs may be used to improve a method or discover failure conditions.

Formal evaluation should use documented conditions and criteria that are not changed retrospectively merely to improve the apparent result.

If formal conditions change, record the change and its rationale.

### 5.8 Experimental Integrity

The researcher should preserve a sufficiently accurate record of the work performed.

Do not fabricate, selectively alter, or omit material observations to create a more favourable conclusion.

Where an experiment cannot be completed as planned, document what was actually performed and what remains incomplete.

---

## 6. Artificial Intelligence Research Methodology

AI experimentation requires particular attention to model variability, configuration, evaluation, data handling, and the interaction between model outputs and application behaviour.

The Lab treats AI systems as technical components whose behaviour must be investigated within a defined context.

An AI model cannot be evaluated independently of its inputs, prompts, configuration, integration, data, and intended task.

AI-specific principles, risk classifications, human oversight, and restrictions are governed by `RESPONSIBLE-AI-v2.0.md`.

### 6.1 AI Research Objectives

An AI experiment should identify what aspect of the system is being investigated.

Possible objectives include:

- Output accuracy.
- Instruction following.
- Reasoning performance.
- Information retrieval.
- Structured data generation.
- Classification.
- Summarisation.
- Code generation.
- Tool usage.
- Workflow automation.
- Multimodal interpretation.
- User interaction.
- Response consistency.
- Cost and latency.
- Safety and reliability.
- Human evaluation.
- Robustness under unexpected inputs.

Multiple objectives may be investigated, but each should have an appropriate evaluation method.

### 6.2 Model Identification

Where relevant, record:

- Model provider.
- Model name.
- Model version or identifier.
- Access method.
- API or interface version.
- Access date.
- Relevant configuration.
- Known provider-side constraints.
- Important model limitations.

Model identifiers and versions should be recorded accurately.

Do not invent unavailable version information.

If a provider changes a model without exposing a stable version identifier, document that limitation.

### 6.3 Prompt Documentation

Prompts are part of the experimental configuration.

Where a prompt materially affects results, document:

- Prompt identifier.
- Prompt version.
- System instructions, where publication is authorised.
- User input.
- Output constraints.
- Examples or contextual material.
- Relevant parameters.
- Intended task.
- Changes between tested versions.

Prompt changes should be versioned where comparative evaluation is required.

If prompts contain confidential or restricted information, they must not be transferred to the public repository.

### 6.4 AI Model Configuration

Record relevant parameters when available:

- Temperature.
- Maximum output tokens.
- Top-p.
- Sampling configuration.
- Seed.
- Tool configuration.
- Context window.
- Structured output requirements.
- Retrieval settings.
- Model-specific parameters.
- Provider-specific settings.

Some providers expose only a subset of these options.

Unavailable parameters should be omitted or identified as unavailable rather than assumed.

### 6.5 AI Input and Output Evaluation

AI outputs should be evaluated against explicit criteria.

Possible criteria include:

**Correctness**

Does the output contain accurate information or produce the intended result?

**Completeness**

Does it address the relevant requirements?

**Instruction Adherence**

Does it follow the requested constraints?

**Consistency**

Does it maintain acceptable behaviour across repeated executions?

**Relevance**

Does it address the intended task?

**Robustness**

Does it behave appropriately when inputs vary or contain ambiguity?

**Safety**

Does it avoid unacceptable or harmful outputs in the tested context?

**Efficiency**

Are latency and resource consumption appropriate?

**Usability**

Can the intended user understand and use the result?

Not every experiment requires every criterion.

The evaluation criteria should match the use case.

### 6.6 Evaluation Datasets and Test Cases

AI evaluations should use a defined set of test cases whenever practical.

A useful test collection may include:

- Typical inputs.
- Edge cases.
- Ambiguous requests.
- Incomplete information.
- Invalid inputs.
- Adversarial inputs where relevant.
- Expected output characteristics.
- Known failure cases.
- Relevant negative examples.

Test sets should be selected with awareness of representativeness and potential bias.

Where a reference answer exists, its origin, accuracy, and validation should be documented.

Evaluation data must be used in accordance with its classification, permitted purpose, licence, and applicable restrictions.

### 6.7 Reproducibility and Variability

AI outputs may vary between executions.

Exact reproduction may be impossible because of:

- Model updates.
- Provider-side infrastructure changes.
- Sampling behaviour.
- Non-deterministic operations.
- Hidden implementation details.
- Changes in retrieval or contextual information.
- Changes in safety or system configurations.

The research record should distinguish:

- Exact reproducibility.
- Approximate reproducibility.
- Configuration-level reproducibility.
- Non-reproducible external behaviour.

Where possible, retain representative inputs and outputs.

Do not present one successful execution as a complete characterisation of the system.

### 6.8 Human Evaluation

Human evaluation may be necessary when quality cannot be adequately determined through automated metrics.

This is particularly relevant for:

- Creative outputs.
- Visual quality.
- Interaction quality.
- Natural-language interpretation.
- Perceived usefulness.
- Relevance.
- Aesthetic coherence.
- Contextual appropriateness.

Human evaluation should document:

- The criteria used.
- The evaluation procedure.
- Relevant evaluator characteristics where appropriate.
- The number of evaluations.
- The method for handling disagreement.
- Any limitations.

Where feasible, reduce evaluator bias through consistent assessment procedures.

### 6.9 AI Failure Analysis

Failures are important research observations.

Potential failure categories include:

- Hallucination.
- Incorrect reasoning.
- Unsupported factual claims.
- Instruction drift.
- Format violations.
- Context loss.
- Inconsistent outputs.
- Tool-use errors.
- Retrieval failures.
- Refusal failures.
- Prompt injection.
- Security weaknesses.
- Data leakage.
- Unintended actions.

A documented failure should identify the conditions under which it occurred and whether the failure was reproducible.

### 6.10 AI Safety and Responsible Evaluation

Experiments must respect applicable safety, privacy, security, and publication requirements.

AI systems should not be assumed to provide reliable protection merely because a safety mechanism is present.

Where an experiment investigates sensitive behaviour, appropriate safeguards and publication restrictions must be established before testing.

The AI Risk Classification A0–A4 must be assigned where required by `RESPONSIBLE-AI-v2.0.md`.

AI Risk Classification must not be confused with Publication Classification P0–P3.

---

## 7. Software and Systems Research

Technical investigations involving software systems should follow an implementation-oriented methodology.

### 7.1 Architecture Investigation

Document:

- System objective.
- Relevant components.
- Component relationships.
- Data flow.
- External integrations.
- Configuration.
- Runtime dependencies.
- Architectural constraints.
- Important technical assumptions.
- Relevant failure boundaries.

Diagrams may be used to communicate complex structures.

Architecture descriptions should distinguish implemented components from proposed or conceptual elements.

### 7.2 Implementation Comparisons

When comparing implementation strategies, establish consistent evaluation criteria.

Possible dimensions include:

- Functional suitability.
- Complexity.
- Maintainability.
- Performance.
- Scalability.
- Compatibility.
- Security.
- Development effort.
- Operational cost.
- Dependency requirements.
- Extensibility.
- Reproducibility.

No single approach should be declared superior without identifying the criteria under which it performs better.

### 7.3 Software Testing

Depending on the project, appropriate tests may include:

- Unit tests.
- Integration tests.
- End-to-end tests.
- Regression tests.
- Performance tests.
- Compatibility tests.
- Accessibility tests.
- Security tests.
- User acceptance tests.
- Failure and recovery tests.

The presence and scope of tests must be described accurately.

### 7.4 Performance Evaluation

Performance studies should document:

- Hardware and environment.
- Software versions.
- Dataset or workload.
- Test duration.
- Number of runs.
- Measurement method.
- Relevant environmental conditions.
- Important resource constraints.

Measurements should be interpreted in context.

A benchmark from one environment cannot automatically establish performance across other systems.

### 7.5 System Behaviour

Where relevant, evaluate:

- Input handling.
- State transitions.
- Error handling.
- Resource consumption.
- Dependency failures.
- Network behaviour.
- Data persistence.
- Concurrent operations.
- Recovery behaviour.
- Permission boundaries.

The research should identify the conditions under which observed behaviour is expected to remain valid.

---

## 8. Creative Technology and Qualitative Research

Creative and interdisciplinary experiments require a methodology appropriate to their subject.

The Lab recognises that not all valuable outcomes can be reduced to numerical measurements.

### 8.1 Creative Hypothesis

A creative investigation may begin with a conceptual proposition.

Examples:

- How does delayed interaction change the perception of a digital narrative?
- Can generative constraints produce more coherent visual compositions?
- How does dynamic typography affect the interpretation of text?
- Can a computational system introduce meaningful variation into an interactive experience?
- How does adaptive sound influence the perception of an interactive environment?
- Can an algorithmic process create a recognisable visual language?

The proposition should be documented in a manner that makes the intention understandable.

### 8.2 Experimental Framework

Creative experiments may investigate:

- Form.
- Behaviour.
- Interaction.
- Timing.
- Perception.
- Composition.
- Variability.
- Interpretation.
- User response.
- Spatial or temporal relationships.
- Generative constraints.
- Human–machine collaboration.

The implementation should preserve enough information to explain how the experience was constructed.

### 8.3 Qualitative Evaluation

Relevant approaches may include:

- Structured observation.
- Interaction analysis.
- Comparative visual inspection.
- User feedback.
- Expert assessment.
- Reflective analysis.
- Documentation of emergent behaviour.
- Comparative interpretation.
- Recorded creative decisions.

Where subjective assessment is used, its criteria and limitations should be acknowledged.

### 8.4 Creative Reproducibility

Perfect visual or experiential reproducibility may not always be necessary or possible.

The research should nevertheless document relevant parameters, constraints, assets, algorithms, configurations, and creative decisions.

The objective is to make the creative process understandable even when every outcome cannot be reproduced identically.

### 8.5 Human Interpretation

Human interpretation may be an essential component of the research.

The research record should identify where conclusions depend on subjective judgement and avoid presenting personal preference as universal evidence.

### 8.6 Creative Outcome Versus Technical Validation

A successful creative experience does not automatically demonstrate technical reliability.

Likewise, technical consistency does not automatically establish creative quality.

The investigation should evaluate each dimension according to its own criteria.

---

## 9. Data Collection and Management

Data handling must be appropriate to the research objective and publication scope.

### 9.1 Data Sources

Possible sources include:

- Public datasets.
- Synthetic datasets.
- Original experimental data.
- Authorised APIs.
- Public technical documentation.
- Licensed research datasets.
- Generated outputs.
- Structured observations.
- User evaluation records, where appropriately authorized.

Data origins must be documented where material to the research.

### 9.2 Data Suitability

Evaluate:

- Relevance.
- Quality.
- Completeness.
- Representativeness.
- Potential bias.
- Provenance.
- Licence conditions.
- Privacy implications.
- Processing restrictions.
- Suitability for the intended analysis.

The availability of a dataset does not automatically establish permission to use it.

### 9.3 Data Integrity

Original data should be preserved when appropriate and permitted.

Transformations should be documented, including:

- Cleaning.
- Filtering.
- Normalisation.
- Aggregation.
- Annotation.
- Sampling.
- Deduplication.
- Exclusion rules.
- Reformatting.
- Feature extraction.

Where a transformation materially affects the results, retain enough information to understand how it was performed.

### 9.4 Data Versioning

When data changes materially between experiments, the relevant version should be identifiable.

Where appropriate, record:

- Dataset identifier.
- Version.
- Date of retrieval.
- Source reference.
- Checksums.
- Relevant transformations.
- Selection criteria.

### 9.5 Data Retention

Data should be retained only when necessary and permitted.

Private, personal, confidential, or restricted data must not be included in public research assets without an appropriate basis and authorization.

### 9.6 Canonical Data Classification

Research data must follow the four canonical classifications defined in `PUBLICATION-POLICY-v2.0.md`:

- Public.
- Internal.
- Confidential.
- Restricted.

Personal information and sensitive information are data characteristics, not additional values in the four-level classification vocabulary.

Personal information should be classified at least as Confidential. Sensitive personal information and information subject to stricter restrictions should be classified as Restricted.

### 9.7 External Data Processing

Where research involves external AI services, APIs, or data platforms, document relevant processing conditions.

This may include:

- Information transmitted.
- Processing purpose.
- Provider or recipient.
- Data classification.
- Retention conditions.
- Authorization and usage rights.
- Relevant access restrictions.

Do not submit confidential or restricted research data to external services without the necessary authorization and safeguards.

---

## 10. Analysis and Interpretation

Analysis must be aligned with the research question and the type of evidence collected.

### 10.1 Quantitative Analysis

Quantitative methods may include:

- Descriptive statistics.
- Frequency analysis.
- Comparative measurements.
- Error rates.
- Response distributions.
- Performance measurements.
- Confidence intervals where appropriate.
- Statistical testing where justified.
- Correlation analysis.
- Timing and resource measurements.

The selected method should be proportionate to the quality and quantity of available data.

### 10.2 Qualitative Analysis

Qualitative methods may include:

- Thematic analysis.
- Structured observations.
- Comparative interpretation.
- Content analysis.
- Behavioural analysis.
- Expert assessment.
- Reflective commentary.
- Interaction analysis.
- Case-based interpretation.

Qualitative findings should identify their basis and avoid presenting subjective interpretation as objective measurement.

### 10.3 Mixed-Method Analysis

Some investigations benefit from combining quantitative and qualitative evidence.

For example, an interface experiment may measure task completion time while also recording user observations.

The relationship between the two forms of evidence should be explained.

Quantitative results should not automatically override qualitative observations when both are relevant to the research question.

### 10.4 Statistical Caution

Statistical significance should not be confused with practical importance.

A numerical difference may exist without representing a meaningful improvement.

Small samples, biased selection, measurement error, and uncontrolled conditions may limit the reliability of conclusions.

Where statistical methods are used, their assumptions and limitations should be documented.

### 10.5 Negative and Inconclusive Results

Research records should preserve relevant negative and inconclusive outcomes.

Do not remove failures from a report merely because they do not support the initial hypothesis.

The absence of a demonstrated effect is not automatically proof that no effect exists.

### 10.6 Causal Interpretation

Causal claims require an appropriate research design.

Observational evidence or correlation alone does not establish causation.

Where causal conclusions cannot be supported, describe the observed relationship without overstating its meaning.

### 10.7 Interpretation Boundaries

A conclusion should identify the population, system, configuration, or conditions to which it applies.

Do not generalise beyond the tested scope without additional evidence.

---

## 11. Reproducibility and Traceability

Reproducibility supports technical understanding and independent evaluation.

The Lab aims to make its experiments reproducible to the extent permitted by their nature, dependencies, and data restrictions.

### 11.1 Reproduction Requirements

Where practical, document:

- Source code.
- Environment.
- Runtime.
- Dependencies.
- Configuration.
- Input data.
- Test cases.
- Execution steps.
- Expected outputs.
- Evaluation method.
- Relevant model or provider information.
- Known reproduction limitations.

### 11.2 Experiment Identification

Substantial experiments should receive a unique identifier.

Recommended format:

`FCL-EXP-YYYY-NNN`

Example:

`FCL-EXP-2026-001`

Identifiers should be unique within the Lab's experiment records.

### 11.3 Version Tracking

Record relevant versions of:

- Source code.
- Dependencies.
- Models.
- Datasets.
- Prompts.
- Configuration.
- External APIs.
- Evaluation procedures.
- Research documentation.

Use commit identifiers or tagged releases when they support traceability.

### 11.4 Research Records

Maintain sufficient records to distinguish:

- Original experiment design.
- Actual execution.
- Modified conditions.
- Intermediate results.
- Failed attempts.
- Final interpretation.
- Subsequent reassessment.

### 11.5 Limits of Reproduction

Where exact reproduction is impossible, explain why.

This may include:

- Unavailable infrastructure.
- Changing external services.
- Non-deterministic models.
- Restricted data.
- Provider-side configuration changes.
- Unavailable historical dependencies.
- Environmental differences.

The limitation must be explicit rather than hidden.

### 11.6 Reproducibility and Publication

Reproducibility does not authorize the disclosure of confidential information, proprietary source code, restricted datasets, or private configurations.

Where full reproduction is not possible publicly, provide the information that can legitimately be shared and identify the remaining restrictions.

---

## 12. Research Quality and Evidence Standards

Research conclusions should be supported by evidence appropriate to their claims.

### 12.1 Evidence Categories

The following categories provide an internal framework for describing the type and maturity of research evidence.

| Category | Description |
|---|---|
| E0 — Conceptual | A proposal or theoretical proposition without experimental support. |
| E1 — Observational | An observation or exploratory finding. |
| E2 — Demonstrated | A functional example or initial experiment. |
| E3 — Evaluated | Results assessed against defined criteria. |
| E4 — Repeated | Relevant results reproduced across repeated conditions. |
| E5 — Independently Corroborated | Findings supported by a separate implementation, evaluator, or independent investigation. |

These are internal descriptive categories, not a universal scientific evidence hierarchy.

A project may have different evidence categories for different claims.

Independent corroboration must never be claimed when the evaluation was conducted only by the original author.

### 12.2 Evidence Categories Are Not Project Maturity

The E0–E5 categories describe the available research evidence.

They must not be confused with:

- Technical Maturity.
- Operational Readiness.
- Lifecycle Stage.
- Project Status.
- Publication Classification.
- Publication Status.
- AI Risk Classification.

For example, E4 evidence does not automatically establish that a project is operationally ready or validated in every relevant context.

Likewise, a project may contain a validated technical component while a separate research claim remains supported only by preliminary evidence.

Technical Maturity remains governed by `QUALITY-STANDARDS-v2.0.md`.

### 12.3 Claim Discipline

The research report should distinguish:

- What was proposed.
- What was implemented.
- What was tested.
- What was observed.
- What was measured.
- What was interpreted.
- What was concluded.

Claims must not exceed the evidence available.

### 12.4 Evidence Limitations

Document important limitations such as:

- Sample size.
- Selection bias.
- Measurement uncertainty.
- External dependencies.
- Model variability.
- Environmental constraints.
- Subjective assessment.
- Missing baseline comparisons.
- Limited test conditions.
- Incomplete source verification.

### 12.5 Confidence

Where useful, findings may be described as:

- Preliminary.
- Indicative.
- Moderately supported.
- Strongly supported within the tested scope.
- Inconclusive.

Confidence descriptions should be explained rather than used as decorative labels.

### 12.6 Independent Corroboration

Independent corroboration requires a meaningful degree of separation from the original investigation.

Depending on the claim, this may involve:

- An independent evaluator.
- A separate implementation.
- A reproduction by another researcher.
- A distinct dataset or evaluation environment.
- A separate analysis of the original evidence.

A second review by the original author does not, by itself, establish independent corroboration.

### 12.7 Evidence Preservation

Where practical, retain relevant evidence such as:

- Test results.
- Measurement records.
- Experimental configurations.
- Source references.
- Evaluation reports.
- Relevant output samples.
- Reproducibility instructions.

Evidence must be retained and published only where the applicable rights, privacy, and confidentiality conditions permit.

---

## 13. Ethics, Privacy, and Responsible Research

Research must be conducted with appropriate consideration for human participants, data subjects, third parties, and wider impacts.

### 13.1 Respect for Individuals

Experiments involving people should respect their privacy, autonomy, and informed participation.

Participation must not be misrepresented or obtained through deceptive practices.

The nature and purpose of participation should be explained in an appropriate manner.

### 13.2 Personal Data

Personal information should not be collected unnecessarily.

Any processing must have an appropriate legal basis and respect applicable obligations.

Research documentation should identify relevant data handling without exposing personal information.

### 13.3 Human Evaluation

Where individuals are asked to evaluate a system, relevant participation conditions should be explained.

Collect only the information necessary for the research.

Where appropriate, record:

- Evaluation purpose.
- Participation conditions.
- Relevant consent or authorization.
- Data collected.
- Data retention.
- Evaluation procedure.
- Limitations.

### 13.4 Sensitive Research

Research involving sensitive personal information, vulnerable populations, or potentially harmful applications requires additional scrutiny.

Where formal ethical review, contractual permission, informed consent, or legal authorization is required, the experiment must not proceed as though an internal methodology were a substitute for those requirements.

### 13.5 Responsible AI

AI research should consider possible bias, harmful outputs, misuse, privacy risks, and the limitations of automated decision-making.

Where relevant, the experiment should document the safeguards and evaluation measures applied.

Detailed AI requirements remain governed by `RESPONSIBLE-AI-v2.0.md`.

### 13.6 Ethical Limitations

Where a meaningful ethical assessment cannot be performed, the limitation must be addressed before the research proceeds into activities that could materially affect people or protected information.

The maintainer should restrict, redesign, or discontinue an investigation when adequate safeguards or authorizations cannot be established.

### 13.7 No Substitution for External Review

The Lab's internal methodology does not constitute:

- An institutional ethics approval.
- A legal assessment.
- A regulatory authorization.
- A professional clinical assessment.
- A formal research ethics certification.

Where such review or authorization is required, it must be obtained through an appropriate process.

---

## 14. Research Documentation Standard

Substantial investigations should follow a common documentation structure.

Each research report should include the relevant sections below.

The exact structure may be adapted to the type and complexity of the investigation.

### 14.1 Research Identity

- Research title.
- Experiment identifier.
- Research domain.
- Author or maintainer.
- Creation date.
- Last revision date.
- Current Project Status, where applicable.
- Relevant project and repository.
- Research scope.
- Relevant document version.

### 14.2 Executive Summary

A concise description of the investigation, its purpose, principal method, and most important findings.

The summary should not present planned work as completed work.

### 14.3 Research Question

The question being investigated and its context.

### 14.4 Background and References

Existing knowledge, relevant sources, and the technical context.

Important claims should be traceable to their original sources.

### 14.5 Hypothesis

The initial proposition or expected outcome, where applicable.

Where the hypothesis has changed, record the change and its rationale.

### 14.6 Scope

The boundaries, assumptions, exclusions, and constraints.

### 14.7 Methodology

The experiment design, tools, procedures, variables, and evaluation criteria.

### 14.8 Implementation

Technical details necessary to understand the experiment.

### 14.9 Results

Observed and measured outputs.

Distinguish direct observations from derived measurements and interpretations.

### 14.10 Analysis

Interpretation of results and comparison against the original question or hypothesis.

### 14.11 Evidence and Confidence

The relevant evidence category, supporting records, and confidence limitations.

The E0–E5 categories may be used where meaningful.

### 14.12 Limitations

Known uncertainties, weaknesses, and constraints.

### 14.13 Conclusion

The principal findings and whether the original hypothesis was supported, rejected, or left unresolved.

### 14.14 Next Steps

Potential additional experiments, improvements, or unresolved questions.

### 14.15 References and Attribution

Sources, third-party resources, and relevant licences.

### 14.16 Reproducibility Information

Where relevant, include the environment, dependencies, configuration, inputs, test procedure, and reproduction limitations.

### 14.17 Publication Considerations

Identify relevant publication restrictions or conditions without reproducing confidential information.

Publication decisions must follow `PUBLICATION-POLICY-v2.0.md`.

---

## 15. Research Decision Framework

At the end of an investigation, findings should lead to an explicit decision.

Recommended research decision categories:

| Decision | Meaning |
|---|---|
| Proceed | Evidence supports continuation into the next research or development activity. |
| Refine | The method or hypothesis requires modification. |
| Repeat | Additional testing is necessary. |
| Expand | The investigation has revealed new research questions. |
| Validate Further | Evidence is promising but insufficient. |
| Hold | The work is temporarily suspended. |
| Reject | The investigated approach is unsuitable within the defined scope. |
| Archive | The investigation is concluded or discontinued while its record is preserved. |

A decision to reject an approach should be accompanied by the reasoning and relevant evidence.

An archived experiment may remain a valuable research record.

### 15.1 Decision Records

A material research decision should record:

- Decision identifier, where used.
- Date.
- Research question or experiment.
- Decision.
- Evidence considered.
- Rationale.
- Known limitations.
- Next action.
- Responsible decision-maker.

### 15.2 Research Decisions Are Not Project Statuses

The categories in this section describe research decisions.

They must not be introduced as additional Project Status values.

The canonical Project Status vocabulary is defined in `PROJECT-LIFECYCLE-v2.0.md`.

### 15.3 Discontinuation

An investigation may be discontinued when:

- The hypothesis is no longer relevant.
- The method is unsuitable.
- The required resources are unavailable.
- The risk is unacceptable.
- The research question has been answered sufficiently.
- The investigation is superseded by a more appropriate approach.

The reasons should be recorded where they provide useful research knowledge or accountability.

---

## 16. Research Governance and Responsibilities

### 16.1 Research Governance

Research activities are conducted under the governance model defined in `GOVERNANCE-v2.0.md` and the foundational principles established by `LAB-CHARTER-v2.0.md`.

The maintainer is responsible for the organisation and integrity of research conducted and published under the Lab's identity.

### 16.2 Methodological Consistency

The methodology should be applied proportionately.

Small exploratory studies do not require the same documentation and validation effort as complex comparative experiments.

However, all substantial investigations should establish their purpose, scope, methods, and relevant limitations.

### 16.3 Changes to Research Methods

Material changes to an experiment's design or evaluation criteria should be documented.

This includes changes made in response to unexpected results.

The original method and subsequent changes should remain distinguishable.

### 16.4 External Review

External technical, academic, or expert review may be sought when appropriate.

Where no external review has taken place, the research must not imply independent verification.

The identity and role of an external reviewer should be represented accurately and with appropriate authorization.

### 16.5 Research Integrity

Research must not knowingly:

- Fabricate results.
- Misrepresent testing conditions.
- Conceal material failures.
- Manipulate evaluation criteria after observing results without disclosure.
- Present generated output as independently verified fact.
- Claim reproducibility without adequate evidence.
- Misattribute authorship.
- Present assumptions as established findings.
- Selectively omit material observations to create a misleading conclusion.
- Present an informal review as independent expert validation.
- Use data without appropriate rights or authorization.

### 16.6 Research Responsibilities

The maintainer is responsible for ensuring that material research published under the Lab's identity is appropriately documented and reviewed.

Contributors and collaborators should:

- Work within the agreed research scope.
- Record material methodological changes.
- Respect data and intellectual property restrictions.
- Identify relevant limitations.
- Report significant failures or risks.
- Avoid unsupported claims.
- Attribute sources and contributions appropriately.

Participation does not automatically grant authority to approve a public release or represent the Lab.

---

## 17. Methodology Adaptation

This methodology provides a shared framework, not a rigid sequence that must be applied identically to every project.

The approach may be adapted according to:

- Research complexity.
- Technical Maturity.
- Experimental uncertainty.
- Available resources.
- Data characteristics.
- Creative or artistic intent.
- Safety and privacy constraints.
- Intended publication format.
- Potential consequences of error.
- Reproducibility requirements.

An adaptation should preserve the principles of transparency, traceability, and intellectual honesty.

For a small experiment, a concise research record may be sufficient.

For a complex AI benchmark or technical investigation, a more formal protocol may be necessary.

The depth of the methodology should reflect the importance and complexity of the claims being made.

### 17.1 Documenting Adaptations

Where a material methodological adaptation affects the reliability or interpretation of results, record:

- What was adapted.
- Why the adaptation was necessary.
- Which requirements were affected.
- What limitations were introduced.
- Whether further evaluation is necessary.

### 17.2 Non-Negotiable Principles

Methodological adaptation must not be used to justify:

- Fabricated findings.
- Misleading reporting.
- Unauthorised data processing.
- Disclosure of confidential information.
- Unauthorised publication.
- False claims of independent validation.
- Concealment of material limitations.

---

## 18. Relationship with Other Lab Documents

This methodology operates within the broader Framing Creativity Lab documentation framework.

| Document | Responsibility |
|---|---|
| `README.md` | Public identity, mission, scope, and repository overview |
| `LAB-CHARTER-v2.0.md` | Mission, foundational principles, and institutional direction |
| `GOVERNANCE-v2.0.md` | Decision authority, responsibilities, and governance |
| `PROJECT-LIFECYCLE-v2.0.md` | Lifecycle stages and canonical Project Status definitions |
| `PROJECT-TEMPLATE-v2.0.md` | Standard project documentation and assessment fields |
| `QUALITY-STANDARDS-v2.0.md` | Technical Maturity, Operational Readiness, and quality expectations |
| `PUBLICATION-POLICY-v2.0.md` | Publication eligibility, classification, and approval controls |
| `RESPONSIBLE-AI-v2.0.md` | AI risk, responsible use, and human oversight |
| `SECURITY.md` | Security practices and vulnerability reporting |
| `CONTRIBUTING.md` | Contribution process and contributor responsibilities |
| `CODE-OF-CONDUCT.md` | Collaboration and behavioural expectations |

The documents serve different purposes and should be interpreted together.

The Lab Charter establishes foundational principles.

The Governance document establishes decision-making authority and responsibilities.

The Project Lifecycle defines the project's stages and canonical statuses.

The Quality Standards define technical maturity and operational readiness.

The Publication Policy determines what can be released publicly and under which conditions.

The Responsible AI Policy addresses AI-specific requirements and risks.

The Research Methodology establishes how investigations are conducted, evaluated, and documented.

A research project must satisfy the applicable requirements of all relevant documents.

### 18.1 Authoritative Terminology

| Subject | Authoritative document |
|---|---|
| Lifecycle Stage | `PROJECT-LIFECYCLE-v2.0.md` |
| Project Status | `PROJECT-LIFECYCLE-v2.0.md` |
| Technical Maturity | `QUALITY-STANDARDS-v2.0.md` |
| Operational Readiness | `QUALITY-STANDARDS-v2.0.md` |
| Publication Classification | `PUBLICATION-POLICY-v2.0.md` |
| Publication Status | `PUBLICATION-POLICY-v2.0.md` |
| AI Risk Classification | `RESPONSIBLE-AI-v2.0.md` |
| Data Classification | `PUBLICATION-POLICY-v2.0.md` |
| Research Evidence Categories E0–E5 | This document |

These fields and vocabularies must remain distinct.

The Research Evidence Categories describe the nature and support of research findings. They do not replace a project's Technical Maturity or Operational Readiness assessment.

---

## 19. Research Templates

The Lab should maintain reusable templates to support consistent research documentation.

Recommended templates include:

### A. Research Brief

Defines the research question, objectives, context, scope, and intended outcomes.

### B. Experiment Protocol

Defines the hypothesis, variables, methodology, test conditions, and evaluation criteria.

### C. AI Evaluation Protocol

Defines model identification, prompts, test datasets, evaluation criteria, configuration, and observed behaviour.

### D. Technical Evaluation Report

Documents implementation, testing, measurements, technical findings, and limitations.

### E. Comparative Study

Provides a structured framework for comparing models, frameworks, methods, or architectures.

### F. Research Findings Report

Summarises results, interpretation, evidence, conclusions, and next steps.

### G. Qualitative Study Record

Documents research questions, observation methods, evaluation criteria, qualitative findings, and interpretive limitations.

### H. Reproducibility Record

Documents the environment, versions, inputs, configuration, procedure, and conditions necessary to repeat an investigation where practical.

Templates should be introduced progressively and adapted to actual research requirements.

The presence of a proposed template in this section does not imply that a dedicated template file already exists.

---

## 20. Methodology Maintenance

### 20.1 Document Ownership

This methodology is maintained by J-ART under the governance framework established by Framing Creativity Lab.

### 20.2 Revision Authority

The maintainer approves substantive revisions in accordance with `GOVERNANCE-v2.0.md`.

### 20.3 Versioning

The document follows semantic document versioning.

- **Major:** Fundamental changes to the research framework.
- **Minor:** Addition or substantive revision of methodologies.
- **Patch:** Clarifications and editorial corrections.

### 20.4 Revision Records

Material changes should record:

- Version.
- Date.
- Author or responsible maintainer.
- Description.
- Reason for revision.
- Approval status.

### 20.5 Consistency Review

Changes should be reviewed for consistency with:

- Lab Charter.
- Governance.
- Project Lifecycle.
- Quality Standards.
- Publication Policy.
- Responsible AI Policy.
- Project Documentation Template.

Changes to canonical terminology must be coordinated with the document that owns the relevant vocabulary.

### 20.6 Continuous Improvement

The methodology may evolve through lessons learned from actual experiments.

Changes should improve research quality without introducing unnecessary administrative complexity.

A revision must not imply that historical experiments followed a method that was introduced only later.

Where relevant, historical research records should identify the methodology version under which they were conducted.

---

## 21. Final Principle

Research is not simply the process of finding confirmation for an idea.

It is the disciplined examination of a question, the willingness to test assumptions, and the ability to distinguish what is known from what is merely believed.

Framing Creativity Lab treats experimentation as a means of developing understanding.

Its methodology seeks to preserve curiosity without sacrificing rigour, technical ambition without hiding limitations, and creative freedom without abandoning accountability.

**Question with purpose.  
Investigate with curiosity.  
Experiment with discipline.  
Evaluate with evidence.  
Document with precision.  
Conclude with intellectual honesty.**

---

**FRAMING CREATIVITY LAB**  
Independent Research · Applied AI · Creative Technology · Digital Innovation

**Maintainer:** J-ART  
**Document:** `RESEARCH-METHODOLOGY-v2.0.md`  
**Reference:** `LAB-CHARTER-v2.0.md`  
**Publication requirements:** `PUBLICATION-POLICY-v2.0.md`

*The value of an experiment lies not only in what it demonstrates, but in what it allows us to understand.*
