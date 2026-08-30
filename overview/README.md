# Overview

- **Publication date:** 2026-08-30

## What the R-Series is

A layered set of standards for **agent trust receipts**: a signed, tamper-evident record of what an
automated agent did, which a party who does not trust the agent's operator can nonetheless check.

Each layer adds one capability on top of the one below it, and each is named `R+n`. **`R+n` is the
canonical public layer naming.**

| Layer | In one line | Where it stands |
|---|---|---|
| **R+2** | The receipt itself — a signed, canonicalised record with a chain | Public standard, public reference verifiers, public conformance corpus |
| **R+3** | Tamper-evident audit export — a bundle of receipts, anchored on a public chain | Public standard, public reference, one mainnet-anchored bundle |
| **R+4** | Zero-knowledge verification — prove a property of a receipt set without revealing the receipts | Public standard and **historical** reference circuit. See the gate on [`../layers/r4.md`](../layers/r4.md) |
| **R+5 → R+12** | Federation, and layers beyond it | See [`../layers/STATUS_R5_R12.md`](../layers/STATUS_R5_R12.md) — one of the eight has public evidence a third party can act on today |

## The posture this portal is written in

The programme's own terminology document sets the standard, and this portal applies it rather than
inventing a softer one:

> **When in doubt, claim less. An accurate "operational prototype" is stronger than a contestable
> "production system."**

And, from the same document, the definition of *production* — independently audited by a party outside
DCS Labs, adversarially tested, and resilient under failure and load:

> **No R-Series layer meets this definition today. The word "production" must not be applied to any
> layer.**

That is the project's own rule, written by the project, before this portal existed. This portal keeps
it.

## Four things stated plainly, so they cannot be missed

1. **Nothing in the R-Series has been externally audited.** Not one layer, not one component. See
   [`../external-audit/README.md`](../external-audit/README.md).
2. **No layer is production.** By the programme's own definition, quoted above.
3. **Where a claim is unproven, this portal says unproven** — and keeps *unproven* strictly apart from
   *did not happen*.
4. **This portal is a skeleton and has not launched.** See [`../STATUS.md`](../STATUS.md).

## What is genuinely strong here

Said as plainly as the weaknesses, because an honest surface reports both:

- The R+3 anchor is a real transaction on a public chain, and its calldata commits the stated root.
  Anyone can check it, today, without asking DCS Labs for anything.
- The R+2 conformance corpus is a real standard with a majority of **negative** vectors — cases a
  verifier passes only by **rejecting** them — and multiple independent implementations pass it.
- The May 2026 ceremony happened, its beacon checks out to the block hash, and its own transcript
  discloses its principal weakness in language most programmes would not write.

**The open problems are in the evidence and publication layers, not in the mathematics.**
