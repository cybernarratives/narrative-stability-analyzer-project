# Architecture Overview

NSA is designed around a simple separation:

> **Model judgment and application judgment should not be the same thing.**

## 1. Input and context layer

The system accepts a narrative artifact plus relevant reader-visible context.

Author-declared intent is handled separately from the initial outside-in assessment so it does not bias the diagnostic pass.

## 2. Diagnostic reasoning layer

An LLM is used as a bounded reasoning component.

Its role is to test how the narrative may be interpreted, identify evidence for materially different readings, and surface candidate diagnostic issues.

A central safeguard is to prevent the model from silently “repairing” the narrative by inventing missing relationships that make the story more coherent than the supplied text actually supports.

## 3. Structured contract layer

Model output is constrained by typed, validated structures so findings remain inspectable, attributable, and versionable.

The public repository intentionally does not expose the production schema or internal reference model.

## 4. Deterministic application layer

The application, not the model, owns deterministic behavior such as validation, orchestration, version handling, persistence, and rendering.

This prevents the model from silently changing the product contract from one run to another.

## 5. Evaluation and conformance layer

The project uses regression and conformance testing to detect failures such as:

- synthesizing coherence the narrative did not establish;
- confusing lack of proof with interpretive instability;
- over-penalizing compressed or broad messaging;
- treating clarification as contradiction;
- multiplying one underlying issue into several unrelated penalties.

## 6. Versioning

A saved result belongs to the methodology and scoring system that produced it.

Future methodology revisions should create new analyses rather than silently reinterpret historical results.

The production implementation, internal schemas, prompt architecture, fixtures, and exact scoring mechanics are intentionally not included in this repository.
