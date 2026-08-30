# Security

- **Publication date:** 2026-08-30

## Reporting a vulnerability

Use the `SECURITY.md` policy in the public standard repository closest to the issue —
`DCS-LabsAI/r2-standard`, `r3-standard` or `r4-standard`. Report privately. Do not open a public issue
for a suspected vulnerability.

## What this portal will not publish

- **Exploit detail of any kind.** Where a defect must be disclosed, this portal names the **class** of
  defect and its consequence for a relying party, and stops there.
- **Proof artefacts demonstrating a defect.** None is published, and none will be while external review
  is outstanding.
- **Internals of any repaired circuit.**
- **Infrastructure topology, host inventory, or internal API surfaces.**

## Packages and installation — read this before installing anything

**This portal publishes no package name and no installation instruction.**

That is a deliberate security decision, not an omission. A canonical package scope for the R-Series has
not yet been fixed, and published documentation elsewhere has named a scope that was never registered.
**An unregistered package scope named in installation documentation is claimable by anyone**, and a
reader following such an instruction installs whatever the claimant put there.

Until one canonical scope is fixed and announced:

> **Do not install any R-Series package from a scope you found in documentation.** Obtain the reference
> implementations by cloning the public standard repositories directly.

## Standing statements

- **No independent third-party security audit of any R-Series layer has been performed.** See
  [`../external-audit/README.md`](../external-audit/README.md).
- **No R-Series layer is production**, by the programme's own published definition of the word. See
  [`../overview/README.md`](../overview/README.md).
- Where an internal document historically used *certified* or *approved*, that is an **internal DCS
  Labs self-assessment**, not an external finding, and it is described as one wherever it is referenced.
