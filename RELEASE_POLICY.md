# DeSBi software release policy

## 1. Purpose

The DeSBi GitHub organization provides a durable, research-unit-level catalogue and curated releases of software produced through DeSBi projects. It does not erase project ownership or replace healthy upstream development communities.

## 2. Definitions

- **Upstream repository:** the original or canonical development repository controlled by the authors or their institution.
- **DeSBi fork/mirror:** a provenance-preserving copy in the `dfg-desbi` organization.
- **Release candidate:** a fork or imported repository undergoing legal, metadata and reproducibility checks.
- **Verified DeSBi release:** a specific tested commit that has passed the repository checklist and is published as a versioned GitHub release.
- **Archived release:** a verified release that is no longer actively maintained but remains available and citable.

A fork is not automatically a release.

## 3. Admission criteria

An output may enter the organization when:

1. its relationship to a DeSBi project, publication or funded activity is documented;
2. the scientific maintainer and relevant repository/institutional owner approve the DeSBi fork or mirror;
3. redistribution is allowed by an explicit software licence;
4. no confidential, personal, clinical, cohort-restricted or otherwise non-redistributable data are included;
5. at least one scientific maintainer and one organization-level backup are named.

Repositories that fail one of these criteria remain catalogue entries with a blocker; they are not branded as official releases.

## 4. Provenance and intellectual property

Every fork or mirror must:

- preserve the full available commit history;
- retain the upstream licence, copyright notices and contributor history;
- link prominently to the canonical upstream repository;
- state whether development occurs upstream or in the DeSBi organization;
- identify modifications made only in the DeSBi fork;
- avoid adding a new licence where the rights holders have not licensed the upstream code.

Licence gaps should be fixed upstream by the rights holders. A DeSBi fork may not manufacture permission retroactively.

## 5. Minimum repository content

A verified release requires:

- a clear README with scientific purpose, installation, quick start and expected output;
- an explicit `LICENSE` file or package-level licence declaration;
- `CITATION.cff` and links to the associated paper(s);
- a DeSBi provenance block naming project(s), funding and upstream;
- a reproducible environment (`pyproject.toml`, lockfile, `environment.yml`, `renv.lock`, container or equivalent);
- a minimal example using public or synthetic data;
- automated tests or, for complex pipelines, at least an automated smoke test;
- a changelog or release notes;
- a statement on data availability and restrictions;
- named maintainers and a support/issue route.

## 6. Release classes

### Incubating

Public and linked to DeSBi, but one or more non-legal quality requirements remain open. Incubating repositories must not be presented as verified releases.

### Verified

All mandatory checklist items pass for a recorded commit. The release notes state the upstream commit/tag, test environment and any deviations.

### Archived

The release is frozen. The README explains why, points to any successor and identifies the last verified version.

## 7. Versioning

- Preserve upstream semantic versions and tags.
- A DeSBi-curated snapshot uses `desbi-YYYY.MM.N`, for example `desbi-2026.08.1`.
- The GitHub release title should be `DeSBi curated release YYYY.MM.N — upstream <tag-or-short-commit>`.
- Release notes must include:
  - upstream repository and immutable commit;
  - DeSBi project(s) and publication(s);
  - verification date and platform;
  - installation/test command;
  - known limitations;
  - DeSBi-only patches, if any.
- Do not create a DeSBi tag when an unchanged upstream tag plus existing DOI already provides the required archival object; in that case, catalogue and verify the upstream release.

## 8. Archiving and citation

Use Zenodo or another recognized repository for persistent archival when appropriate.

- Preserve an existing canonical DOI.
- Create a new DOI only for a genuine DeSBi release object, not merely to duplicate an identical upstream archive.
- Relate the records using `isVersionOf`, `isSupplementTo` or an equivalent relation where supported.
- Cite both the scientific paper and the software release when both are necessary to understand and reproduce the result.

## 9. Synchronization

When upstream remains canonical:

- sync the default branch at least quarterly and before each DeSBi release;
- never force-push over DeSBi release tags;
- submit generally useful fixes upstream first;
- document any DeSBi-only patch as a small, reviewable commit;
- run the verification workflow after an upstream synchronization.

A fork that diverges substantially must declare that the DeSBi organization has become a maintained downstream distribution.

## 10. Review and approval

A verified release requires:

- approval by a scientific maintainer;
- approval by a DeSBi release reviewer from another project or the coordination team;
- completion of `REPO_CHECKLIST.md`;
- a successful installation/reproduction check on a clean environment.

## 11. Deprecation

Deprecate or archive a repository when:

- a maintained successor exists;
- the method is no longer reproducible and cannot reasonably be repaired;
- licensing or data-rights problems emerge;
- maintainers withdraw support.

The repository must remain visible where legally possible, with a prominent successor or archival notice. Superseded repositories such as DualView should be catalogued, not promoted as new releases.
