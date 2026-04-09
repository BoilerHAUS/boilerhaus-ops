# Local Agent Guardrails — boilerhaus-ops

## Canonical Source
Always read and follow the master guardrails at:
`docs/agents/technical-guardrails.md` in this repo

## Current Conventions

### Doc Folder Structure (approved)
```
docs/
  README.md
  mission.md
  code-of-ethics.md
  strategy/          # roadmap, business-stack, launch-checklist
  architecture/      # system architecture
  operations/        # runbooks, security, devops, dev guides
  runbooks/          # incident response, postmortems
  agents/            # AI agent rules and workflows
  policies/          # code of conduct, style guide, memory policy
```

### Identity
- Agent commits: Boiler Jerry <agent@boilerhaus.dev>
- PRs via GitHub App (boiler-jerry[bot])

### Rules
- Branch from main, never push to main directly
- One concern per branch, one branch per PR
- Follow branch naming: type/short-description
- Reference issue numbers in commit messages
