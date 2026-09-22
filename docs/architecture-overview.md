# Architecture Overview

NSA is designed around a simple separation:

> **Model judgment and application judgment should not be the same thing.**

## 1. Input and context layer

The system accepts a narrative artifact plus reader-visible context such as audience, artifact type, completeness, and communication posture.

Declared author intent is handled separately so it cannot contaminate the initial outside-in assessment.

## 2. Diagnostic reasoning layer

An LLM is used as a bounded reasoning component.

Its job is to help identify:

- the likely reader model;
- materially supported alternate models;
- explicit evidence and counterevidence;
- unresolved consequential relationships;
- diagnostic observations;
- candidate findings.

The model is instructed not to “repair” the narrative by supplying a missing governing abstraction, product role, causal bridge, or expectation boundary merely because doing so would make the message coherent.

## 3. Structured contract layer

Model output is constrained by schemas and typed references.

This layer exists to make the reasoning inspectable and to support:

- required fields;
- evidence traceability;
- finding ownership;
- confidence and applicability;
- stress-test lifecycle;
- result comparability;
- methodology versioning.

## 4. Deterministic application layer

The application, not the model, owns deterministic behavior such as:

- validation;
- scoring orchestration;
- score bands;
- version identifiers;
- persistence;
- migration handling;
- result rendering.

This prevents the model from silently changing the scoring contract from one run to another.

## 5. Evaluation and conformance layer

The project uses regression fixtures and conformance checks to test whether the implementation behaves according to the methodology.

Important failure modes include:

- inventing a synthetic umbrella narrative;
- rewarding internal coherence that the source copy never established;
- confusing absent proof with narrative instability;
- punishing broad positioning merely for being broad;
- treating every qualification as a correction;
- forcing multiple interpretations when only one is supported;
- double-counting one underlying issue across multiple diagnostic areas.

## 6. Versioning

A saved result belongs to the methodology and scoring system that produced it.

Future methodology revisions should create new analyses rather than silently reinterpret historical results.

The production implementation, internal schemas, prompts, fixtures, and exact scoring mechanics are intentionally not included in this repository.
