# DeSBi software catalogue

This repository is the authoritative index of software, benchmarks and reusable methodological infrastructure associated with the DeSBi Research Unit.

## Curated DeSBi releases (v1.0.0, desbi-2026.09.1)

| Output | Research role | Upstream | Licence |
|---|---|---|---|
| DNCIT | Deep nonparametric conditional-independence tests for images | [MSimnach/DNCIT](https://github.com/MSimnach/DNCIT) | GPL-3.0 |
| transferGWAS | Image-based genome-wide association studies using deep transfer learning | [mkirchler/transferGWAS](https://github.com/mkirchler/transferGWAS) | MIT |
| DualXDA | Sparse and explainable training-data attribution | [gumityolcu/DualXDA](https://github.com/gumityolcu/DualXDA) | BSD-3-Clause-Clear |
| cocodeel | Control-variable adjustment for deep neural networks | [mpff/cocodeel](https://github.com/mpff/cocodeel) | MIT |
| Pathology Foundation Model Benchmark | Pathology foundation-model benchmark for cell phenotyping | [Kainmueller-Lab/Pathology-Foundation-Model-Benchmark](https://github.com/Kainmueller-Lab/Pathology-Foundation-Model-Benchmark) | MIT |
| MFD | Metadata-guided feature disentanglement for functional genomics | [HealthML/MFD](https://github.com/HealthML/MFD) | MIT |
| SemanticLens | Mechanistic interpretation and validation of large vision models | [jim-berend/semanticlens](https://github.com/jim-berend/semanticlens) | BSD-3-Clause |
| RR-ClArC | Concept-level model correction to reduce bias sensitivity | [frederikpahde/rrclarc](https://github.com/frederikpahde/rrclarc) | BSD-3-Clause |
| UDBench | Semi-synthetic benchmark for uncertainty disentanglement | [WizgallF/udbench-benchmark](https://github.com/WizgallF/udbench-benchmark) | MIT |
| dnn-shapes | Deep shape regression for planar curves with multimodal covariates | [mpff/dnn-shapes](https://github.com/mpff/dnn-shapes) | MIT |

## Status model

| Status | Meaning |
|---|---|
| **Fork now** | Public, explicitly licensed and technically suitable for a first-wave fork, subject to maintainer approval and release checks. |
| **Owner approval** | Technically suitable, but institutional or multi-consortium ownership requires explicit governance approval. |
| **Cleanup first** | Public code exists, but licensing, provenance or packaging blocks an official release. |
| **Publish required** | A reusable output is named in DeSBi materials, but no unambiguous public repository was located. |
| **Do not fork** | Superseded, external or otherwise unsuitable for DeSBi branding. |

## Second-wave candidates

| Output | DeSBi project(s) | Research role | Upstream | Licence | Current status / next action |
|---|---|---|---|---|---|
| PLRP | P5 | Pruned Layer-wise Relevance Propagation | [dacs-hpi/plrp](https://gitlab.com/dacs-hpi/plrp) | GPL-3.0 | Verified release review. Prepare a documented GitLab-to-DeSBi mirror. |
| quanda | P2, P3, P4 | Evaluation of training-data attribution | [dilyabareeva/quanda](https://github.com/dilyabareeva/quanda) | MIT | Release candidate. |
| PURE | P2, P3, P4 | Identifying relevant circuits to turn polysemantic neurons into pure features | [maxdreyer/PURE](https://github.com/maxdreyer/PURE) | BSD 3-Clause | Release candidate. |
| pcx | P2, P3, P4 | Explainability research output | [maxdreyer/pcx](https://github.com/maxdreyer/pcx) | BSD 3-Clause | Release candidate. |
| Uncertainty Aggregation (Aggrigator) | P3 | Spatially aware aggregation of segmentation uncertainty | [Kainmueller-Lab/aggrigator](https://github.com/Kainmueller-Lab/aggrigator) | MIT | Release candidate. |

## Catalogue-only repositories

| Output | DeSBi project(s) | Research role | Upstream | Licence | Current status / next action |
|---|---|---|---|---|---|
| LRP-eXplains-Transformers | P2 | Transformer explainability | [DFG-DeSBi/LRP-eXplains-Transformers](https://github.com/DFG-DeSBi/LRP-eXplains-Transformers) | Clear BSD | Catalogue only. |
| zennit | P2, P5 | Layer-wise relevance propagation framework | [DFG-DeSBi/zennit](https://github.com/DFG-DeSBi/zennit) | No explicit upstream licence recorded | Catalogue only; obtain an explicit upstream licence and approval before any release review. |
| explain_dnabert2 | P5 | Explainability for DNABERT2 | [dacs-hpi/explain_dnabert2](https://gitlab.com/dacs-hpi/explain_dnabert2) | No explicit upstream licence | Catalogue only; not eligible for release review until an upstream licence and approval are recorded. |
| Toybrains | P7, P1 (confirm) | Causal synthetic benchmark | [RoshanRane/toybrains](https://github.com/RoshanRane/toybrains) | GPL-3.0 | Catalogue only. A DeSBi fork exists, but nomination and written maintainer approval are still required before release review. |
| Arctique | P3 (confirm) | Histopathology uncertainty benchmark | [Kainmueller-Lab/arctique](https://github.com/Kainmueller-Lab/arctique) | GPL-3.0 | Catalogue only. A DeSBi fork exists, but nomination and written maintainer approval are still required before release review. |
| DeepRepViz | P7 (confirm) | Confounder diagnostics | [RoshanRane/DeepRepViz](https://github.com/RoshanRane/DeepRepViz) | BSD-4-Clause | Catalogue only. A DeSBi fork exists, but nomination and written maintainer approval are still required before release review. |

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
