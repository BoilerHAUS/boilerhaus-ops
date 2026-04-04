# Boilerhaus Business Stack Decision Tracker

## Purpose

This document is the working decision tracker for the minimum business stack needed to launch Boilerhaus cleanly.

Boilerhaus is the legal company.
`ScopeHouse` is the first product and likely the first public-facing operating name.

## Core rule

Do not decide the whole stack at once.

Only lock the decisions that unblock:

- legal setup
- taking money
- keeping records clean
- running the first weekly operating cadence

## Current working assumptions

- legal structure direction: federal corporation
- preferred legal name: `Boilerhaus Inc.` if available
- product or operating name: `ScopeHouse`
- current invoicing direction: Wave
- current payment collection direction: Wave
- current domain email provider: IONOS
- docs source of truth: this repo
- file storage direction: Nextcloud for files, contracts, receipts, and working assets
- product analytics direction: defer full setup until the first live users, shortlist PostHog later

## Decision tracker

| Category | Current direction | Status | Next decision to close |
| --- | --- | --- | --- |
| Legal entity and naming | Incorporate Boilerhaus federally and use `ScopeHouse` as the first operating name if needed. | In progress | Confirm final name, fallback path, and Ontario filings needed for `ScopeHouse`. |
| Banking | Open a business account immediately after incorporation. | Not started | Shortlist banks and decide signing authority. |
| Bookkeeping | Keep the shortlist lean: Wave, Manager, or one accountant-led alternative. | Not started | Pick one system and create the first chart of accounts. |
| Invoicing and payments | Use Wave for the launch path unless a concrete blocker appears. | Direction chosen | Create proposal, invoice, and payment collection templates. |
| Email and calendar | Keep IONOS for domain email now; revisit a broader suite later if shared calendar becomes necessary. | Partially decided | Document inbox ownership, aliases, forwarding, and recovery paths. |
| Docs and files | Repo for source-of-truth docs, Nextcloud for files and operational records. | Direction chosen | Build the folder structure and define what must never live only in chat or email. |
| Security and access | Use a password manager and 2FA for all critical systems. | Not started | Choose the password manager and inventory all critical accounts. |
| Product analytics | Wait until the first live workflows are repeatable. | Deferred | Define activation and the first event list before instrumenting. |

## Research scorecard

Use this before locking any tool choice that still feels uncertain.

- setup effort
- monthly cost
- maintenance burden
- Canadian fit
- migration pain later
- small-team fit
- trust in running it personally

## Immediate launch decisions

Close these in order:

1. legal name, share structure, directors, and registered office plan
2. federal incorporation
3. Ontario operating-name and registry requirements for `ScopeHouse`
4. CRA access, GST HST decision, and payroll decision
5. business banking and reimbursement workflow
6. bookkeeping system and chart of accounts
7. invoice, proposal, and payment collection templates
8. email ownership, security baseline, and document system

## What to avoid

- deciding every future tool before launch
- using self-hosting as the default answer
- letting legal and finance setup drift because product work feels more urgent
- keeping important operating decisions only in chat threads
