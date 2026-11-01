# Requirements traceability

## Scope and sources

This index records confirmed placeholder scope and documentation maintenance
constraints for `cargo-binpack`. It does not approve product ideas or infer
functionality from the repository name. Naming and product scope remain
undecided. Windows-local prototypes and notes are not present and were not
reviewed; they provide no evidence for this index.

The source baseline is repository revision
[`4d4b99389989b08d986801e60b993fd75f0690c5`](https://github.com/rustcommons/cargo-binpack/tree/4d4b99389989b08d986801e60b993fd75f0690c5),
particularly its [primary guidance](https://github.com/rustcommons/cargo-binpack/blob/4d4b99389989b08d986801e60b993fd75f0690c5/AGENTS.md).
The current [AGENTS.md](../AGENTS.md) records the documentation audit's maintenance
constraints. The [shared conventions](https://github.com/rustcommons/.github/blob/main/docs/DOCUMENTATION.md)
are being established centrally; final shared-link validation and merge depend on
that document landing on `main`.

“Verified” below means only the named source inspection supports the stated
constraint in this documentation revision. It does not verify runtime behavior,
external files, future compliance, or a published package. There is no approved
functional requirement set, manifest, binary, build workflow, or automated test
suite in the inspected baseline.

## Requirements

| ID | Requirement and source | Implementation / documentation | Verification evidence | Status and gaps |
| --- | --- | --- | --- | --- |
| CB-REQ-001 | Preserve placeholder scope; do not infer capabilities or rename the repository without an explicit task. Source: baseline AGENTS.md, Project scope. | [README](../README.md); [project scope](../AGENTS.md#project-scope). | Baseline tracked-file inspection (`git ls-tree -r --name-only 4d4b99389989b08d986801e60b993fd75f0690c5`) and current README/AGENTS scope review identify documentation, license, and ignore rules only. | Verified. Product naming and scope remain undecided; local prototypes and notes are unreviewed. |
| CB-REQ-002 | Keep AGENTS.md primary and CLAUDE.md an import shim without duplicate rules. Source: baseline AGENTS.md and CLAUDE.md. | [AGENTS](../AGENTS.md); [CLAUDE](../CLAUDE.md). | Compare CLAUDE.md with the baseline (`git diff 4d4b99389989b08d986801e60b993fd75f0690c5 -- CLAUDE.md`); its exact contents remain unchanged and import AGENTS.md. | Verified. Evidence covers instruction-file contents only. |
| CB-REQ-003 | Keep documentation aligned with confirmed scope and record missing evidence explicitly. Source: AGENTS.md, Working conventions and Documentation and requirements traceability. | [README](../README.md); this index, Scope and sources. | Review README and this index against the baseline file inventory and AGENTS scope: no installation, runtime, compatibility, or test outcome claims are supplied. | Verified. Future ideas are not approved requirements; external prototypes remain outside reviewed evidence. |
| CB-REQ-004 | Maintain stable repository-scoped requirement IDs and update affected documentation and trace links together. Source: AGENTS.md, Documentation and requirements traceability. | This index; [README links](../README.md); [shared guidance](../AGENTS.md#documentation-and-requirements-traceability). | Inspect this table for unique CB-REQ numeric IDs and README/AGENTS links to it. No requirement IDs existed in the baseline. | Verified. This checks the initial index only; future edits require renewed review. |
| CB-REQ-005 | Validate documentation with source, command, link, rendering, and diff checks; avoid unrelated builds. Source: AGENTS.md, Repository layout and validation and Documentation and requirements traceability. | [Validation guidance](../AGENTS.md#repository-layout-and-validation); this index, Maintenance. | Source inspection confirms documentation-only scope and no defined build/test commands in the baseline. No runtime checks are prescribed for this placeholder. | Verified. Source inspection verifies the documented validation constraint only; final central-link validation remains pending. |
| CB-REQ-006 | Preserve the existing license. Source: baseline AGENTS.md, Repository layout and validation. | [LICENSE](../LICENSE). | Compare LICENSE with baseline (`git diff 4d4b99389989b08d986801e60b993fd75f0690c5 -- LICENSE`): unchanged. | Verified. Evidence is limited to preservation of the existing file. |
| CB-REQ-007 | Runtime implementation and verification are outside the confirmed placeholder scope. Source: baseline AGENTS.md, Project scope and Repository layout and validation. | No runtime implementation or validation is established. | Not applicable; no builds, installs, or runtime tests apply to this documentation audit. | Not applicable. A future approved scope and actual implementation would require their own requirements and evidence. |

## Documentation map

| Document | Purpose |
| --- | --- |
| [README.md](../README.md) | Public placeholder scope, setup limitations, and guide links. |
| [AGENTS.md](../AGENTS.md) | Primary repository scope, maintenance, validation, and Git conventions. |
| [CLAUDE.md](../CLAUDE.md) | Unchanged import shim for primary guidance. |
| [docs/REQUIREMENTS.md](REQUIREMENTS.md) | Confirmed constraints, sources, bounded evidence, and gaps. |
| [LICENSE](../LICENSE) | Existing license text. |
| [Shared documentation conventions](https://github.com/rustcommons/.github/blob/main/docs/DOCUMENTATION.md) | Central conventions; final link validation awaits central merge. |

No maintained setup guide, roadmap, release record, or runtime validation report
exists in the inspected repository. Do not create such claims from unreviewed
local material or interpret future ideas as approved requirements.

## Maintenance

Preserve `CB-REQ-001` through `CB-REQ-007`. Assign the next unused numeric suffix
for newly confirmed requirements; never renumber or reuse an ID. Keep retired IDs
with their rationale. Record the actual source before adding a product requirement.

Use only these status categories: Verified (with bounded named evidence),
Implemented—partial verification, Planned, Deferred, and Not applicable. Planned
or deferred work requires a confirmed source; an idea alone is not a requirement.
Update affected rows, README links, and primary guidance together. Identify exact
revisions or versions for historical evidence without rewriting past outcomes.

For documentation-only changes, inspect source and command claims, resolve local
links and anchors, review rendered Markdown, and run `git diff --check`. Check
external links, recording pending shared targets explicitly. Repeat final shared
link checks after the central conventions merge, and obtain independent approval
before merging this repository's documentation PR. No builds or installs apply to
this placeholder audit.
