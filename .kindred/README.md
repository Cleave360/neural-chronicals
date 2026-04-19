# .kindred local ledger layout

This repository uses `.kindred/` for local orchestration and execution artifacts that should NOT be committed.

## Structure

### .kindred/ (local runtime, git-ignored)
- `audit/` - local audit trail files
- `executions/` - execution run state and runtime metadata
- `export/` - generated exports and bundles
- `locks/` - local lock files for coordination
- `tmp/` - temporary scratch files
- `README.md` - this documentation

### runs/ (tracked at repo root)
Decision artifacts and gate deliverables are tracked at the root in `runs/issue-02/`, `runs/issue-03/`, etc. This provides the audit trail for publication gates and agent coordination.

Structure:
- `runs/issue-02/00-brief/` - issue brief and constraints
- `runs/issue-02/10-editorial/` - editorial drafts
- `runs/issue-02/20-distribution/` - distribution strategy
- `runs/issue-02/30-alignment/` - alignment handoffs between teams
- `runs/issue-02/40-build/` - web build artifacts
- `runs/issue-02/50-qa/` - QA signoff

## Optional published fixtures
If you need reproducible examples for docs/tests, create sanitized fixtures in a separate tracked path (for example `docs/fixtures/runs/`) and do not include sensitive runtime data.
