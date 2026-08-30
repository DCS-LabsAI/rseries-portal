# Roadmap

- **Publication date:** 2026-08-30

**This page publishes a sequence, not a delivery claim.** There are no completion badges here, and no
layer is described as delivered or signed. A badge is a claim; a sequence is a plan.

No **future** item on this page carries a date. Committed dates that were overtaken within days of
publication are part of what this portal is correcting, and replacing them with fresh guesses would
repeat the defect rather than fix it. Items already **done** carry the date they were done, which is a
record rather than a forecast.

## Release status

**Current release: CLOSED, 30 August 2026.** Items 1 to 4 below are done — all nine P0 publication
corrections are applied and in effect, each re-verified against the live surface on that date. Items 5
onward are **future phase**. They are recorded here as sequence, they hold nothing open, and none of
them is claimed as delivered.

**C2.10 SEALED — NOT FROZEN. Production ceremony and further external validation are planned for a
future phase.**

## Order of work

The order matters more than the contents — several items are cheap only if the ones above them are done
first.

### Done — the current release

1. **DONE 2026-08-30 — Close the private-repository security items.** Nothing public moved before
   these. *(P0-1, P0-2)*
2. **DONE 2026-08-30 — Correct the live public claims.** The adversarial-suite figure now states the
   corrected result against the frozen tag, with its erratum and both repair commits; *audited* now
   appears on the live surfaces only inside explicit negations; the unregistered package scope appears
   only where labelled unpublished and reserved, beside an instruction not to install it, and in two
   dated blog errata; the evidence page links its record, names its populations and prints its three
   dates separately. *(P0-3, P0-5, P0-7)*
3. **DONE 2026-08-30, by erratum rather than re-issue — Correct the post-quantum wording.** The live
   text is corrected. The five issued PDFs are **preserved byte-identical** and annotated by a published
   erratum. **Re-issuing the set as a set is future-phase — see item 9**, because the tool that
   produced those documents is not available on current hardware. *(P0-6)*
4. **DONE 2026-08-30 — Banner the R+4 repository as historical and publish the defect erratum.**
   *(P0-8)* This un-gated [`../layers/r4.md`](../layers/r4.md), which now carries hash, constraint
   count, status and errata only.
5. **DONE 2026-08-30 — Withdraw the long-duration evidence.** All six documents, including the
   aggregating one, are withdrawn on the live surface with every original preserved unchanged. *(P0-4)*
   **The withdrawal is what closed; the re-run is item 10.**

### Future phase — recorded as roadmap, holding nothing open

No item below is claimed as started, and none carries a date.

6. **Publish the ceremony artefacts** as release assets with a SHA-256 manifest, after correcting the
   reproduction instructions that currently describe artefacts the repository does not contain.
7. **Verify the deployed verifier's source on the block explorer** — the single highest-value open
   verification — and **publish the five R+3 receipts**, which closes the largest reproducibility gap in
   the best public artefact the programme has.
8. **Build the harnesses** behind [`../cryptographic-evidence/README.md`](../cryptographic-evidence/README.md),
   so a reader can run a check rather than read what it returned, and **continue this portal** from the
   allow-list, file by file, default-exclude.
9. **Re-issue the five evidence PDFs as a set**, with the post-quantum wording corrected in the
   documents themselves. Until then the originals stand byte-identical beside their erratum.
10. **Fix the controls that could not report failure, add a cycle-completeness gate, and re-run the
    long-duration programme.** Publish the original artefacts or state that none exist. **No corrected
    soak figure is published before this.**
11. **Freeze the repaired R+4 circuit and split the identifier collision**, then run a production
    ceremony — independent external contributors, a beacon height pre-announced on day zero, a genuine
    window of at least fourteen days, and dated attestations. **C2.10 SEALED — NOT FROZEN. Production
    ceremony and further external validation are planned for a future phase.**
12. **Settle the contract text with counsel** where it carries the unregistered package scope.
13. **`external-audit/` stays empty** until a named external firm completes signed work. This is not a
    scheduled item and no engagement is claimed: **nothing in the R-Series has been externally
    audited**, and no internal review, internal gate, internal self-assessment or AI-assisted review
    counts as one.

## What will not appear on this roadmap

- A layer marked delivered on the strength of an internal result.
- A completion badge for any layer whose source is private.
- A ceremony described as complete before it has been run.
