# Status and launch gate

- **Publication date of this state:** 2026-08-30
- **Repository state:** SKELETON — structure built, content deliberately incomplete
- **Launch:** HELD

This portal does not launch until every P0 gate below closes. The gates come from an internal
reconciliation of the R-Series evidence completed on 30 August 2026. **That reconciliation is an
internal review. It is not an external audit and is not counted as one.**

## Why a skeleton is being published at all

Because a structure that says what is missing is more honest than a structure that waits until it can
say only good things. Every gap below is marked **ABSENT — GATED** and names its gate. Nothing here is
provisional: a figure whose correctness depends on an open gate is **not printed at all**, rather than
printed with a caveat.

## The P0 register

| Gate | What it blocks in this portal | State |
|---|---|---|
| **P0-1** | Credential-handling verification on a private repository. Blocks nothing in this portal directly; it blocks the whole publication sequence. | OPEN |
| **P0-2** | A full-history secret scan, with archives opened, of a private repository that has never been scanned. Same. | OPEN |
| **P0-3** | The adversarial-suite figure and its oracle correction. Blocks [`cryptographic-evidence/`](cryptographic-evidence/README.md). | OPEN |
| **P0-4** | Long-duration ("soak") results. **No soak figure is published anywhere in this portal.** Blocks [`evidence/long-duration/`](evidence/long-duration/README.md). | OPEN |
| **P0-5** | Removal of *audited* language and of references to an unpublished package scope from the live web surface. Nothing in this portal uses either. | OPEN (elsewhere) |
| **P0-6** | Post-quantum wording corrections in the document set. Blocks every cryptographic figure in [`cryptographic-evidence/`](cryptographic-evidence/README.md). | OPEN |
| **P0-7** | Evidence-record linking, population labelling and date labelling on the live evidence page. Blocks this portal from citing that record. | OPEN |
| **P0-8** | Historical banner and defect erratum on the public R+4 repository. **Blocks [`layers/r4.md`](layers/r4.md).** | OPEN |
| **P0-9** | A private archive repository stays private. No delete-and-flip. | STANDING |

## What is deliberately absent, and under which gate

| Absent from this portal | Gate |
|---|---|
| Any adversarial-fuzz case count, and any figure derived from it | P0-3 |
| Any long-duration / soak duration, cycle count, uptime figure or pass verdict | P0-4 |
| Any post-quantum conformance or validation figure | P0-6 |
| Any citation of the reference-core evidence record, and any population or date drawn from it | P0-7 |
| Any description of R+4 as a layer, beyond the preserved ceremony history | P0-8 |
| Any external-audit content | No external audit has occurred. Indefinite. |
| Any exploit detail, proof artefact or repaired-circuit internal | Indefinite, by policy |
| Any package name or installation instruction | Canonical-scope decision, open |

## What is not gated, and is published here

- The May 2026 ceremony record, preserved exactly, with errata appended and never edited —
  [`history/`](history/README.md).
- The publication architecture — [`architecture/`](architecture/README.md).
- Pointers to the three public standard repositories, which are the primary evidence —
  [`standards/`](standards/README.md).
- The R+2 and R+3 layer statements — [`layers/`](layers/README.md).
- The R+5 → R+12 status document — [`layers/STATUS_R5_R12.md`](layers/STATUS_R5_R12.md).
- The statement that no external audit exists — [`external-audit/`](external-audit/README.md).
