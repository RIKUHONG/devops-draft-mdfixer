# E2 Backlog

| ID | Task | Owner | Deliverable | Acceptance | Status |
| --- | --- | --- | --- | --- | --- |
| E2-01 | Unified task model | A/B | `contracts/common/task.schema.json` | Represents DRAFT, FULL_CHECK, INCREMENTAL_CHECK, and REPAIR | Done |
| E2-02 | DRAFT contract | B | DRAFT schema, docs, and samples | Repository, build commands, limits, iteration logs, and verification result | Done |
| E2-03 | Full check contract | A/B | FULL_CHECK samples | Commit, configuration, environment, graphs, findings, and report references | Done |
| E2-04 | Historical graph input | A | INCREMENTAL_CHECK samples | Missing baseline rejected; baseline commit and configuration are checkable | Done |
| E2-05 | MDFixer contract | B | REPAIR schema, docs, and samples | MISSING-only input; patch, build, test, and recheck results | Done |
| E2-06 | Artifact contract | A/B | Artifact schema and docs | URI, producer job, repository commit, configuration, and optional SHA-256 | Done |
| E2-07 | Async API decision | A/B | `ADR.md`, interface docs | POST returns 202/QUEUED; GET queries terminal state | Done |
| E2-08 | Schema validation | B | `scripts/validate.py` | Valid samples pass; invalid job type and missing baseline are rejected | Done |
| E2-09 | A/B compatibility migration | B | `MIGRATION.md`, synchronized contracts | B-group repository uses A-group field names and schemas | Done |
| E2-10 | Complete identity metadata | B | README and contribution record | Group, member, commit, and Issue/PR details are filled | Pending |

## Next steps

1. Confirm field naming, `configuration_id`, and artifact URI mapping with A group.
2. Exchange one real artifact from each side and record SHA-256 verification.
3. Fill real identity, group numbers, commit SHA, and Issue/PR in the contribution record.
4. Prepare a runnable DRAFT project and fixed MD report before E3.
