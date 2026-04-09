# CLAUDE.md — Boilerhaus Ops

> This is the operating system for Boilerhaus. It is not a product codebase — it is a structured document and issue system for running the company. Treat every file here as a living decision record, not a scratchpad.

---

## Repo Identity

**Boilerhaus** is the legal company. **ScopeHouse** is the first product and the primary public-facing name.

This repo is the control plane: legal, finance, operating cadence, launch planning, and issue tracking all live here in markdown. The source of truth is always in the file, not in chat.

---

## Design Identity: Bauhaus DNA

The name is not accidental. **Boilerhaus** carries the Bauhaus inheritance — the 1919 German design school that insisted form follows function, that beauty and utility are not in tension, and that a grid is not a cage but a foundation.

This design identity governs every surface Boilerhaus and ScopeHouse will present to the world.

### Core Principles

1. **Form follows function.** Every visual decision earns its place. No decoration that does not work.
2. **Geometric precision.** Sharp corners, consistent radii, strict baseline grids. No accidental softness.
3. **Primary restraint.** A narrow, confident palette. One dominant neutral, one strong accent. Nothing diluted.
4. **Typographic hierarchy.** Type is structure. It does not merely label — it organizes and communicates priority.
5. **Negative space as architecture.** White space is not emptiness. It is the grid made visible.

---

## Design System — Reference Spec

> This is the canonical design language for Boilerhaus and ScopeHouse. All product UI, marketing surfaces, and internal tooling follow these tokens.

### Color Tokens

```css
/* Core palette — Bauhaus primaries, industrial neutrals */
--color-void:       #0C0C0C;   /* Near-black — primary text, headers */
--color-paper:      #F7F5F0;   /* Warm white — primary background */
--color-signal:     #D92B2B;   /* Bauhaus red — primary accent, CTAs */
--color-signal-alt: #1A52CC;   /* Bauhaus blue — secondary accent, links */
--color-rule:       #E2DED8;   /* Warm grey — borders, dividers */
--color-smoke:      #6B6660;   /* Mid grey — secondary text, captions */
--color-ash:        #2E2C2A;   /* Dark grey — sidebar, code backgrounds */

/* Semantic aliases */
--color-text-primary:   var(--color-void);
--color-text-secondary: var(--color-smoke);
--color-bg-primary:     var(--color-paper);
--color-bg-inverted:    var(--color-void);
--color-accent:         var(--color-signal);
--color-border:         var(--color-rule);
```

### Typography

**Display / Headings** — `"Barlow Condensed"` (Google Fonts) — uppercase, wide tracking, high visual weight.
**Body** — `"DM Sans"` (Google Fonts) — humanist geometric, clear at small sizes.
**Monospace / Code** — `"JetBrains Mono"` (Google Fonts) — expressive, built for long reading.

```css
/* Type scale — major third (1.25 ratio) */
--type-xs:   0.64rem;   /* 10px — labels, metadata */
--type-sm:   0.80rem;   /* 13px — captions, footnotes */
--type-base: 1.00rem;   /* 16px — body */
--type-md:   1.25rem;   /* 20px — lead text */
--type-lg:   1.56rem;   /* 25px — card headings */
--type-xl:   1.95rem;   /* 31px — section headings */
--type-2xl:  2.44rem;   /* 39px — page headings */
--type-3xl:  3.05rem;   /* 49px — hero display */
--type-4xl:  3.81rem;   /* 61px — brand display */

/* Heading style — always condensed, always tracked */
font-family: "Barlow Condensed", sans-serif;
font-weight: 700;
letter-spacing: 0.04em;
text-transform: uppercase;

/* Body style */
font-family: "DM Sans", sans-serif;
font-weight: 400;
line-height: 1.65;
```

### Spacing System

8px base unit. All spacing is a multiple of 8.

```css
--space-1:  4px;
--space-2:  8px;
--space-3:  12px;
--space-4:  16px;
--space-5:  24px;
--space-6:  32px;
--space-7:  48px;
--space-8:  64px;
--space-9:  96px;
--space-10: 128px;
```

### Grid

- 12-column grid
- 24px gutters (32px on large screens)
- Max content width: 1280px
- Sidebar (if applicable): 280px fixed

### Borders and Radius

```css
--radius-none: 0px;
--radius-sm:   2px;
--radius-md:   4px;    /* Default — cards, inputs */
--radius-lg:   8px;    /* Modals, panels */
--radius-full: 9999px; /* Pills, badges */

--border-width: 1px;
--border-color: var(--color-rule);
```

### Motion

Bauhaus does not fidget. Motion is purposeful, fast, and geometric.

```css
/* Transitions */
--ease-standard: cubic-bezier(0.4, 0, 0.2, 1);   /* General UI */
--ease-enter:    cubic-bezier(0, 0, 0.2, 1);       /* Elements entering */
--ease-exit:     cubic-bezier(0.4, 0, 1, 1);       /* Elements leaving */

/* Durations */
--duration-fast:   100ms;   /* Hover states */
--duration-base:   200ms;   /* Standard transitions */
--duration-slow:   350ms;   /* Entrances, reveals */
--duration-xslow:  500ms;   /* Page transitions, modals */
```

No bounce. No spring. No easing that draws attention to itself.

### Elevation (Shadows)

```css
--shadow-sm:   0 1px 2px rgba(12, 12, 12, 0.08);
--shadow-md:   0 2px 8px rgba(12, 12, 12, 0.10);
--shadow-lg:   0 8px 24px rgba(12, 12, 12, 0.12);
--shadow-xl:   0 16px 48px rgba(12, 12, 12, 0.16);
```

---

## Component Philosophy

When building any UI component for Boilerhaus or ScopeHouse:

1. **Start from the token system.** No raw hex values, no arbitrary pixel values outside the spacing scale.
2. **One component, one concern.** A card does not know about navigation. A button does not know about layout.
3. **Accessible by default.** WCAG AA minimum. Color contrast verified. Focus states always visible.
4. **No motion without purpose.** If you cannot articulate why an animation exists, remove it.
5. **Dark mode second.** Build light mode first against `--color-paper`. Dark mode inverts with the `--color-ash` and `--color-void` tokens.

---

## Working in This Repo

### What this repo is

- Source of truth for legal, financial, operating, and launch decisions
- Issue backlog for company launch work
- Reference for GitHub workflow, milestones, and templates

### What this repo is not

- A product codebase
- A notes dump
- A place for open-ended brainstorming without a decision or deliverable

### Rules for Claude in this repo

1. **Read before writing.** Always check the existing doc before proposing an edit.
2. **Decisions over notes.** If something is not a decision, a checklist, or a deliverable — it does not belong in a doc.
3. **Keep docs short and specific.** One topic per file. No open threads.
4. **Use the issue template.** New work items follow `.github/ISSUE_TEMPLATE/work-item.md`.
5. **Update the index when adding files.** If a new doc is created, update `docs/README.md`.
6. **No hardcoded secrets.** This repo may contain sensitive operational details — nothing that looks like a credential, API key, or personal financial data goes in a file.
7. **Follow the milestone structure.** Issues belong to one of the five milestones in `docs/github/milestones.md`.

### Priority labels

- `P0` — blocks legal setup, banking, or revenue. Do immediately.
- `P1` — strongly needed for launch discipline. Do next.
- `P2` — useful after the core launch path is running.

---

## File Structure

```text
CLAUDE.md                              ← this file
README.md                              ← repo overview and start-here links
CONTRIBUTING.md                        ← contribution guidelines
LICENSE                                ← project license

.github/
  ISSUE_TEMPLATE/
    bug_report.md                      ← bug report template
    work-item.md                       ← standard issue template
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
    business-stack.md                  ← tool shortlists and decision framework
    company-launch-checklist.md        ← launch readiness checklist
    federal-incorporation-guide.md     ← federal incorporation guide
    issue-map.md                       ← full launch issue list with priority
    milestones.md                      ← five milestone definitions
    mission.md                         ← company mission statement
    ROADMAP.md                         ← product roadmap
```

---

## Design System Milestone

The Boilerhaus design system is tracked as an active workstream.

Goal: a reusable, token-based design system that every Boilerhaus and ScopeHouse surface — marketing site, product UI, internal tools — can reference without reinventing visual decisions.

See the design system issue in the GitHub issue backlog to track scope, phases, and acceptance criteria.

---

## References

- [Repo README](./README.md)
- [Docs Index](./docs/README.md)
- [Issue Map](./docs/strategy/issue-map.md)
- [Milestones](./docs/strategy/milestones.md)
- [Business Stack](./docs/strategy/business-stack.md)
- [Company Launch Checklist](./docs/strategy/company-launch-checklist.md)
