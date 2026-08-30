# Long-duration assurance

- **Classification:** WITHDRAWN
- **Publication date of this page:** 2026-08-30
- **Gate:** P0-4 ([`../../STATUS.md`](../../STATUS.md))

## No original artefacts are published, and no figure is published

**This section contains no long-duration figure of any kind.** No duration, no cycle count, no uptime
percentage, no pass verdict, no scorecard number. That is not an oversight and it is not a formatting
placeholder — it is the finding.

Long-duration ("soak") runs were executed internally in June and July 2026. Their raw evidence is not
published. Three of the five runs were gated by controls that a subsequent internal review found
**unable to report failure at all** — a control that returns success regardless of input is not
evidence of success, and a result gated by one carries no assurance.

**Those results are withdrawn pending re-run.** They are withdrawn as *verification evidence*; the
runs are not asserted to have not happened, and no claim is made in either direction about what a
correct re-run would show.

## What has to happen before anything appears here

1. The controls that could not report failure are fixed in code, and a completeness gate is added so
   that a run which did not finish cannot be recorded as one that did.
2. The programme is **re-run** under the fixed controls.
3. The **original artefacts** of that re-run are published here — not a summary of them, and not a
   number extracted from them.

If original artefacts for a given run cannot be produced, this page will say that no publishable
artefact exists for that run. It will not substitute a reconstructed one.

## Why the artefacts and not the summary

Because the defect being corrected here is precisely that a summary was trusted in place of the thing
it summarised. A number without its artefact is a claim, not proof.
