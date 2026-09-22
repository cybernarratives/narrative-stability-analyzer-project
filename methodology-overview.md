# Methodology Overview

## Narrative stability

Narrative stability is the degree to which supplied messaging, within its reader-visible context, supports a sufficiently determinate consequential mental model and makes materially equivalent interpretations likely among the intended audience.

The construct is narrower than “good messaging.”

A narrative may be persuasive but unstable. It may be technically true but unstable. It may be elegant but unstable. Conversely, a compressed or provocative message can still be stable if the intended reader is unlikely to form materially different expectations from it.

## What the analyzer examines

NSA looks for consequential ambiguity in how a reader is likely to understand the offering, the problem it addresses, the way it works, the boundaries of responsibility, and the outcome being implied or promised.

The methodology distinguishes between what the narrative actually establishes and what a reader or model would have to supply to make the story coherent.

The public version of the methodology intentionally does not expose the internal parameter model, finding taxonomy, applicability rules, or scoring structure.

## Interpretive convergence

The analyzer does not search for every imaginable alternate reading.

Instead, it asks whether there are **reasonable, materially supported alternatives** that would change how an intended reader understands evaluation, workflow, responsibility, deployment, purchase, or expected outcome.

A useful distinction is:

> Conceivable ambiguity is not the same as consequential interpretive competition.

The methodology is designed to determine whether one reading is sufficiently privileged by the supplied narrative or whether multiple materially different models remain viable.

## Continuity

Narrative stability also depends on what happens as the message expands.

Later explanation can deepen, qualify, revise, or contradict an earlier interpretation. More detail is not automatically evidence of instability. The key question is whether the reader must consequentially revise the model they had already formed.

## Findings, not checklist penalties

The system is designed to reason from underlying causes rather than count every triggered observation as an independent defect.

A single source of ambiguity can affect multiple parts of a narrative without representing multiple unrelated failures.

## Context

Interpretation is evaluated relative to legitimate reader-visible context, such as audience, artifact type, completeness, narrative position, and adjacent material.

Context changes the amount of interpretive work an artifact is expected to perform. It should not be used to excuse a materially misleading interpretation created by the supplied wording.

## Blind analysis and declared intent

A core design principle is to separate outside-in assessment from comparison with the author’s intended takeaway.

This reduces the risk that the analyzer simply “finds” the meaning it has been told to expect.

The implementation details of that separation remain private.

## Current status

The methodology is under active validation. Current development work includes methodology conformance, anti-synthesis behavior, finding attribution, evaluation design, and version-safe scoring.

This public overview intentionally omits the production prompt system, internal parameter taxonomy, scoring implementation, stress-test contract, schemas, and evaluation corpus.
