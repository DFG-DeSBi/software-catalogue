# DeSBi software catalogue

This repository is the authoritative index of software, benchmarks and reusable methodological infrastructure associated with the DeSBi Research Unit.

## Status model

| Status | Meaning |
|---|---|
| **Fork now** | Public, explicitly licensed and technically suitable for a first-wave fork, subject to maintainer approval and release checks. |
| **Owner approval** | Technically suitable, but institutional or multi-consortium ownership requires explicit governance approval. |
| **Cleanup first** | Public code exists, but licensing, provenance or packaging blocks an official release. |
| **Publish required** | A reusable output is named in DeSBi materials, but no unambiguous public repository was located. |
| **Do not fork** | Superseded, external or otherwise unsuitable for DeSBi branding. |

## Second-wave candidates

| Output | Research role | Upstream | Licence |
|---|---|---|---|
| quanda | Evaluation of training-data attribution | [dilyabareeva/quanda](https://github.com/dilyabareeva/quanda) | MIT |
| Arctique | Histopathology uncertainty benchmark | [Kainmueller-Lab/arctique](https://github.com/Kainmueller-Lab/arctique) | GPL-3.0 |
| DeepRepViz | Confounder diagnostics | [RoshanRane/DeepRepViz](https://github.com/RoshanRane/DeepRepViz) | BSD-4-Clause |
| Toybrains | Causal synthetic benchmark | [RoshanRane/toybrains](https://github.com/RoshanRane/toybrains) | GPL-3.0 |

“Fork now” does **not** mean “brand without asking.” Written maintainer approval and the release checklist are still required.

## Files

- [`catalogue.yml`](catalogue.yml) — machine-readable audit.
- [`REPOSITORY_INVENTORY.md`](REPOSITORY_INVENTORY.md) — detailed findings, blockers and recommended waves.
- [`RELEASE_POLICY.md`](RELEASE_POLICY.md) — governance and versioning rules.
- [`REPO_CHECKLIST.md`](REPO_CHECKLIST.md) — release gate.
- [`CONTRIBUTING.md`](CONTRIBUTING.md) — how to nominate or update an output.
- [`templates/`](templates/) — drop-in provenance, citation and release-note templates.

## Audit date and maintenance

Audit date: **2026-09-07**. Re-run the audit before the renewal review and then at least twice per year. Repository metadata changes quickly; `catalogue.yml` records the current decision, not an eternal truth.
