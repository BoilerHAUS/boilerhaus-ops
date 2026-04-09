# CI/CD Process

## Purpose
CI/CD process for boilerhaus-ops docs and code.

## Workflow
1. All changes proposed via pull request
2. No direct pushes to main
3. At least one review required before merge

## Pipelines
- Docs: lint markdown, verify links
- Issues: validate templates and labels

## Release Gating
- All tests must pass before merge
- No manual overrides for failing builds

## Rollback
To revert a merge:
1. Open a PR to revert the commit
2. Get review approval
3. Merge to main
