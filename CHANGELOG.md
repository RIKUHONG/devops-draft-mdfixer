# Contract Change Log

## 1.1 - 2026-09-20

Synchronized with A group's current contract version:

- Moved canonical schemas into `contracts/common/`, including task, job, artifact, finding, dependency graph, and error schemas.
- Moved the four task samples into `contracts/{draft,buildchecker,echecker,mdfixer}/` and added failure, rejection, and negative samples.
- Changed DRAFT limits to `input.limits`; standardized environment fields to `image_uri`, `configuration_id`, and `workdir`.
- Changed REPAIR to use a complete `error_report` reference and moved build and verify commands into `environment`.
- Changed artifacts to use `repository_commit`; made `configuration_id` required; made `sha256` optional; renamed `IMAGE` to `CONTAINER_IMAGE`.
- Synchronized error codes to `REQ_*`, `BASE_*`, `ENV_*`, `EXEC_*`, `ANALYSIS_*`, and `REPAIR_*`.
- Updated validation result to `17 passed, 0 failed`.

## 1.0 - 2026-09-17

Initial E2 interface contract for DRAFT, FULL_CHECK, INCREMENTAL_CHECK, and REPAIR asynchronous jobs.
