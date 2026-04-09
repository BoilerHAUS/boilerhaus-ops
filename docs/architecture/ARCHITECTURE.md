# Architecture

## System Overview
boilerhaus-ops is the control plane for the legal company Boilerhaus. It contains
legal, finance, operating cadence, launch planning, and issue tracking.

## Key Components

### GitHub (boilerhaus-ops)
- Source of truth for incorporation docs, policies, and launch planning
- Issue tracking for company setup milestones
- PR-based workflow for all changes

### Nextcloud
- Internal file sharing and collaboration
- Complementary to GitHub (not a replacement)

### Domain Infrastructure
- ScopeHouse product domain
- Boilerhaus corporate domain

## Tech Choices
- GitHub for structured document management and issue tracking
- Markdown-first documentation (no proprietary formats)
- Agent-accessible (Boiler Jerry reads and writes from this repo)

## Constraints
- No secrets or sensitive financial data in this repo
- All changes go through PR review
