# Verification — what a third party can check today

- **Publication date:** 2026-08-30

This page exists to answer one question honestly: **what can someone who does not trust DCS Labs check
for themselves, right now, without asking DCS Labs for anything?**

## Checkable today

| What | How | Classification |
|---|---|---|
| The R+2 conformance corpus | Clone `r2-standard`, run the corpus. 30 of 30 vectors, majority negative | **PUBLIC-REPRODUCIBLE** |
| The R+5 federation vectors | Same repository, `conformance/federation-vectors/` — 6 of 6 | **PUBLIC-REPRODUCIBLE** |
| The R+3 anchor transaction and its committed root | Fetch the transaction from any Base node or explorer and read its calldata. See [`../layers/r3.md`](../layers/r3.md) | **PUBLIC-CHECKABLE** |
| The R+4 ceremony beacon | Fetch Bitcoin block 950552 and compare its hash to the transcript. See [`../history/r4-v0.1-may-2026.md`](../history/r4-v0.1-may-2026.md) | **PUBLIC-CHECKABLE** |
| The R+4 verifier's existence and deployment | Fetch the contract and its deploy transaction on Base | **PUBLIC-CHECKABLE** |

## Not checkable today, and why

| What | Why not | Closable by |
|---|---|---|
| That the anchored Merkle root is the root of those five receipts | The five receipts are not published | Publishing the receipts |
| That the deployed verifier bytecode corresponds to the published source | Explorer source is unverified | Verifying the source on the explorer |
| That the ceremony's setup-verification line is what it says | No captured output; the input artefacts are unpublished | Publishing the ceremony artefacts as release assets with a manifest |
| How many contributors actually contributed | **Not verifiable by anyone**, for any ceremony of this size, including by DCS Labs. Stated so that nobody reads silence as confidence | — |
| That contributor machines were wiped | **Not verifiable by anyone.** Same | — |
| R+11 and R+12 figures | Their packages are unpublished | Publishing the packages |

## The rule this page follows

**Evidence without source is a claim, not proof.** Where this portal has published a record but not the
thing that produced it, the record is labelled **PUBLISHED-EVIDENCE-ONLY** and is not counted as
verification. Where nothing has been located at all, it is labelled **UNPROVEN**, which is kept
strictly distinct from *did not happen*.
