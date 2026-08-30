# R-Series Portal

**This portal is published. It is a deliberately partial claim surface, and it names where it is partial.**

Nothing here should be read as a finished statement of what the R-Series is or does. Content is
published where evidence supports it; where it does not, the page says so by name rather than filling
the gap with a plausible sentence. **A section marked absent is a statement, not a gap awaiting text.**

- **Publication date of this state:** 2026-08-30
- **Status:** PUBLISHED — current release closed
- **Release record:** the P0 register in [`STATUS.md`](STATUS.md). **All nine P0 publication items are
  CLOSED — applied and in effect** as at 2026-08-30, each re-verified against the live surface on that
  date rather than carried forward from the register. The launch gate that previously held this portal
  is discharged.
- **What closing this release does not do.** It does not freeze C2.10, does not create a production
  ceremony, and does not make any part of the R-Series externally audited. **C2.10 SEALED — NOT FROZEN.
  Production ceremony and further external validation are planned for a future phase.** Future-phase
  work is recorded as roadmap in [`roadmap/`](roadmap/README.md) and is not a claim of delivery.

---

## What this repository is

The single documentation portal for the R-Series. It is built **fresh**, from an explicit allow-list,
**default-exclude**, assembled file by file. It inherits no history from any other repository, and no
file was copied wholesale from a private repository.

There is one portal, not one repository per layer. **Repository count is not a trust metric.**

## What this repository is not

- It is **not** an audit, and it does not report one. **No independent third-party security audit of any
  R-Series layer has been performed.** See [`external-audit/`](external-audit/README.md), which ships
  empty and will stay empty until a named external firm completes signed work.
- It is **not** a product page. Where a claim is unproven, this portal says unproven.
- It is **not** an installation surface. No package names and no install instructions are published
  here yet — see [`security/`](security/README.md).

## Where the actual artefacts live

The normative specifications, reference implementations and conformance vectors are in the three
public standard repositories, which are the primary evidence and are not duplicated here:

| Repository | Contents |
|---|---|
| `DCS-LabsAI/r2-standard` | R+2 receipt standard, conformance corpus, reference verifiers, R+5 federation spec section and vectors |
| `DCS-LabsAI/r3-standard` | R+3 audit-export standard, reference builder/verifier, anchored bundle |
| `DCS-LabsAI/r4-standard` | R+4 zero-knowledge standard, the **original** May 2026 circuit, ceremony record |

Those repositories keep their history unchanged. This portal links to them; it does not fork them.

## Reading this portal

| Section | State |
|---|---|
| [`overview/`](overview/README.md) | Written |
| [`architecture/`](architecture/README.md) | Written — publication architecture only |
| [`standards/`](standards/README.md) | Written — pointers to the public repositories |
| [`layers/`](layers/README.md) | R+2, R+3 and R+4 written — R+4 un-gated when P0-8 closed · **[R+5 → R+12 status](layers/STATUS_R5_R12.md)** written |
| [`verification/`](verification/README.md) | Written — what a third party can check today |
| [`conformance/`](conformance/README.md) | Written — pointer |
| [`test-vectors/`](test-vectors/README.md) | Written — pointer |
| [`cryptographic-evidence/`](cryptographic-evidence/README.md) | **No figure published.** The P0-3 and P0-6 corrections are applied and live; this section publishes harnesses, and those are future-phase work |
| [`evidence/long-duration/`](evidence/long-duration/README.md) | **No figure published.** Prior results withdrawn and the withdrawal is in effect; the re-run is future-phase work |
| [`history/`](history/README.md) | Written — the May 2026 ceremony, preserved exactly |
| [`receipts/`](receipts/README.md) | **No receipts published.** The five R+3 bundle receipts are future-phase work |
| [`security/`](security/README.md) | Written |
| [`roadmap/`](roadmap/README.md) | Written — sequence only, no delivery badges |
| [`external-audit/`](external-audit/README.md) | **Empty, by design** |

Every evidence page carries a [classification label](CLASSIFICATION.md) and, where it reports a
result, a **run date and a publication date printed separately**.

## Licensing of this portal's content

**Dual-licensed by material type**, decided by the rights holder on 2026-08-30. See [`LICENSE`](LICENSE).

| Material | Licence |
|---|---|
| Documentation authored by DCS AI Technologies L.L.C — prose, tables, diagrams, status pages, specifications | **CC BY 4.0** ([`LICENSE-DOCS`](LICENSE-DOCS)) |
| Code, scripts, configuration and examples authored by DCS AI Technologies L.L.C | **MIT** ([`LICENSE-MIT`](LICENSE-MIT)) |
| **Third-party material** — anything DCS AI Technologies L.L.C did not author, including the verbatim ceremony transcript in [`history/`](history/README.md) | **Excluded from both grants** unless separately and explicitly licensed where it appears |

Neither licence is an assurance claim. A permissive licence grants reuse rights; it does not confer
verification status, and **nothing in the R-Series has been externally audited**. This portal is
deliberately partial — reusing a page that states an absence does not convert that absence into a
published figure.

## Provenance of this repository

Every file in this repository is either **newly written for it** or **reproduced verbatim from an
already-public repository with its source named on the page**. Exactly one file is a verbatim
reproduction: [`history/r4-v0.1-may-2026.md`](history/r4-v0.1-may-2026.md), which reproduces
`r4-standard/reference/ceremony/CEREMONY_TRANSCRIPT.md`.

**No file in this repository originated from any private repository.** The private implementation and
archive repositories stay private, and nothing has been extracted from either into this one.
