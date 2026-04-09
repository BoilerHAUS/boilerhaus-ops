# Security Policy

## Purpose
Security posture and vulnerability handling for boilerhaus-ops.

## Vulnerability Process
- Report vulnerabilities privately to the project owner
- Do not open a public issue for security findings
- Response expected within 48 hours

## Access Controls
- GitHub access follows the principle of least privilege
- Bot identity (boiler-jerry[bot]) used for automated PRs
- Personal accounts used for human review and merge decisions

## Secrets Handling
- No secrets, tokens, or credentials in this repository
- Use environment variables and secret managers for access
- Rotate immediately if accidentally committed

## Patch Cadence
- Review dependency security advisories weekly
- Apply critical patches within 24 hours

## Incident Response Integration
See `RUNBOOKS/INCIDENT_RESPONSE.md` for incident procedures.
