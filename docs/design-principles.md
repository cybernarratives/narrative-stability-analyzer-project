# Design Principles

## 1. Judgment before generation

The primary job is diagnosis, not rewriting.

NSA should first establish what interpretive problem exists, if any. Recommendations or rewrites are downstream tasks.

## 2. Do not solve ambiguity for the author

Ordinary comprehension requires inference.

What the analyzer must not do is supply an absent **organizing relationship** simply because one would make the narrative coherent.

If the source copy does not materially privilege an interpretation, plausible alternatives should remain visible.

## 3. Evidence must be traceable

A finding should be grounded in supplied material.

The analyzer should distinguish:

- supporting evidence;
- counterevidence;
- contextual inference;
- unresolved information.

## 4. Stability is not truth

NSA does not determine whether a product claim is factually true.

A false claim can be narratively stable. A true claim can be narratively unstable.

Product truth, evidence quality, and narrative interpretation are related but distinct problems.

## 5. Stability is not persuasion

The system is not designed to optimize conversion language, emotional appeal, or stylistic polish.

Its core concern is whether intended readers can form materially consistent expectations.

## 6. Compression is not a defect

Headlines and short-form messaging are allowed to be compressed.

The relevant question is whether compression creates consequentially different interpretations, not whether every mechanism or exception has been stated.

## 7. Context matters, but context must be observable

Audience expertise and adjacent information can legitimately reduce interpretive burden.

“Buyers know what we mean” is not enough unless that knowledge is reasonably available to the intended reader.

## 8. One issue should not become five penalties

Diagnostic richness should not create scoring inflation.

If multiple observations share one causal source, they should normally cluster into one finding with multiple affected areas or consequences.

## 9. Stress tests are probes, not buyer evidence

Compression, retelling, expansion, and cross-functional translation can expose instability.

Generated retellings are diagnostic probes. They are not empirical evidence of how real buyers will behave.

## 10. Methodology is versioned

The diagnostic contract should be able to evolve without rewriting history.

Saved analyses retain the methodology and scoring version that produced them.

## 11. The model is replaceable

The system should not depend on one frontier model provider.

The defensible asset is the diagnostic methodology, structured contract, evaluation corpus, and product logic around the model.

## 12. Public proof, controlled execution

This repository exists to make the problem, architecture, and design thinking inspectable.

The hosted application remains the execution surface. Proprietary prompts, scoring details, evaluation fixtures, and production code remain private.
