# Cryptographic evidence

- **Classification:** ABSENT — GATED
- **Gates:** **P0-3** and **P0-6** ([`../STATUS.md`](../STATUS.md))
- **Publication date of this page:** 2026-08-30

## No cryptographic figure is published on this page

Not one. No adversarial case count, no fuzz result, no post-quantum conformance or validation figure,
no signature-suite pass rate. **They are absent, not provisional**, and they will stay absent until
P0-3 and P0-6 close.

## Why

Two separate reasons, and it is worth keeping them apart.

**P0-3 — a figure that is true of the wrong code.** An adversarial suite reported a clean result. A
subsequent internal review found that the suite's oracle **could not detect the attack family the suite
enumerated** — the check could not report failure, so its success meant nothing. Re-run with a corrected
oracle against that same pinned code, the same suite reports failures. The underlying defect is repaired
in the current implementation, where the corrected suite reports clean again. **The repair is not
present in the tag the published figure pins to.** Publishing the original figure would publish a
number that is true of code the citation does not point at.

**P0-6 — wording, not mathematics.** Post-quantum descriptions in the document set need correction
before any post-quantum figure is published alongside them. A figure that is correct beside a
description that is not is worse than no figure, because the reader will carry away the description.

## What will appear here, when it does

**Harnesses, not asserted numbers.** The intent of this section is that a reader can run the check
themselves rather than read what it returned. A number published without the harness that produced it
is the exact failure mode this whole section is gated on.

Each entry, when published, will carry its classification label and its **run date and publication date
printed separately**.
