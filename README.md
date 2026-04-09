# Boilerhaus Ops

This repository is the internal operating system for Boilerhaus.

Private internal repository. Confidential and proprietary. No unauthorized use, copying, or distribution.

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
CLAUDE.md                              ← agent context & design system
CONTRIBUTING.md                        ← contribution guidelines
LICENSE                                ← project license
README.md                              ← this file

.github/
  ISSUE_TEMPLATE/
    bug_report.md                      ← bug report template
    work-item.md                       ← standard work-item template
  PULL_REQUEST_TEMPLATE.md             ← PR description template

docs/
  README.md                            ← docs index
  agents/
    technical-guardrails.md            ← AI agent workflow rules
  architecture/
    ARCHITECTURE.md                    ← system architecture overview
  github/
    workflow.md                        ← GitHub conventions
  incorporation/
    phase2/
      articles_of_incorporation.md     ← articles of incorporation
      directors_officers.md            ← directors & officers registry
      isc_disclosures.md               ← ISC disclosure documents
      phase2_checklist.md              ← phase 2 filing checklist
    phase3/
      filing_package.md                ← phase 3 filing package
  operations/
    DEVOPS-CI-CD.md                    ← CI/CD process guide
    SECURITY.md                        ← security policy
    weekly-business-metrics-review.md  ← weekly review template
  policies/
    CODE_OF_CONDUCT.md                 ← code of conduct
    code-of-ethics.md                  ← code of ethics
    MEMORY_POLICY.md                   ← agent memory handling rules
    STYLE_GUIDE.md                     ← documentation style guide
  runbooks/
    INCIDENT_RESPONSE.md               ← incident response playbook
    POSTMORTEM_TEMPLATE.md             ← postmortem template
  strategy/
    business-stack.md                  ← tool shortlists & decision framework
    company-launch-checklist.md        ← launch readiness checklist
    federal-incorporation-guide.md     ← federal incorporation guide
    issue-map.md                       ← full launch issue list with priority
    milestones.md                      ← five milestone definitions
    mission.md                         ← company mission statement
    ROADMAP.md                         ← product roadmap
```

## Start here

- [Docs Index](./docs/README.md)
- [Mission](./docs/strategy/mission.md)
- [Roadmap](./docs/strategy/ROADMAP.md)
- [Business Stack](./docs/strategy/business-stack.md)
- [Company Launch Checklist](./docs/strategy/company-launch-checklist.md)
- [Milestones](./docs/strategy/milestones.md)
- [Issue Map](./docs/strategy/issue-map.md)
- [Technical Guardrails](./docs/agents/technical-guardrails.md)
