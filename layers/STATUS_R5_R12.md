# R+5 → R+12 — layer status

- **Publication date:** 2026-08-30
- **Scope:** five fields per layer, and only five: **purpose · current maturity/status · source
  public/private/dark · public evidence available · next milestone**.

**What this document deliberately does not contain.** No private implementation detail. No internal
architecture. No defect mechanism, exploit detail or proof artefact. No installation instruction and
no package name. Where a field cannot be substantiated from the public repositories or from the
30 August 2026 internal reconciliation, it says **unpublished** or **unproven**. No gap in this
document is filled with a plausible sentence.

**How to read the figures here.** Per [`../CLASSIFICATION.md`](../CLASSIFICATION.md): no bare counts,
the population is named in the same sentence, and what is true *today* of an artefact is printed apart
from what the layer is intended to cover *eventually*. Run dates and publication dates are printed
separately.

**Nothing in this document is externally audited.** No independent third-party security audit of any
R-Series layer has been performed.

---

## R+5 — Federation (cross-issuer verification)

| Field | Statement |
|---|---|
| **Purpose** | Extend R+2 receipt verification across multiple independent issuers, using a signed federation manifest as the trust anchor. It introduces no new cryptographic primitives — it inherits R+2's Ed25519 + RFC 8785 (JCS) model and adds exactly one new trust anchor: the authority that signs the manifest. |
| **Current maturity / status** | **Operational prototype.** The normative specification section and the cross-issuer conformance vectors are public and exercised by public CI. A multi-node reference prototype exists in the public R+4 repository. **Multi-organisation federation across organisations outside DCS Labs is unproven** — every federation participant on the internal record is a DCS-operated node. |
| **Source** | **Public**, for the specification section, the six cross-issuer conformance vectors and the multi-node reference prototype. **Private**, for the internal federation service and its trust-algebra component, which are not published and are not required to use the public specification. |
| **Public evidence available** | `r2-standard/spec/SPEC_R5_FEDERATION.md` and `r2-standard/conformance/federation-vectors/f01`–`f06` — **6 of 6 vectors public**, mostly negative cases, run by that repository's CI. Classification: **PUBLIC-REPRODUCIBLE.** One qualification, published rather than omitted: a federation end-to-end test in the public R+4 reference **cannot run as shipped**, because a fixture it needs is not committed. Any count cited for that particular suite is therefore not reproducible today, and no such count is printed in this portal. |
| **Next milestone** | Commit the missing fixture or withdraw the count that depends on it. Then demonstrate a federation in which at least one issuer is operated by an organisation outside DCS Labs, and publish that demonstration's artefacts. Until that happens, "federation" means the specification and its vectors, not a running multi-organisation network. |

---

## R+6 — Agent Economy

| Field | Statement |
|---|---|
| **Purpose** | Receipt-backed reputation and agent-to-agent contract state. Settlement is recorded as **intent only**; no value is transferred. |
| **Current maturity / status** | **Internal. Not public.** Value-movement paths are dark by design and by standing directive. There is no protocol artefact here that a third party could implement against — the internal component is a small state machine, not a specification. |
| **Source** | **Dark.** Not published, and no publication decision has been taken. |
| **Public evidence available** | **None.** No specification, no vectors, no records, no figures. Classification: **INTERNAL-ONLY.** |
| **Next milestone** | **Unpublished.** No milestone for this layer is published, because none has been committed to. Publishing an unsettled economic design would invite third parties to build on semantics DCS Labs has not fixed. |

---

## R+7 — Sovereign Memory

| Field | Statement |
|---|---|
| **Purpose** | Provenance and hard-erasure receipts for agent memory — a record that an erasure actually occurred, rather than a soft delete. |
| **Current maturity / status** | **Internal. Not ready to be public in any form.** The 30 August 2026 internal reconciliation records a specific, named, unresolved defect on this layer's write path, and a legacy path that is still present alongside the corrected one. The mechanism is deliberately not described here. Publishing the design in this state would publish the defect. |
| **Source** | **Private.** |
| **Public evidence available** | **None.** Classification: **INTERNAL-ONLY.** |
| **Next milestone** | Close the recorded write-path defect and remove the legacy path. Only then is a publication decision for this layer even in scope. No date is published. |

---

## R+8 — Governance

| Field | Statement |
|---|---|
| **Purpose** | Receipted policy evaluation and approval — recording governance decisions as verifiable receipts, with policy expressed in a restricted, non-executing decision language. |
| **Current maturity / status** | **Internal. Not public.** The same class of unresolved write-path defect recorded for R+7 applies here. One component — the argument for why the policy language cannot execute arbitrary code — is identified internally as potentially worth publishing as a specification later. It is **not published now**, because no adversarial test suite in the reviewed source backs the figure that has been asserted for it elsewhere. **That figure is therefore not printed in this portal.** |
| **Source** | **Private.** |
| **Public evidence available** | **None.** Classification: **INTERNAL-ONLY.** |
| **Next milestone** | Close the write-path defect. Build and run an adversarial suite against the policy language before any figure about it is published, and publish the suite alongside any figure it produces. |

---

## R+9 — Quantum Trust

| Field | Statement |
|---|---|
| **Purpose** | **No publishable statement.** |
| **Current maturity / status** | **UNSUBSTANTIATED — NOT CARRIED.** Locked as a rights-holder decision on 2026-08-30, pending evidence reconciliation. The 30 August 2026 internal reconciliation found this layer's claim **unsubstantiated in both public and private scope** — the only claim in that review that failed in both directions. R+9 is therefore not carried as a published R-Series layer. It is listed here so that the numbering has no silent gap, and for no other reason. The decision is revisited only if an evidence reconciliation produces evidence; it is not revisited by re-asserting the claim. |
| **Source** | Not applicable. Nothing is published, and nothing is asserted. |
| **Public evidence available** | **None.** Classification: **UNPROVEN** — evidence not located. This is not a statement that the work did not happen; it is a statement that no evidence supporting the layer as a layer was located in either scope. |
| **Next milestone** | **Unpublished.** This layer is not carried as a published R-Series layer, and no milestone is claimed for it. Any future publication would start from evidence, not from the existing claim. |

---

## R+10 — Interoperability / Fabric

| Field | Statement |
|---|---|
| **Purpose** | Project R+2 receipts into third-party provenance and credential formats, so that a receipt can be consumed by ecosystems that do not implement R+2 — including IETF SCITT signed statements, C2PA manifests, and W3C Verifiable Credentials. |
| **Current maturity / status** | **Internal prototype**, plus one shim published on the npm registry. The bridge components are format projections, not a standard. The internal reconciliation records that the SCITT bridge component is **executed by no test and no CI job**, and that a live round-trip against an independent third-party implementation **has not been performed**. On that basis the bridge is not offered as a reference implementation. |
| **Source** | **Private**, except the published npm shim. |
| **Public evidence available** | The published npm shim. **No conformance vectors and no test evidence are published for this layer, and no figure is printed here.** Classification: **INTERNAL-ONLY** for the bridge; **PUBLIC-CHECKABLE** only for the bare fact that a shim package exists. **The package name is deliberately not printed in this portal** — one canonical npm scope has not yet been fixed, and this portal publishes no installation instruction until it is. See [`../security/README.md`](../security/README.md). |
| **Next milestone** | Complete a live SCITT round-trip against an independent implementation and publish it. Publish the format mapping with its scope note. Fix and announce one canonical package scope, then — and only then — publish install instructions. |

---

## R+11 — Confidential Compute

| Field | Statement |
|---|---|
| **Purpose** | Bind a receipt to an attestation of the environment that produced it, so that a relying party can distinguish a computation that ran in an attested environment from one that claims it did. |
| **Current maturity / status** | **Experimental. Internal. Not ready to be public in any form.** Its test suite is **upheld**: re-executed on **2026-08-30**, **31 of the 31 assertions in that suite passed, exit code 0**, from a package dated **2026-07-23**. That is what is true *today* of the suite. What is **eventually** claimed for the layer — verifiable confidential compute — is **not covered by that suite**: no trusted-execution hardware has ever been used in this programme, so the layer's central claim cannot be verified inside it. |
| **Source** | **Private.** The package is a separate package; it is **not part of the R-Series reference core**, and it is not published. |
| **Public evidence available** | **None.** The 31-of-31 result is an **internal result**, not a publicly reproducible one, because the package that produces it is unpublished. Classification: **PUBLISHED-EVIDENCE-ONLY.** Run date **2026-08-30** · publication date of this statement **2026-08-30** · package date **2026-07-23**. |
| **Next milestone** | Publish the package — it has no external dependencies, and publishing it would make the figure publicly reproducible in a single step — or stop citing the figure. Separately, obtain access to real attestation hardware before any claim about *attested* execution is made at all. |

---

## R+12 — Provenance Fabric

| Field | Statement |
|---|---|
| **Purpose** | A cross-domain provenance passport: carry receipt lineage across domain boundaries in a form that can be verified offline. |
| **Current maturity / status** | **Experimental. Internal. Not ready to be public in any form.** Its test suite is **upheld**: re-executed on **2026-08-30**, **33 of the 33 assertions in that suite passed, exit code 0**, from a package dated **2026-07-23**. That is what is true *today* of the suite. It is **not** a statement that a cross-domain passport has been verified by any party outside DCS Labs — none has. |
| **Source** | **Private.** A separate package, **not part of the R-Series reference core**, not published. |
| **Public evidence available** | **None publicly reproducible.** Classification: **PUBLISHED-EVIDENCE-ONLY.** Run date **2026-08-30** · publication date of this statement **2026-08-30** · package date **2026-07-23**. **One defect in the existing evidence record is disclosed rather than repeated:** the previously published record for this layer carries an **incorrect repository and commit attribution** — it names a repository that does not contain the suite — and a **null suite-file hash**. That record is **not linked from this portal and is not cited as evidence here**, and the incorrect attribution is **not reproduced**. Correcting the record is an open item. |
| **Next milestone** | Correct the evidence record's repository/commit attribution and its suite-file hash. Then publish the package so the figure becomes publicly reproducible, or stop citing the figure. |

---

## Summary

| Layer | Source | Public evidence | Publicly reproducible today |
|---|---|---|---|
| R+5 Federation | Public spec + vectors · private service | Spec section, 6 of 6 cross-issuer vectors | **Yes**, for the vectors |
| R+6 Agent Economy | Dark | None | No |
| R+7 Sovereign Memory | Private | None | No |
| R+8 Governance | Private | None | No |
| R+9 Quantum Trust | — (omitted; unsubstantiated) | None | No |
| R+10 Interop / Fabric | Private, except one npm shim | The shim's existence only | No |
| R+11 Confidential Compute | Private | None | No — internal result only |
| R+12 Provenance Fabric | Private | None | No — internal result only |

**One layer of the eight has public evidence a third party can act on today.** That is the honest
shape of R+5 → R+12, and it is stated here rather than left to be inferred.
