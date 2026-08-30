# Cryptographic evidence

- **Classification:** ABSENT — by publication standard
- **Former gates:** **P0-3** and **P0-6** — both **CLOSED 2026-08-30** ([`../STATUS.md`](../STATUS.md))
- **Publication date of this page:** 2026-08-30

## No cryptographic figure is published on this page

Not one. No adversarial case count, no fuzz result, no post-quantum conformance or validation figure,
no signature-suite pass rate. **They are absent, not provisional.**

**The gates that once held this page are closed.** That did not make the figures appear here. The
reason this page is empty is no longer procedural — it is the publication standard set out below.

## What the two closed gates settled

Two separate matters, and it is worth keeping them apart.

**P0-3 — a figure that was true of the wrong code. Corrected, and published where it belongs.** An
adversarial suite reported a clean result. A subsequent internal review found that the suite's oracle
**could not detect the attack family the suite enumerated** — the check could not report failure, so
its success meant nothing. Re-run with a corrected oracle against that same pinned code, the same suite
reports failures. The underlying defect is repaired in the current implementation, where the corrected
suite reports clean again; **the repair is not present in the tag the original figure pinned to.** The
corrected result, the corrected-oracle date and both repair commits are now published on the live
evidence page with an erratum, by addition. The original figure no longer stands there.

**P0-6 — wording, not mathematics. Corrected in the live text.** The post-quantum position is now
stated in corrected terms where it is published: a real ML-DSA-65 leg, software key custody rather than
a FIPS-certified hardware root, and no claim to a FIPS 204 / FIPS 205 validated module. The issued PDF
set is **preserved byte-identical and annotated by a published erratum** rather than re-issued.
Re-issuing that set is future-phase.

## Why this page still publishes nothing

**Because this section publishes harnesses, not asserted numbers** — and the harnesses are not built.

A number published without the harness that produced it is the exact failure mode this section exists
to avoid, and it is the failure mode that produced P0-3 in the first place. Restating a corrected
figure here, away from the runnable check, would repeat the defect in a smaller font.

**This is future-phase work.** It does not hold the current release open, and no date is attached to it.

## What will appear here, when it does

**Harnesses, not asserted numbers.** The intent of this section is that a reader can run the check
themselves rather than read what it returned.

Each entry, when published, will carry its classification label and its **run date and publication date
printed separately**.
