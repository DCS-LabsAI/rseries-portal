# Classification labels

Every page in this portal that reports a result carries one of these labels, and prints its **run
date** and its **publication date** separately. The two are not the same date and are never merged.

| Label | Meaning |
|---|---|
| **PUBLIC-REPRODUCIBLE** | Anyone can re-run this from artefacts that are published today, and get the same answer. |
| **PUBLIC-CHECKABLE** | Anyone can check this against an external source — a block explorer, a chain, a registry — without re-running anything. |
| **PUBLISHED-EVIDENCE-ONLY** | A record is published; the source that produced it is private. The result is an internal result. It is not publicly reproducible, and it is not proof. |
| **INTERNAL-ONLY** | Not published in any form. No figure, no record. |
| **WITHDRAWN** | Previously stated, now withdrawn. The reason is named on the page. |
| **UNPROVEN** | No evidence has been located. Distinct from *did not happen* — this portal keeps those two apart everywhere. |
| **ABSENT — by publication standard** | Deliberately not published, because publishing it would breach a standard this portal holds to — most often the rule that a figure appears only with the harness that produced it. The reason is named on the page. |
| **ABSENT — future phase** | Deliberately not published because the work that would produce it has not been done. Named on the page and recorded in [`roadmap/`](roadmap/README.md), with no date attached. **This is not a held release.** |
| **ABSENT — GATED** | *Retained so older references still read.* Deliberately not published until a named gate in [`STATUS.md`](STATUS.md) closed. **All nine P0 gates closed on 2026-08-30**, so no page in this portal now carries this label. |

## How to read a number in this portal

Three rules, applied without exception.

1. **Never a single unlabelled count.** A bare number is not evidence of anything.
2. **Always name the population.** "31 of 31" is meaningless until you know 31 of *what*, selected
   *how*. Every figure here names its population in the same sentence.
3. **Today and eventual, separately.** What is true of the artefact as it stands today is printed
   apart from what the layer is intended to cover eventually. A figure that is true of a suite is not
   thereby true of the claim the suite was written to support.

## What is excluded from the word "audit"

An **external audit** means a named, independent, human-led firm completing signed work.

Excluded by definition, and never counted as one anywhere in this portal: internal reviews, internal
verification gates, internal self-assessments, AI-assisted reviews of any kind, draft outreach,
unsigned engagement paperwork, and planned engagements.

The word *audited* does not appear as a description of any R-Series artefact in this portal. Where an
internal document historically used *certified* or *approved*, it is an **internal DCS Labs
self-assessment** and is described as one.
