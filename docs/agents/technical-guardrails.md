# Boilerhaus Technical Guardrails — v0.1

**Last Updated:** April 08, 2026  
**Owner:** Boiler Jerry  
**Canonical Source:** [boilerhaus-ops/docs/agents/technical-guardrails.md](https://github.com/BoilerHAUS/boilerhaus-ops/blob/main/docs/agents/technical-guardrails.md)

> These are the non-negotiable rules for all work across Boilerhaus repositories. Human or agent — the same standard applies.

---

## 1. Branching and Workflow

### 1.1 Main Branch
- **Main is always production-ready.** No direct pushes, no exceptions.
- All changes land via pull request with at least one review.
- Protected branch configuration should enforce this at the repo level.

### 1.2 Branch Naming
- **Format:** `type/short-description`
- **Types:**
  - `feat/` — new features, capabilities, or additions
  - `fix/` — bug fixes or corrections
  - `docs/` — documentation-only changes
  - `refactor/` — restructuring without behavior change
  - `ops/` — infrastructure, CI/CD, or tooling changes
- **Examples:** `feat/user-auth`, `fix/login-redirect`, `docs/api-reference`

### 1.3 Pull Requests
- Every PR must reference a work item (issue).
- Descriptions must include: what changed, why, and how to verify.
- Keep PRs focused — one concern per pull request.
- Squash merge to main for clean history.

### 1.4 Commit Messages
- Imperative mood: "Add validation," not "Added validation."
- Short headline (72 chars), optional body after blank line.
- Reference issues when applicable: `fix rate limiter timeout (#14)`

---

## 2. Code Quality and Review

### 2.1 Before Merge
- [ ] Code passes existing linting and type checks
- [ ] Tests added or updated for behavioral changes
- [ ] No console.log, debugger, or TODO markers in merged code
- [ ] Secrets removed — no API keys, tokens, or credentials in code or comments

### 2.2 Review Requirements
- All PRs require at least one approving review
- Review comments must be addressed or explicitly acknowledged
- Stale or abandoned PRs are closed after 14 days of inactivity

### 2.3 Testing Philosophy
- Tests should be fast, deterministic, and focused
- Integration tests for critical paths, unit tests for complex logic
- No test that depends on external network calls in CI

---

## 3. Security

### 3.1 Secret Management
- **Never commit secrets.** Not in code, config, comments, or base64.
- Use environment variables or a secret manager for credentials.
- Rotate immediately if accidentally committed — even if force-pushed away.

### 3.2 Secret Scanning
- GitHub secret scanning must remain enabled on all repositories.
- Push protections (push protect) should block credential commits at the hook level.

### 3.3 Dependencies
- Monitor for known vulnerabilities (Dependabot or equivalent).
- Pin dependency versions — no floating `*` or `latest` in production.
- Review major version bumps before accepting automated PRs.

### 3.4 Access Control
- Principle of least permission — tokens are scoped, not blanket admin.
- Personal Access Tokens (PATs) scoped to minimal repo access.
- GitHub App credentials preferred for automated bot identity.

---

## 4. Agent Execution Rules

### 4.1 Default Posture
- **Read-first.** Always inspect the repo before modifying any file.
- **Fail loudly.** If a guardrail is violated, stop and report — do not silently continue.

### 4.2 Scope of Action
- **Safe (no ask):** Read, explore, organize, search, analyze
- **Ask first:** Any action that leaves the machine — emails, posts, public comments, or data exfiltration
- **Destructive operations:** Always confirm before `rm`, `DROP`, or force-push

### 4.3 Documentation Discipline
- Decision over notes. If it's not a decision, a checklist, or an deliverable — it doesn't belong in a doc.
- One topic per file. No open threads.
- Update indices when adding files to the docs directory.
- Keep docs short and actionable.

### 4.4 Repo-Specific Rules
- Check for local agent guardrails in `.hermes/` or `.agents/` before acting.
- If local rules exist, they take priority over these global guardrails.
- If no local rules found, fall back to this document.

### 4.5 Identity
- Agent commits use: `user.name: "Boiler Jerry"`, `user.email: "agent@boilerhaus.dev"`
- Bot identity (GitHub App) should be used for automated PRs and issue management.
- Human identity for all manual review and merge decisions.

---

## 5. Infrastructure and CI/CD

### 5.1 Pipeline Rules
- CI must pass before merge — no manual overrides for failing builds.
- Build artifacts are immutable — same commit always produces same output.
- Deployment is automated from the pipeline — no manual SSH + deploy workflows.

### 5.2 Environments
- Development → Staging → Production (if applicable)
- Promotions are explicit — never auto-promote to production.
- Rollback procedure documented for every service.

### 5.3 Monitoring
- Logs are structured and searchable.
- Errors and alerts are actionable — no alert that goes ignored.
- Dashboards exist for each service's health.

---

## 6. File Structure Conventions

### 6.1 Documentation
```
docs/
  README.md              ← index of all documents
  agents/
    technical-guardrails.md   ← this file
  github/
    workflow.md
    milestones.md
  operations/
```

### 6.2 Agent Configuration
```
.hermes/
  agent-guardrails.md    ← repo-specific agent rules (optional)
  config.yaml            ← agent configuration
```

### 6.3 GitHub Templates
```
.github/
  ISSUE_TEMPLATE/
    work-item.md
  PULL_REQUEST_TEMPLATE.md
```

---

## 7. Enforcement

- These guardrails are **living documents** — they evolve with the team.
- Proposed changes should be PR'd to this file in `boilerhaus-ops`.
- Version bump on meaningful changes (v0.1 → v0.2, etc.).
- Last updated date must be maintained.

---

*Form follows function. Structure is not bureaucracy — it's the grid that makes the work clean.*
