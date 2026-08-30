# Evidence

- **Publication date:** 2026-08-30

Every page in this section carries a [classification label](../CLASSIFICATION.md) and prints its **run
date and publication date separately**.

| Section | State |
|---|---|
| [`long-duration/`](long-duration/README.md) | **No figure published.** Prior results withdrawn pending re-run. Gated on P0-4 |
| [`../cryptographic-evidence/`](../cryptographic-evidence/README.md) | **Placeholder.** Gated on P0-3 and P0-6 |
| [`../verification/`](../verification/README.md) | Written — what a third party can check today, and what it cannot |
| [`../external-audit/`](../external-audit/README.md) | **Empty by design.** No external audit has occurred |

## The standard applied to everything in this section

A number is published here only with the artefact that produced it. A record published without its
source is labelled **PUBLISHED-EVIDENCE-ONLY** and is not counted as verification.

The reason is specific rather than stylistic. The recurring defect this programme has been correcting
across every layer is **a control that cannot report failure** — a check whose success is guaranteed
regardless of input, and which therefore carries no information. Several published figures turned out
to be gated by exactly such a control. **Publishing the harness alongside the number is what makes the
number falsifiable**, and a figure that cannot fail is not evidence of anything.
