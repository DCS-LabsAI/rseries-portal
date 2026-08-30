# R-Series Portal

**This repository is a skeleton under construction. It is not yet a published claim surface.**

Nothing here should be read as a finished statement of what the R-Series is or does. The structure
exists; most of the content does not, and the places where content is missing say so by name rather
than filling the gap with a plausible sentence.

- **Publication date of this state:** 2026-08-30
- **Status:** SKELETON — launch gated
- **Launch gate:** the P0 register in [`STATUS.md`](STATUS.md). **Of nine P0 items, two are CLOSED and
  seven remain OPEN** as of 2026-08-30 — one of the seven with its first half closed. Until all nine
  close, this portal does not launch and its pages must not be cited as the R-Series public record.

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
| [`layers/`](layers/README.md) | R+2 and R+3 written · R+4 gated on P0-8 · **[R+5 → R+12 status](layers/STATUS_R5_R12.md)** written |
| [`verification/`](verification/README.md) | Written — what a third party can check today |
| [`conformance/`](conformance/README.md) | Written — pointer |
| [`test-vectors/`](test-vectors/README.md) | Written — pointer |
| [`cryptographic-evidence/`](cryptographic-evidence/README.md) | **Placeholder** — gated on P0-3 and P0-6 |
| [`evidence/long-duration/`](evidence/long-duration/README.md) | **No figure published** — gated on P0-4 |
| [`history/`](history/README.md) | Written — the May 2026 ceremony, preserved exactly |
| [`receipts/`](receipts/README.md) | **Placeholder** — gated on P1-7 |
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
verification status, and **nothing in the R-Series has been externally audited**. This portal remains
a skeleton under construction — reusing a gated or placeholder page does not make its content a
published claim.

## Provenance of this repository

Every file in this repository is either **newly written for it** or **reproduced verbatim from an
already-public repository with its source named on the page**. Exactly one file is a verbatim
reproduction: [`history/r4-v0.1-may-2026.md`](history/r4-v0.1-may-2026.md), which reproduces
`r4-standard/reference/ceremony/CEREMONY_TRANSCRIPT.md`.

**No file in this repository originated from any private repository.** The private implementation and
archive repositories stay private, and nothing has been extracted from either into this one.
