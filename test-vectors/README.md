# Test vectors

- **Classification:** PUBLIC-REPRODUCIBLE
- **Publication date:** 2026-08-30

The test vectors are the strongest evidence in the estate, and they are **already fully public**. They
are indexed here and deliberately not copied — a vector corpus with two homes eventually has two
answers.

**Where they are:** `DCS-LabsAI/r2-standard` — `conformance/vectors/` (30), `verifier/vectors/` (30),
and `conformance/federation-vectors/` (6).

See [`../conformance/README.md`](../conformance/README.md).

## One corpus that is built but not yet published

A signature-suite-binding vector set exists internally and is **not published**. It encodes an
interoperability rule that third parties genuinely need:

> The signature suite is determined by **signed content only**. An algorithm label carried outside the
> signed content is a **label**, never an input to suite selection.

That rule is stated here because it is a real requirement learned from a real defect, and stating a
requirement is not the same as publishing a corpus. **The vectors themselves are absent**, pending the
publication decision. When they are published they will be published into the existing public
conformance surface, not into a new repository.
