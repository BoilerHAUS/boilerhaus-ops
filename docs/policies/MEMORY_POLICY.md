# Memory Policy

## Purpose
Define memory hygiene and retention principles for boilerhaus-ops.

## Retention Guidelines
- Active docs stay in their canonical folder
- Superseded docs move to `archive/` with a symlink from their last known path
- Never delete a doc without archiving first (Git history preserves, but discoverability doesn't)

## Deletion / Archival Process
1. Mark the doc with `[ARCHIVED YYYY-MM-DD]` in frontmatter
2. Move to `archive/` directory
3. Remove internal links to the doc from other files
4. Close any related GitHub issues

## Review Cadence
Review all docs quarterly. Archive anything obsolete.
