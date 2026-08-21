# Contributing to the DeSBi software catalogue

## Nominate an output

Open a **Release candidate** issue and provide:

- output name and upstream repository;
- DeSBi project(s), publication and funding evidence;
- licence and copyright holder;
- scientific maintainer and institutional owner;
- whether upstream will remain the canonical development home;
- installation and minimal reproduction instructions;
- data, model-weight or cohort restrictions;
- desired status: catalogue only, release candidate or verified release.

A repository may be catalogued before it is ready to fork. This is preferable to hiding a licensing or packaging blocker.

## Update an existing entry

Submit a pull request changing `catalogue.yml` and, where needed, `REPOSITORY_INVENTORY.md`. Include evidence for changes to:

- licence;
- canonical repository;
- maintainer;
- publication/DOI;
- release status;
- successor or deprecation state.

## Prepare a release

1. Obtain maintainer and owner approval.
2. Resolve legal/licensing blockers upstream.
3. Fork or import while preserving history.
4. Add the provenance block and citation metadata.
5. Complete `REPO_CHECKLIST.md`.
6. Ask a reviewer from another DeSBi project or coordination to reproduce the minimal example.
7. Tag, publish, archive and update the catalogue.

## Contributions belong upstream where possible

Bug fixes, documentation improvements and general features should normally be proposed to the canonical upstream repository. The DeSBi fork should remain a thin, provenance-preserving release layer unless DeSBi explicitly assumes downstream maintenance.

## Sensitive data

Never open an issue or pull request containing patient data, participant identifiers, cohort credentials, non-public access URLs or restricted model artefacts. Describe access procedures and restrictions without exposing protected material.
