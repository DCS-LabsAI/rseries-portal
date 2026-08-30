# Status and release record

- **Publication date of this state:** 2026-08-30
- **Repository state:** PUBLISHED — content deliberately partial, and every absence stated
- **Release:** **CURRENT RELEASE CLOSED**

The launch gate that previously held this portal was the P0 register below. **All nine P0 items are
closed — applied and in effect — as at 30 August 2026**, and the portal is published on that basis.
The gates came from an internal reconciliation of the R-Series evidence completed on 30 August 2026.
**That reconciliation is an internal review. It is not an external audit and is not counted as one.**

## What closing this release does and does not mean

**It means:** the nine corrections that had to reach a reader before this portal could be cited have
reached one, on the live surface, and each was re-checked against that surface on 30 August 2026.

**It does not mean** any of the following, none of which has happened:

- **Nothing is externally audited.** No independent third-party security audit of any R-Series layer
  has been performed. [`external-audit/`](external-audit/README.md) is empty and stays empty.
- **C2.10 is SEALED — NOT FROZEN.** Production ceremony and further external validation are planned
  for a future phase.
- **No corrected soak figure is published**, here or anywhere. The withdrawal is complete; the re-run
  is not done.
- Closing a release does not convert an internal result into a public proof.

Work that is genuinely future-phase is recorded as **roadmap** in [`roadmap/`](roadmap/README.md).
It is recorded there as sequence, never as a delivery badge, and it does not hold this release open.

## Why a partial portal is published at all

Because a structure that says what is missing is more honest than a structure that waits until it can
say only good things. Every absence below is stated and gives its reason. Nothing here is provisional:
a figure whose correctness is not established is **not printed at all**, rather than printed with a
caveat.

## The P0 register — closed

**Population: nine items. Nine CLOSED, zero open.** Four closed before 30 August 2026; the remaining
five — every one a correction to a surface outside this repository, the live website and the issued
document set — closed on 30 August 2026.
State as at **2026-08-30**; each row's state was re-verified against the live surface on that date,
not carried forward.

**"CLOSED" here means applied and in effect — not drafted.** Remediation that exists only on an
unmerged branch is **not** closed. Every row below was confirmed merged and serving; a correction that
is green in a branch has not corrected anything a reader can see.

| Gate | What it blocks in this portal | State |
|---|---|---|
| **P0-1** | Credential-handling verification on a private repository. Blocks nothing in this portal directly; it blocks the whole publication sequence. | **CLOSED 2026-08-30 — both arms.** The rotated credential is verified **refused**; a current credential is verified **accepted**. The second arm mattered: the host answers a mismatch with the same status it uses for an unknown route, so the refusal alone could not distinguish a gate that rejects a dead credential from one that rejects everything. The control is now proven able to fail in both directions |
| **P0-2** | A full-history secret scan, with archives opened, of a private repository that had never been scanned. Same. | **CLOSED 2026-08-30.** History, working tree, all archives expanded recursively to a fixed point, and the embedded repository's object store scanned blob by blob. The scanning ruleset was itself found defective twice and repaired both times |
| **P0-3** | The adversarial-suite figure and its oracle correction. **Formerly blocked** [`cryptographic-evidence/`](cryptographic-evidence/README.md). | **CLOSED 2026-08-30 — live.** The public evidence page now states the corrected result against the frozen tag — **309 slips out of 404,000 adversarial cases**, not 0 — names the corrected-oracle date, cites both repair commits, and links its erratum. The original figure no longer stands anywhere on that page. The correction was published by **addition and annotation**; no prior document was rewritten |
| **P0-4** | Long-duration ("soak") results. **No soak figure is published anywhere in this portal.** Blocks [`evidence/long-duration/`](evidence/long-duration/README.md). | **CLOSED 2026-08-30 — withdrawal complete and in effect.** Satisfied *within this portal* by construction: no figure is printed. Elsewhere the withdrawal now covers the full set — **all six soak evidence documents**, including the sixth aggregating document found on 2026-08-30 that no prior list named. Every card on the live evidence page carries a WITHDRAWN marker and links the notice; every original document is preserved unchanged. **The withdrawal is closed; the re-run is not done and is future-phase** |
| **P0-5** | Removal of *audited* language and of references to an unpublished package scope from the live web surface. Nothing in this portal uses either. | **CLOSED 2026-08-30 — live.** Verified across the live surfaces on that date: the word *audited* now appears only inside explicit negations ("not externally audited", "not independently audited by external third parties"), never as a description of an R-Series artefact. The unregistered scope now appears only where it is labelled **unpublished and reserved**, beside an instruction not to run an install command for it, and in two dated blog errata that name the correction. No live install instruction resolves to an unregistered name |
| **P0-6** | Post-quantum wording corrections in the document set. **Formerly blocked** every cryptographic figure in [`cryptographic-evidence/`](cryptographic-evidence/README.md). | **CLOSED 2026-08-30 — live, by erratum rather than re-issue.** The live evidence surface states the post-quantum position in corrected terms: a real ML-DSA-65 leg, software key custody rather than a FIPS-certified HSM, and no claim to a FIPS 204 / FIPS 205 validated module. The five issued PDFs are **preserved byte-identical and annotated by a published erratum** rather than re-issued. **Re-issuing the PDF set is future-phase work** — see the roadmap note below |
| **P0-7** | Evidence-record linking, population labelling and date labelling on the live evidence page. **Formerly blocked** this portal from citing that record. | **CLOSED 2026-08-30 — live.** The evidence record is linked; populations are named beside their figures rather than left as bare counts; and the three dates that were previously collapsed into one — tag creation, run date and baseline date — are printed separately, with the page stating in terms that collapsing them is how a July run comes to look like an August result. **No figure was changed to close this gate**; the labelling was added around the figures already published |
| **P0-8** | Historical banner and defect erratum on the public R+4 repository. **Formerly blocked [`layers/r4.md`](layers/r4.md).** | **CLOSED 2026-08-30 — merged and in effect.** The public repository now carries the historical banner above its first line and the defect erratum beside it, and the two attack-proof artefacts are withheld. [`layers/r4.md`](layers/r4.md) was written on that basis and is no longer gated |
| **P0-9** | A private archive repository stays private. No delete-and-flip. | **CLOSED — verified private on 2026-08-30**, by query rather than assumption, and nothing about it was changed. It remains a **standing** requirement: it stays private permanently, and reopening it would reopen this gate |

## What is deliberately absent, and why it stays absent

**The P0 gates are closed. These absences are not waiting on them.** Each one below now stands on a
substantive reason of its own, stated in its own terms. Closing a gate that blocked a figure does not
make the figure publishable — it removes the procedural hold and leaves the evidence question exactly
where it was.

| Absent from this portal | Why it stays absent |
|---|---|
| Any adversarial-fuzz case count, and any figure derived from it | **Not gated — a publication standard.** This portal publishes a **harness a reader can run**, not a number to be taken on trust. The corrected figure is published on the live evidence page with its erratum; the runnable harness is future-phase |
| Any long-duration / soak duration, cycle count, uptime figure or pass verdict | **No re-run has been performed.** Three of five runs were gated by controls that could not report failure. The withdrawal is complete and in effect; **an aggregate of withdrawn numbers is a withdrawn number**. Nothing appears here until the controls are fixed, the programme is re-run, and the **original artefacts** of that re-run are published. Future-phase |
| Any post-quantum conformance or validation figure | Published on the live evidence page with its custody and certification limits stated. **Not restated here without its harness** — same standard as the row above |
| Any citation of the reference-core evidence record, and any population or date drawn from it | P0-7 is closed and the live record is linked and labelled. This portal cites it only alongside the harness that reproduces it. Future-phase |
| ~~Any description of R+4 as a layer, beyond the preserved ceremony history~~ | ~~P0-8~~ — **un-gated 2026-08-30**; [`layers/r4.md`](layers/r4.md) now carries hash, constraint count, status and errata only |
| Any external-audit content | **No external audit has occurred.** Indefinite, and not a roadmap item with a date |
| Any exploit detail, proof artefact or repaired-circuit internal | Indefinite, by policy |
| Any package name or installation instruction | No canonical scope is fixed. The contract-text question is with counsel — future-phase |

## Future phase — recorded as roadmap, not as a held release

These are **not** blockers on the current release and do not hold it open. They are recorded so that a
reader knows the difference between *done* and *not yet attempted*.

- **C2.10 SEALED — NOT FROZEN. Production ceremony and further external validation are planned for a
  future phase.** The repaired circuit has no trusted setup, and therefore no ceremony, no verifying
  key and no deployed verifier. An identifier collision is open and must be split before any ceremony.
- **Re-run of the long-duration programme**, under fixed controls and a cycle-completeness gate, with
  original artefacts published. No corrected soak figure will be published before that.
- **Re-issue of the five evidence PDFs as a set.** The documents are preserved **byte-identical** and
  annotated by a published erratum. The tool that produced them is **not available on this hardware**,
  so re-issue is a future-phase action, not a pending edit.
- **External validation by a named firm.** Until one completes signed work,
  [`external-audit/`](external-audit/README.md) stays empty. **No internal review, internal gate,
  internal self-assessment or AI-assisted review is an external audit**, and none is counted as one.
- **Counsel on the contract text** carrying the unregistered package scope.
- **Publication of the five R+3 bundle receipts**, and of the ceremony artefacts as release assets
  with a SHA-256 manifest.
- **Block-explorer source verification of the deployed verifier** — the highest-value single open
  verification.

## What is published here

- The May 2026 ceremony record, preserved exactly, with errata appended and never edited —
  [`history/`](history/README.md).
- The publication architecture — [`architecture/`](architecture/README.md).
- Pointers to the three public standard repositories, which are the primary evidence —
  [`standards/`](standards/README.md).
- The R+2, R+3 and R+4 layer statements — [`layers/`](layers/README.md).
- The R+5 → R+12 status document — [`layers/STATUS_R5_R12.md`](layers/STATUS_R5_R12.md).
- The statement that no external audit exists — [`external-audit/`](external-audit/README.md).
