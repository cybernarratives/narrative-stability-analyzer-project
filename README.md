# Narrative Stability Analyzer

**An AI-assisted diagnostic system for testing whether positioning and messaging create stable, predictable interpretations.**

The Narrative Stability Analyzer (NSA) is an active project exploring a simple question:

> When a company communicates a product, category, or market narrative, will reasonable intended readers form materially similar mental models — or will the message create avoidable ambiguity, expectation drift, or correction burden?

NSA is being designed as a diagnostic instrument rather than a copywriting tool. It does not try to invent strategy for the author. It evaluates how effectively a supplied narrative translates strategy into reader-visible meaning.

## Why this exists

Strong products can still create weak market outcomes when the narrative asks buyers to supply too much interpretation on their own.

The problem is often not grammatical clarity. A message can be readable, polished, and internally coherent while still producing materially different understandings of:

- what the offering fundamentally is;
- what it actually does;
- where its scope begins and ends;
- who or what is responsible for consequential actions;
- why the mechanism produces the claimed result;
- what outcome is actually being promised.

NSA is intended to make those failure modes inspectable before they become sales qualification, buyer confusion, implementation correction, or messaging debt.

## Core idea

**The model is the engine. The methodology is the product.**

Large language models are useful reasoning systems, but an unconstrained model can easily “help” by supplying an organizing abstraction, causal bridge, or boundary that the source narrative itself never established.

NSA therefore uses a structured methodology to distinguish what the narrative establishes from what a reader would have to supply on their own, and to test whether materially different interpretations remain plausible.

The goal is not to punish compression or provocative messaging. The goal is to determine whether the narrative does enough interpretive work for the intended audience without relying on the model to silently repair missing relationships.

## Current architecture

The project combines three layers:

- **Structured diagnostic methodology** — a formal set of rules for evaluating whether a narrative supports a sufficiently stable reader interpretation.
- **LLM-assisted reasoning** — used inside bounded diagnostic tasks rather than as an unconstrained grader.
- **Deterministic application logic** — used for validation, orchestration, versioning, and repeatable output handling.

The production implementation, prompts, calibration corpus, scoring details, and evaluation fixtures remain private.

See:
- [Methodology overview](docs/methodology-overview.md)
- [Architecture overview](docs/architecture-overview.md)
- [Design principles](docs/design-principles.md)
- [Illustrative analysis](examples/sample-analysis.md)

## Project status

**Active development.**

The current work is focused on methodology validation, conformance testing, anti-synthesis behavior, finding attribution, and version-safe scoring design.

A hosted version is planned. This public repository is a project and methodology overview, not the production codebase.

## What this project demonstrates

Beyond the product idea itself, NSA is also an experiment in how domain expertise can be encoded into a repeatable AI-assisted decision system.

The work includes:

- translating a qualitative PMM problem into a formal diagnostic contract;
- defining schemas and typed outputs;
- separating model judgment from deterministic application logic;
- building regression and conformance tests;
- designing safeguards against plausible-but-unsupported model synthesis;
- versioning methodology and saved results independently;
- treating AI as a reasoning component inside a larger product system rather than as the product itself.

## What this is not

NSA is not:

- a generic messaging grader;
- a readability tool;
- an AI copywriter;
- a persuasion optimizer;
- a substitute for product or market strategy.

It assumes the author owns the strategy. The analyzer evaluates how that strategy survives translation into narrative.

## Availability

A hosted version is in development.

If you are interested in the methodology, product design, or the broader problem of buyer interpretation and narrative credibility, you can follow the related work at [Cyber Narratives](https://cybernarratives.substack.com).

---

**Repository note:** This repository intentionally contains documentation and illustrative material only. The production application and proprietary implementation remain private.
