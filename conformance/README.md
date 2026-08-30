# Conformance

- **Classification:** PUBLIC-REPRODUCIBLE
- **Publication date:** 2026-08-30

The conformance corpus is **not duplicated here**. It lives in `DCS-LabsAI/r2-standard`, where CI runs
it, and that repository is the single normative home.

| Corpus | Path | Population |
|---|---|---|
| R+2 receipt conformance | `r2-standard/conformance/vectors/` | **30 of 30 vectors public** |
| R+2 verifier corpus | `r2-standard/verifier/vectors/` | **30 of 30 public** |
| R+5 cross-issuer federation | `r2-standard/conformance/federation-vectors/` | **6 of 6 public** |
| Algorithm registry | `r2-standard/conformance/alg-registry.json` | — |
| CI workflow | `r2-standard/.github/workflows/conformance.yml` | Has run and passed |

## Why the negative cases are the point

The corpus is dominated by vectors a verifier passes **only by rejecting them** — tampered payloads,
wrong keys, broken and replayed chains, non-canonical encodings, unknown and reserved algorithm labels,
malformed signatures.

A corpus of valid inputs proves that an implementation can say yes. It says nothing about whether the
implementation can say no, which is the entire security property. That is why the negatives dominate,
and it is the strongest single design decision in the public estate.

## What is absent here

No pass-rate figure is printed on this page. Run the corpus yourself — that is what publishing it is
for, and a number quoted here would be strictly weaker evidence than the thirty seconds it takes to
reproduce it.
