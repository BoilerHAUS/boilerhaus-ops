# Boilerhaus Ops

This repository is the internal operating system for Boilerhaus.

It is the source of truth for the company setup, operating checklists, launch planning, and recurring review process that sit beside product development.

Planning started in `ScopeHouse-Ops`. This repo now replaces it as the main internal home for Boilerhaus operations.

## Purpose

Use this repo to keep the business legible and runnable:

- legal and incorporation guidance
- finance and bookkeeping decisions
- launch checklists
- operating metrics and review cadence
- issue backlog for company launch work

## Current focus

- incorporate Boilerhaus federally
- register ScopeHouse correctly for Ontario use if it will be public-facing
- stand up banking, bookkeeping, invoicing, and CRA access
- tighten the operating stack for docs, files, email, and security
- turn launch work into a clear GitHub issue backlog

## Working rules

1. Keep docs short, specific, and current.
2. Prefer decisions and checklists over open notes.
3. Use docs to define work before opening issues.
4. Update docs and issue definitions together when the source of truth changes.
5. Treat this repo as the control plane for Boilerhaus operations.

## Repo structure

```text
README.md
.github/
  ISSUE_TEMPLATE/
    work-item.md
docs/
  README.md
  github/
    workflow.md
    milestones.md
    issue-map.md
  operations/
    business-stack.md
    company-launch-checklist.md
    federal-incorporation-guide.md
    weekly-business-metrics-review.md
```

## Start here

- [Docs Index](./docs/README.md)
- [Business Stack](./docs/operations/business-stack.md)
- [Company Launch Checklist](./docs/operations/company-launch-checklist.md)
- [Federal Incorporation Guide](./docs/operations/federal-incorporation-guide.md)
- [Issue Map](./docs/github/issue-map.md)
