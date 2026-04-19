# .kindred local ledger layout

This repository uses `.kindred/` for local orchestration and execution artifacts.

## Committed
- `README.md` (this file)

## Not committed (ignored)
- `audit/` - local audit trail files
- `executions/` - execution run state and runtime metadata
- `export/` - generated exports and bundles
- `locks/` - local lock files for coordination
- `tmp/` - temporary scratch files

## Optional published fixtures
If you need reproducible examples for docs/tests, create sanitized fixtures in a separate tracked path (for example `docs/fixtures/kindred/`) and do not include sensitive runtime data.
