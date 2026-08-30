# Publication architecture

- **Publication date:** 2026-08-30

**Scope note.** This page describes **how the R-Series publishes** — which repositories exist, what
each one is for, and how large artefacts are distributed. It does **not** describe deployment topology,
infrastructure, hosts, or any internal system architecture, and it never will.

## The shape

> The R-Series publishes through **three existing standard repositories and one new documentation
> portal**. The portal is built from an explicit allow-list; nothing is copied wholesale, and it
> inherits no history. Ceremony artefacts are distributed as **release assets with a SHA-256
> manifest** rather than committed to git.

| Tier | Repository | Rule |
|---|---|---|
| **Public standards** | `r2-standard`, `r3-standard`, `r4-standard` | Public, **history unchanged**. Corrected **by addition only** — banners, status files, errata. No force-push, no history rewrite, no visibility change. |
| **Documentation portal** | `rseries-portal` (this repository) | New, public, allow-listed, no inherited history. |
| **Implementation** | *private* | Stays private. Not published, not mirrored here. |
| **Archive** | *private* | Stays private, permanently. Not published, not scrubbed-and-flipped. |

## One portal, not one repository per layer

**Repository count is not a trust metric.** A reader gains nothing from twelve repositories that
thirteen documents in one repository would not give them, and the maintenance burden of the existing
three is already visible in their commit history. There will be no `r5-standard`, no `r6-standard`, and
so on down the list.

## How this repository was assembled

**Default-exclude, file by file.** A file is in this repository only if it was individually reviewed
and found public-safe. Nothing was copied in bulk from anywhere, and no size target was set — an
earlier estimate of the publishable document count was wrong by roughly ten times in the unsafe
direction, which is exactly what estimating instead of enumerating produces.

Every file here is either newly written, or reproduced verbatim from a repository that is **already
public**, with its source named on the page.

## Large artefacts: release assets, never git

When the ceremony artefacts are published — the constraint system, the witness generator, the powers-of-tau
file, the final proving key, the verifying key, and the per-contribution transcript hashes — they will be
published as **GitHub Release assets with a `SHA256SUMS` manifest and exact verification instructions.
They will never be committed to git history.**

Three reasons, in order of weight:

1. **Git cannot forget.** A multi-gigabyte binary committed once is in every future clone forever, and
   removing it requires a history rewrite — the exact operation this programme has correctly forbidden
   itself. Committing the artefact would create a permanent problem to solve a temporary one.
2. **Release assets are immutable, versioned, and cost nothing for a public repository.** They live
   next to the repository whose history they attest to, with no additional vendor, credential or
   billing dependency for a reader to trust.
3. **Generic object storage introduces an account a reader cannot verify still exists.** It is an
   acceptable second copy for durability. It is not the right primary citation target.

The manifest digest will be mirrored in this portal, and may additionally be anchored on-chain — the
same pattern R+3 already uses — so that the artefact set is tamper-evident without anyone having to
trust the hosting platform.

## What is never published

- Deployment topology, infrastructure inventory, and internal API surfaces.
- Exploit detail of any kind, and any proof artefact demonstrating one.
- Internals of any repaired circuit.
- Internal self-assessments presented as external work.
- Anything from a private repository that has not been individually reviewed as public-safe — which,
  today, is everything in them.
