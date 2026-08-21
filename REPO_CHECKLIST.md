# DeSBi repository and release checklist

Complete this checklist for the exact commit that will be tagged as a verified DeSBi release.

## A. Relationship, rights and provenance — hard gate

- [ ] The DeSBi project(s), publication(s) and contribution are identified.
- [ ] The scientific maintainer has approved the official DeSBi fork/mirror.
- [ ] The institutional or repository owner has approved where ownership is not individual.
- [ ] An explicit software licence permits redistribution.
- [ ] The upstream licence and copyright notices are unchanged and complete.
- [ ] The full available commit history is preserved.
- [ ] The canonical upstream repository is linked prominently.
- [ ] No restricted cohort, clinical, personal or otherwise non-redistributable data are included.
- [ ] Third-party model weights, assets and data have compatible terms and attribution.

A release cannot proceed while any item in this section is open.

## B. Scientific identity and citation

- [ ] The README states the scientific question and intended use.
- [ ] Associated paper(s), preprint(s) and benchmark/data records are linked.
- [ ] `CITATION.cff` is valid and names the correct authors.
- [ ] DFG funding is acknowledged as: `Deutsche Forschungsgemeinschaft (DFG), project 459422098, KI-FOR 5363 (DeSBi)`.
- [ ] The relevant DeSBi project number(s) are stated.
- [ ] The preferred citation distinguishes paper citation from software-release citation.
- [ ] ORCID identifiers are included where available and approved.

## C. Installation and reproducibility

- [ ] Installation succeeds in a clean environment.
- [ ] Supported operating system, language and dependency versions are stated.
- [ ] Dependencies are pinned or constrained sufficiently for reproduction.
- [ ] A CPU-compatible smoke test exists, or the GPU/HPC requirement is explicit.
- [ ] A minimal example runs on public or synthetic data.
- [ ] The expected output of the minimal example is shown or automatically checked.
- [ ] Random seeds and non-determinism are documented.
- [ ] External binaries, model weights and downloads have checksums or immutable version references.
- [ ] Paper-specific reproduction steps are separated from the reusable API/tool.

## D. Software quality

- [ ] Automated tests or an automated smoke test pass.
- [ ] CI runs on the default branch.
- [ ] The public API or main command-line entry points are documented.
- [ ] Errors for missing data, weights or dependencies are actionable.
- [ ] No secrets, credentials, internal paths or private endpoints are present.
- [ ] Basic security/dependency scanning is enabled where appropriate.
- [ ] A support route and named maintainers are visible.
- [ ] At least one organization-level backup maintainer exists.

## E. Release object

- [ ] The exact upstream tag or commit is recorded.
- [ ] DeSBi-only changes are listed.
- [ ] The version follows the upstream scheme or `desbi-YYYY.MM.N`.
- [ ] Release notes include installation/test commands and known limitations.
- [ ] The source archive is generated from the verified commit.
- [ ] A persistent archive/DOI is created or the decision to retain an existing canonical DOI is documented.
- [ ] `catalogue.yml` is updated with the release URL, version, DOI and status.
- [ ] Repository description and topics are set consistently.
- [ ] The release is reviewed by a second DeSBi project or coordination reviewer.

## F. Status after release

- [ ] The repository is labelled `verified` in the catalogue.
- [ ] The landing page link resolves.
- [ ] Upstream-sync responsibility and review interval are assigned.
- [ ] A deprecation/successor route is known.
- [ ] Renewal evidence records distinguish this verified release from mere public repositories and release candidates.

## Reviewer record

- **Repository:**
- **Verified commit:**
- **Upstream tag/commit:**
- **DeSBi release tag:**
- **Scientific maintainer:**
- **Independent reviewer:**
- **Verification date:**
- **Environment:**
- **DOI/archive:**
- **Open limitations:**
