# Public repository audit and fork plan

**Audit date:** 2026-08-21  
**Scope:** public GitHub/GitLab repositories, the official DeSBi site, publication code links and the current renewal materials.

## Decision principle

A repository becomes an **official DeSBi release** only when three conditions hold:

1. the relationship to DeSBi is documented and approved by the maintainers;
2. the licence permits redistribution and the original copyright/provenance is preserved;
3. a specific commit is tested, versioned, described and archived as a citable research release.

A raw fork is therefore an intake mechanism, not the final product.
## Wave 1 — forkable after maintainer sign-off
| Output | Projects | Purpose | Upstream | Licence | Readiness | Required before release |
|---|---|---|---|---|---|---|
| **DNCIT** | P1 | Deep nonparametric conditional-independence testing for images and other high-dimensional modalities. | [DNCIT](https://github.com/MSimnach/DNCIT) | `GPL-3.0-or-later` | high | Obtain maintainer sign-off; fork with full history; add CITATION.cff and an archived DeSBi snapshot. |
| **quanda** | P2 | Toolkit for quantitative evaluation of training-data attribution methods. | [quanda](https://github.com/dilyabareeva/quanda) | `MIT` | high | Obtain maintainer sign-off; fork and retain upstream as the canonical development home. |
| **transferGWAS** | P1, P2, P4, P5 | Embed-then-test genome-wide association analysis for whole medical images. | [transferGWAS](https://github.com/mkirchler/transferGWAS) | `MIT` | medium | Obtain owner sign-off; fork; add current environment lockfiles and clearly separate reusable method code from paper-specific reproduction code. |
| **MFD** | P1, P4, P5 | Metadata-guided feature disentanglement for functional genomics. | [MFD](https://github.com/HealthML/MFD) | `MIT` | medium | Obtain owner sign-off; fork; add citation metadata, a small runnable example and CI for the core method. |
| **SemanticLens** | P2 | Semantic interpretation and validation of components in large vision models. | [semanticlens](https://github.com/jim-berend/semanticlens) | `BSD-3-Clause` | high | Confirm DeSBi release attribution with all maintainers; fork without changing the canonical package identity. |
| **DualXDA** | P2 | Sparse, efficient and feature-explainable attribution of predictions to training samples. | [DualXDA](https://github.com/gumityolcu/DualXDA) | `BSD-3-Clause-Clear` | high | Confirm DeSBi attribution and the intended replacement of DualView; fork the maintained successor only. |

## Licensed but governance approval required
| Output | Projects | Upstream | Licence | Governance issue | Recommendation |
|---|---|---|---|---|---|
| **EmmaEmb** | P5 | [EmmaEmb](https://github.com/broadinstitute/EmmaEmb) | `MIT` | Technically forkable, but institutional ownership and multi-consortium provenance make governance approval essential. | Prefer a catalogue link unless the Broad Institute maintainers explicitly approve an official DeSBi fork and release label. |

## Wave 2 — public repository, cleanup first
| Output | Projects | Upstream | Blocking issue | Required action |
|---|---|---|---|---|
| **PLRP** | P5 | [plrp](https://gitlab.com/dacs-hpi/plrp) | GitLab import plus licence validation | Validate or add an explicit licence, confirm owners, then import or mirror the GitLab repository while preserving full history. |
| **Arctique** | P3 | Procedurally generated histopathology benchmark with controllable image and label uncertainty. | [arctique](https://github.com/Kainmueller-Lab/arctique) | `GPL-3.0` | high | Obtain maintainer sign-off; fork; document the relation between code, generated data and data licences. |
| **DeepRepViz** | P7 | Visualization and Con-score diagnostics for confounder encoding in deep representations. | [DeepRepViz](https://github.com/RoshanRane/DeepRepViz) | `BSD-4-Clause` | medium | Obtain maintainer sign-off; fork; add automated smoke tests, citation metadata and a versioned release. |
| **Toybrains** | P7, P1 | Synthetic neuroimaging-inspired benchmark with a controllable causal data-generating graph. | [toybrains](https://github.com/RoshanRane/toybrains) | `GPL-3.0` | high | Obtain maintainer sign-off; fork; preserve the existing canonical Zenodo citation and record the upstream commit used for the DeSBi snapshot. |
| **Reveal2Revise** | P2 | [Reveal2Revise](https://github.com/maxdreyer/Reveal2Revise) | No explicit reusable-software licence was confirmed | Add an explicit licence and funding/citation metadata upstream before forking. |
| **PCX** | P2 | [pcx](https://github.com/maxdreyer/pcx) | No explicit reusable-software licence was confirmed | Add an explicit licence, citation metadata and a minimal reproducible example before forking. |
| **Reactive correction / R-ClArC** | P2 | [reactive_correction](https://github.com/dilyabareeva/reactive_correction) | No explicit reusable-software licence was confirmed | Add an explicit licence and a release-level README that identifies the associated paper and DeSBi contribution. |
| **PURE** | P2 | [PURE](https://github.com/maxdreyer/PURE) | No explicit reusable-software licence was confirmed | Add an explicit licence, citation metadata and a stable environment before forking. |
| **Probabilistic / pattern CAV framework** | P2 | [cav-unifying-view-adversarial](https://github.com/jawhar00/cav-unifying-view-adversarial) | No explicit reusable-software licence was confirmed | Add an explicit licence and stable release metadata before forking. |
| **RR-ClArC / latent-space bias unlearning** | P2 | [rrclarc](https://github.com/frederikpahde/rrclarc) | No explicit reusable-software licence was confirmed | Add an explicit licence and citation/funding metadata before forking. |
| **TW-autoencoder** | P3, P2 | [TW-autoencoder](https://github.com/Kainmueller-Lab/TW-autoencoder) | No explicit reusable-software licence was confirmed | Add an explicit licence, installation instructions and a small demonstration before forking. |
| **transfer-gwas-brain-mri** | P1, P2, P4, P5 | [transfer-gwas-brain-mri](https://github.com/HealthML/transfer-gwas-brain-mri) | No licence confirmed; supplementary/thin repository | Do not make this a flagship fork yet; first decide whether its content should be merged into or linked from the main transferGWAS release. |
| **medical-ai-safety** | P2 | [medical-ai-safety](https://github.com/frederikpahde/medical-ai-safety) | DeSBi relationship and licence both require confirmation | Confirm that the repository is a DeSBi output and add an explicit licence before considering a fork. |

## Wave 3 — publish or locate the implementation
| Named output | Projects | Intended role | Public-repository result | Next action |
|---|---|---|---|---|
| **BaGGLS** | P5, P6 | Bayesian overlapping-group shrinkage implementation. | No unambiguous public repository located in this audit | Identify the maintained codebase, publish it with a licence and citation metadata, then create the first DeSBi release. |
| **abamlss variational-inference framework** | P5 | Scalable variational inference for GAMLSS/SADR models. | No unambiguous public repository located in this audit | Confirm the canonical package/repository and whether it is already public under another name; publish or catalogue accordingly. |
| **AttnLRP adaptation for DNABERT-2** | P5 | Architecture-aware relevance propagation for genome language models. | No unambiguous public repository located in this audit | Publish the DeSBi adaptation rather than forking a generic LXT or DNABERT-2 dependency repository. |
| **Post-hoc orthogonalisation (PHO)** | P5, P7 | Post-hoc orthogonalisation for separating structured effects from learned representations. | No unambiguous public repository located in this audit | Identify and package the shared implementation, including a minimal example and tests. |
| **XAI evaluation toolkit** | P4, P5 | Shared benchmarking and visualisation harness for explanation methods in genomics. | No unambiguous public repository located in this audit | Resolve the final repository name and publication status, then publish the shared toolkit. |
| **ICON Decomposition** | P7, P1, P4 | Orthogonal concept directions for screening deep representations for shortcuts and biases. | No unambiguous public repository located in this audit | Publish the project implementation; do not confuse it with unrelated repositories named ICON. |
| **CovLRP and second-order uncertainty explanations** | P2, P3 | Second-order explanation methods for predictive uncertainty. | No unambiguous public repository located in this audit | Locate or publish the paper implementation with a licence and reproducibility instructions. |
| **Control-variable / omitted-variable-bias correction** | P7 | Confounder-aware deep learning that separates omitted-variable bias from mediated effects. | No unambiguous public repository located in this audit | Publish a reusable implementation and the simulation/benchmark pipeline. |
| **Explainable deep test statistics** | P1, P2 | Sample- and feature-level explanations for deep two-sample and related statistical tests. | No unambiguous public repository located in this audit | Consolidate the paper implementations into one citable package or clearly catalogue separate repositories. |
| **Counterfactual explanations for deep tests** | P1, P2 | Plausible sample-level edits that reduce distributional discrepancies measured by deep tests. | No unambiguous public repository located in this audit | Publish the accepted-paper implementation when author and institutional approvals are complete. |

## Do not fork
| Item | Reason | Action |
|---|---|---|
| **DualView** | The repository itself states that it is outdated. | Catalogue only as historical provenance and direct users to DualXDA. |
| **Generic dependencies** | General-purpose projects used by DeSBi code, such as Captum, LXT, DNABERT-2 or generic CRP libraries. | Reference them as dependencies; do not brand them as DeSBi releases. |
## Recommended first public release set

For the renewal, the most convincing initial set is:

1. **DNCIT** — direct evidence of the core statistical-inference contribution;
2. **quanda** — mature, reusable evaluation infrastructure;
3. **SemanticLens** — polished concept-level/mechanistic interpretation software;
4. **MFD** — a cross-project genomics output;
5. **transferGWAS** — a recognizable embed-then-test application pipeline;
6. **DualXDA** — a maintained successor for data attribution.

The profile page can show all, while the organization should pin a balanced subset spanning inference, explanation, uncertainty, confounding, simulation and genomics.

## Five-day rollout for renewal evidence

### Day 1 — approvals and namespace

- Send one standardized approval message to each first-wave maintainer.
- Create the `.github` and `software-catalogue` repositories.
- Add the organization description, website and project metadata.
- Create the nine forks, but label them **release candidates** until the checklist is complete.

### Day 2 — visible landing page

- Publish the organization profile.
- Add consistent repository descriptions and topics.
- Pin six repositories representing different methodological strands.
- Add a short DeSBi provenance block to each fork without overwriting the upstream README.

### Day 3 — verified release core

Prioritize DNCIT, quanda and SemanticLens. For each:

- record the upstream tag/commit;
- run the installation and minimal example;
- add or verify `CITATION.cff`;
- create a `desbi-2026.08.1` curated snapshot tag;
- publish release notes and archive appropriately.

### Day 4 — cross-project evidence and blockers

- Prepare MFD, transferGWAS and DualXDA.
- Open upstream issues or pull requests for Wave-2 licences rather than silently adding licences only in the forks.
- Assign every “publish required” output to a project PI/maintainer with a due date and repository decision.

### Day 5 — renewal documentation

- Capture a clean screenshot of the organization overview and the software catalogue.
- Add the organization and catalogue links to the Mantel software/reproducibility text.
- Report separate counts for **public repositories**, **verified DeSBi releases**, and **outputs in release preparation**; do not collapse these categories.
- Freeze the audit date in the proposal evidence package.

## Risks to avoid

- **Blind mass-forking:** creates an impressive count but weakens credibility if repositories lack licences, documentation or relation to DeSBi.
- **Re-licensing in the fork:** a fork must retain the upstream licence; licensing gaps must be resolved by the rights holders.
- **Duplicate canonical packages:** do not publish a fork to PyPI/CRAN under the same package name unless the upstream maintainers explicitly agree.
- **Duplicate DOIs:** preserve an existing canonical software DOI when a DeSBi snapshot adds no materially distinct release.
- **Restricted biomedical data:** release code, synthetic examples and access instructions—not clinical or cohort data that cannot legally be redistributed.
- **Orphan forks:** every official release needs at least one scientific maintainer and one organization-level backup.
