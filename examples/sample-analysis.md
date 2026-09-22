# Illustrative Analysis

> This is a simplified public example. It demonstrates the shape of the diagnostic reasoning, not the production output contract or scoring system.

## Submitted narrative

> Acme Sentinel is an autonomous security platform that investigates every alert and stops threats before they become incidents.
>
> Analysts review the platform’s recommendations and approve containment actions before changes are made.

## Likely reader model

The opening sentence strongly suggests that the product independently investigates alerts and takes action to stop threats.

The supporting sentence establishes a materially more human-mediated operating model: the product recommends, while analysts retain approval authority for containment.

## Diagnostic issue

**Autonomy and responsibility are not consistently bounded.**

The problem is not that human approval makes the word “autonomous” inherently false. Policy-bounded autonomy can be legitimate.

The issue is that the first sentence reasonably supports a stronger operational interpretation than the later workflow.

## Supporting evidence

- “autonomous security platform”
- “investigates every alert”
- “stops threats”

## Counterevidence / qualification

- analysts “review” recommendations;
- analysts “approve” containment actions before changes occur.

## Why it matters

A buyer could form materially different expectations about:

- who owns the final action;
- what the product executes independently;
- staffing implications;
- workflow changes;
- governance requirements.

## Continuity assessment

The later sentence does more than merely add implementation detail. It materially narrows the operating model implied by the opening.

That makes this a correction-risk issue, not simply a request for more technical detail.

## Smallest useful intervention

Clarify the autonomy boundary in the primary narrative rather than adding more explanation downstream.

For example, the messaging could distinguish between:

- autonomous investigation;
- autonomous recommendation;
- policy-bounded execution;
- human-approved containment.

## What this example is not

This example does not determine whether Acme Sentinel is technically autonomous, whether the claims are true, or whether the product is good.

It only evaluates the interpretation created by the supplied narrative.
