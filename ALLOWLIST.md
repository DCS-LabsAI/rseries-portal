# Allow-list

- **Publication date:** 2026-08-30

This repository was assembled **default-exclude**. A file is here only because it was individually
reviewed and found public-safe. Nothing was copied in bulk, from anywhere.

## The two admissible origins

| Origin | Rule | Count today |
|---|---|---|
| **Newly written for this repository** | Derived from the public repositories and from an internal reconciliation dated 2026-08-30. Every claim traced to a source before it was written. | 19 files |
| **Verbatim from an already-public repository** | Reproduced unedited, with the source repository and path named on the page. | 1 file — [`history/r4-v0.1-may-2026.md`](history/r4-v0.1-may-2026.md), from `DCS-LabsAI/r4-standard`, `reference/ceremony/CEREMONY_TRANSCRIPT.md` |

**No file in this repository originated from a private repository.** No history was inherited from any
repository. This repository's first commit is its first commit.

## Excluded by category

These categories were considered and **rejected in full**. Each is excluded as a category, so that a
future addition has to argue its way in rather than slip in beside a similar file.

| Excluded | Reason |
|---|---|
| Anything from a private repository | Not individually reviewed as public-safe. The default is exclusion, and it applies to all of it |
| Infrastructure and deployment architecture; internal API surfaces | Operational attack surface. Never published |
| Internal security-pass records | Contain the detail they were written to fix |
| Exploit detail, and any proof artefact demonstrating one | Publishing a defect's existence is disclosure; publishing its construction is a recipe |
| Internals of any repaired circuit | Same |
| Internal self-assessments and their verdict strings | An internal review is not an external finding, and a document that reads like a certificate will be read as one |
| Raw scan output containing matched secret material | Publishing the finding requires publishing the secret |
| Long-duration figures | Gated on P0-4. **No soak figure appears anywhere in this repository** |
| Adversarial-suite figures | Gated on P0-3 |
| Post-quantum figures | Gated on P0-6 |
| Any citation of the reference-core evidence record | Gated on P0-7 |
| Any description of R+4 as a layer | Gated on P0-8. The ceremony *history* is separately cleared and is published |
| Package names and installation instructions | No canonical scope is fixed. See [`security/README.md`](security/README.md) |
| Embargoed specifications and any material behind unsigned agreements | Self-evident |
| Ceremony key material and large binaries | Not excluded on safety grounds — excluded from **git**. They belong in release assets with a manifest. See [`architecture/README.md`](architecture/README.md) |

## Why the list was enumerated rather than estimated

An earlier estimate of how many documents were publishable was wrong by roughly ten times, in the
unsafe direction. It was reached by counting files rather than reviewing them — duplicates counted
separately, and code files counted as documents.

**Enumerate. The default is exclusion.** A size estimate is not an allow-list, and the difference
between the two is the entire security property of this repository.
