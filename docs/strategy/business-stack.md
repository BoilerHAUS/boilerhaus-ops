# Boilerhaus Business Stack Research and Readiness Guide

## Purpose

This document is the working guide for choosing the business stack Boilerhaus needs to launch cleanly.

It is not a final stack decision document.
It is a founder shortlist, testing, and readiness document.

Boilerhaus is the legal company.
`ScopeHouse` is the first product and likely the first public-facing operating name.

## How to use this document

Work category by category.

1. Keep each shortlist to 2 or 3 viable options.
2. Test the options against the same scenarios.
3. Lock only the decisions that unblock real operations.
4. Delay heavier tooling until the current process breaks.

## Core rule

Do not decide the whole business stack at once.

You only need enough decisions to:

- incorporate correctly
- take money
- keep records clean
- run the first weekly operating cadence

## Decision stages

### Stage 1, needed now

- legal entity and naming path
- Ontario operating-name handling
- business banking
- bookkeeping
- invoicing and payments
- email
- document and file system
- security baseline

### Stage 2, needed soon

- CRM or pipeline workflow
- proposal and signature workflow
- website and public contact basics
- product and launch analytics

### Stage 3, needed later

- broader automation
- deeper integrations
- larger CRM or RevOps tooling
- self-hosted business systems beyond what is already maintained

## Research scorecard

Score each option from 1 to 5:

- setup effort
- monthly cost
- maintenance burden
- Canadian fit
- founder trust in running it
- migration pain later
- small-team fit
- how well it protects focus during launch

Use this template:

### Option name

- category:
- option type:
- setup effort:
- monthly cost:
- maintenance burden:
- Canadian fit:
- founder trust:
- migration pain later:
- small-team fit:
- focus protection:
- notes:
- final decision:

## Category-by-category research checklist

## 1. Legal entity and naming

Goal:
Decide how Boilerhaus exists legally and how `ScopeHouse` sits under it.

Options to test:

- named federal corporation: `Boilerhaus Inc.` or close variant
- numbered federal corporation first, then rename later
- `ScopeHouse` used only as a product name inside Boilerhaus materials
- `ScopeHouse` used publicly and registered in Ontario as a business name if required

Questions to answer:

- is brand clarity more important than filing speed
- do you want the umbrella company structure locked now
- will customers see `ScopeHouse` publicly before the Boilerhaus name is established

Test method:

- write the legal name, fallback name, directors, registered office, and share structure on one page
- decide whether `ScopeHouse` will appear publicly on invoices, website copy, proposals, or contracts
- confirm the Ontario-facing filing path before using `ScopeHouse` publicly

Deliverable:

- legal entity decision
- name path
- operating-name decision for `ScopeHouse`
- founder action list for incorporation

Done when:

- you know exactly what to file
- you know the order of filing
- you know which records must be saved

## 2. Ontario operating-name handling

Goal:
Decide what Ontario registrations or Business Registry steps are needed once Boilerhaus is federally incorporated.

Options to test:

- Boilerhaus only in public materials
- Boilerhaus as legal company plus `ScopeHouse` as registered Ontario business name
- delay public use of `ScopeHouse` until Ontario handling is complete

Questions to answer:

- will customers sign or pay under `ScopeHouse`
- will the website, sales deck, or email signatures identify the business as `ScopeHouse`
- what Ontario account access is needed to manage filings later

Test method:

- list every place the public will see the name
- mark each place as `Boilerhaus`, `ScopeHouse`, or both
- confirm whether the name use triggers Ontario business-name registration

Deliverable:

- written Ontario filing position
- business-name decision for `ScopeHouse`
- admin access plan for Ontario filings

Done when:

- there is no ambiguity about public name usage
- the Ontario filing path is explicit

## 3. Business banking

Goal:
Choose a banking path that cleanly separates company money from personal money.

Options to test:

- major bank small-business account
- local credit union business account
- digital-first banking setup, only if it supports the workflows you need

Questions to answer:

- how important is branch access for deposits, drafts, or identity verification
- do you need strong business credit-card options right away
- do you want banking tied closely to bookkeeping integrations

Test method:

- compare onboarding friction
- compare monthly fees and transaction rules
- confirm how easy it is to export statements and reconcile transactions
- confirm whether the bank supports the payment processors you expect to use

Deliverable:

- bank shortlist
- signing authority decision
- founder reimbursement workflow

Done when:

- the business account is open
- money can move through the company without using personal accounts

## 4. Bookkeeping and accounting

Goal:
Choose the bookkeeping system that keeps records clean without creating unnecessary admin burden.

Options to test:

- Wave
- Manager
- Akaunting

What each option represents:

- Wave: low-friction cloud accounting and invoicing, strongly oriented to small businesses in the US and Canada
- Manager: free desktop option plus cloud and server editions, stronger control and lower lock-in, but a less polished user experience
- Akaunting: open-source online accounting with self-hosted flexibility and a broader app-store style extension path

Questions to answer:

- do you want the simplest founder workflow or more long-term control
- how much self-hosting are you actually willing to maintain
- does the tool support the level of bookkeeping discipline you want
- will an external accountant be comfortable receiving year-end exports

Test method:

Create the same test business in each shortlisted option and do the same six tasks:

1. create the company
2. set a basic chart of accounts
3. enter one founder expense
4. enter one invoice
5. record one payment
6. export or inspect the P&L and balance sheet

Deliverable:

- bookkeeping system decision
- first chart of accounts
- monthly bookkeeping routine

Done when:

- one system is chosen
- a launch-ready chart of accounts exists
- monthly reconciliation has an owner and rhythm

## 5. Invoicing and proposals

Goal:
Choose how Boilerhaus sends estimates, proposals, and invoices.

Options to test:

- Wave invoicing
- Stripe Invoicing
- Invoice Ninja
- bookkeeping-tool-native invoicing if the accounting tool wins clearly

What each option represents:

- Wave: easiest fit if bookkeeping also lives in Wave
- Stripe Invoicing: good if you want invoicing closer to future online payments and subscription infrastructure
- Invoice Ninja: stronger if you want a more flexible invoicing system and possible self-hosting path

Questions to answer:

- do you want invoicing tightly coupled to accounting
- do you need estimates or quotes before invoices
- do you need online payment collection built into the invoice experience
- how important is future migration into product billing

Test method:

In each shortlisted option:

1. create one branded estimate or proposal
2. convert it to an invoice if supported
3. add taxes and payment terms
4. send a test invoice to yourself
5. record or simulate payment

Deliverable:

- invoicing system decision
- proposal workflow decision
- first proposal and invoice templates

Done when:

- you know how proposals will be sent
- you know how invoices will be sent
- you know how receivables will be tracked

## 6. Payments

Goal:
Choose how Boilerhaus gets paid.

Options to test:

- Wave payments tied to Wave invoices
- Stripe payment collection tied to Stripe-hosted invoices or payment links
- manual EFT or bank transfer as a baseline fallback

Questions to answer:

- what payment methods do your first customers actually want
- is fast setup more important than future product-billing alignment
- do you need online card collection immediately or can bank transfer work at first

Test method:

- send a real or mock invoice using each path
- confirm the customer payment experience
- confirm where the money lands
- confirm how the payment is reconciled in bookkeeping

Deliverable:

- payment processor decision
- first payment collection workflow
- refund and exception notes

Done when:

- customers can pay cleanly
- funds land in the right account
- bookkeeping can reconcile the payment without hacks

## 7. Email and calendar

Goal:
Choose the company-standard email setup and decide whether the current IONOS path is enough.

Options to test:

- stay on IONOS Mail Business
- Google Workspace
- Microsoft 365

What each option represents:

- IONOS: cheapest path and already in motion
- Google Workspace: strongest fit if you want simple collaboration and lightweight team admin
- Microsoft 365: strongest fit if Outlook and Microsoft admin controls matter more than Google-style collaboration

Questions to answer:

- do you need shared calendar, shared drive, or team collaboration soon
- are aliases and forwarding enough for now
- how much admin overhead are you willing to take on

Test method:

- list every mailbox and alias you need in the next 90 days
- confirm domain setup, forwarding, and recovery flow
- test calendar sharing and shared-contact needs if considering a suite move

Deliverable:

- email provider decision
- inbox and alias list
- admin ownership and recovery checklist

Done when:

- business email is live
- recovery is documented
- key aliases are planned and tested

## 8. Docs, files, and internal workspace

Goal:
Decide how Boilerhaus will split source-of-truth docs from working files and records.

Options to test:

- GitHub docs plus Nextcloud Files only
- GitHub docs plus Nextcloud Files and Collectives
- GitHub docs plus Nextcloud Files, Deck, and Tables

What each option represents:

- Files only: simplest operational file storage
- Collectives: adds handbook-style internal knowledge pages
- Deck and Tables: adds lightweight boards and structured trackers inside Nextcloud

Questions to answer:

- should docs live primarily in markdown in this repo
- do you need wiki-like team pages inside Nextcloud
- should trackers stay as markdown or move into Tables
- should pipeline boards live in Deck or somewhere else

Test method:

Create a small live setup with:

1. one legal folder
2. one finance folder
3. one customer folder
4. one operations folder
5. one board or table for a real workflow if testing Deck or Tables

Deliverable:

- file-system operating model
- folder structure plan
- app usage plan for Collectives, Deck, and Tables

Done when:

- internal docs are not scattered
- files, receipts, and contracts have a clear home
- the system feels simpler, not heavier

## 9. CRM and pipeline workflow

Goal:
Choose how to manage leads, design partners, and service opportunities.

Options to test:

- markdown or spreadsheet tracker plus manual follow-up
- Nextcloud Tables and Deck
- HubSpot free CRM

What each option represents:

- manual tracker: lowest setup cost, highest discipline requirement
- Nextcloud Tables and Deck: keeps data inside your existing environment
- HubSpot: strongest dedicated CRM option if you need a real pipeline quickly

Questions to answer:

- how many active leads will you realistically have in the next 90 days
- do you need email logging and reminders, or just visible next actions
- do you want the CRM to be part of a bigger future GTM stack

Test method:

Create the same test pipeline with 10 sample leads and do the same five tasks:

1. add a lead
2. move stage
3. log note
4. set next action
5. report overdue follow-ups

Deliverable:

- interim pipeline decision
- trigger points for moving to a larger CRM

Done when:

- no lead goes stale without visibility
- next action is visible for every active lead

## 10. Contracts and signatures

Goal:
Choose how proposals, agreements, and signatures will work.

Options to test:

- PDF plus email acceptance
- SignWell
- Dropbox Sign

What each option represents:

- PDF plus email: fastest baseline for very early founder-led sales
- SignWell: simpler dedicated e-sign path with lower-friction positioning
- Dropbox Sign: stronger if you want signatures tied into a Dropbox-style file workflow

Questions to answer:

- when do you actually need formal e-signature flow
- what customer trust or legal expectations exist in your first deals
- how should signed docs flow back into storage and bookkeeping

Test method:

- send yourself one service agreement through each shortlisted path
- confirm signer experience
- confirm template reuse
- confirm where the signed document and audit trail end up

Deliverable:

- signature workflow decision
- first contract template path

Done when:

- paid work can be documented cleanly
- signed documents land in one place with a visible audit trail

## 11. Product and launch analytics

Goal:
Choose how Boilerhaus will measure activation and early demand without overbuilding the stack.

Options to test:

- manual weekly dashboard only
- PostHog
- website-only analytics plus manual product tracking

What each option represents:

- manual dashboard: best if usage is still too low for tooling to matter
- PostHog: strongest path if you want product analytics, retention, and funnels in one stack
- website-only plus manual tracking: good if the website matters before in-app usage does

Questions to answer:

- what events actually matter right now
- do you have enough usage volume to justify product instrumentation
- is launch learning happening more in calls or in product behavior

Test method:

- write the first event list before installing anything
- define the first success moment
- define one weekly dashboard using those events

Deliverable:

- analytics decision
- first event list
- first dashboard list

Done when:

- you know what activation means
- you know what not to instrument yet
- the weekly review can see real signal

## 12. Security and access

Goal:
Set the baseline for founder security and account control.

Options to test:

- hosted password manager
- self-hosted password manager only if it is already within your maintenance capacity
- encrypted emergency access record plus manual inventory as the minimum fallback

Questions to answer:

- who owns each critical account
- where are recovery codes stored
- what systems must have 2FA immediately
- what data must be backed up automatically

Test method:

- inventory domains, GitHub, email, banking, payments, hosting, and CRA-related access
- turn on 2FA everywhere feasible
- verify that one recovery method exists for every critical system

Deliverable:

- password manager decision
- critical account inventory
- backup and recovery checklist

Done when:

- critical systems are recoverable
- admin access is not dependent on memory or scattered notes

## Immediate launch decision order

If everything feels too broad, close these decisions in order:

1. legal entity and naming
2. Ontario operating-name handling
3. business banking
4. bookkeeping
5. invoicing and payments
6. email and recovery
7. docs and file system
8. security baseline
9. pipeline workflow
10. signature workflow
11. analytics

## What to avoid

- deciding every future tool before launch
- installing self-hosted tools because they feel philosophically correct
- mixing legal decisions, product branding, and ops tooling into one vague thread
- picking tools without running one realistic test workflow through them
- keeping stack decisions only in chat

## Current working shortlist

This is the starting point, not the final answer.

| Category | Current shortlist |
| --- | --- |
| Legal entity | Named federal corporation or numbered federal corporation |
| Ontario name handling | Boilerhaus only or Boilerhaus plus registered `ScopeHouse` business name |
| Banking | Major bank account, credit union account, or digital-first banking path |
| Bookkeeping | Wave, Manager, Akaunting |
| Invoicing | Wave, Stripe Invoicing, Invoice Ninja |
| Payments | Wave, Stripe, EFT fallback |
| Email | IONOS, Google Workspace, Microsoft 365 |
| Docs and files | GitHub plus Nextcloud Files, then optionally Collectives, Deck, Tables |
| CRM | Manual tracker, Nextcloud Tables and Deck, HubSpot |
| Signatures | PDF plus email, SignWell, Dropbox Sign |
| Analytics | Manual dashboard, PostHog, website-only analytics plus manual product tracking |
| Security | Hosted password manager, self-hosted password manager, minimum manual fallback |

## References

Federal and Ontario setup:

- [Federal Incorporation Guide](./federal-incorporation-guide.md)

Current product references used to refresh shortlist options:

- Wave support on current US and Canada focus: `https://support.waveapps.com/hc/en-us/articles/27277914806804-Changes-for-Wave-users-outside-the-United-States-and-Canada`
- Manager editions and portability: `https://www2.manager.io/index`, `https://www2.manager.io/cloud/`, `https://www2.manager.io/server/`
- Akaunting overview: `https://akaunting.com/`
- Stripe Invoicing: `https://docs.stripe.com/invoicing`
- Invoice Ninja: `https://invoiceninja.com/`
- Google Workspace business email: `https://workspace.google.com/intl/en_US/business/`
- Microsoft 365 business email: `https://www.microsoft.com/en-us/microsoft-365/business/business-email-address`
- IONOS business email: `https://www.ionos.com/office-solutions/create-an-email-address`
- Nextcloud Collectives: `https://apps.nextcloud.com/apps/collectives`
- Nextcloud Deck: `https://apps.nextcloud.com/apps/deck/`
- Nextcloud Tables: `https://apps.nextcloud.com/apps/tables`
- PostHog product analytics: `https://archive.posthog.com/`
- HubSpot free CRM: `https://www.hubspot.com/products/free-crm-software`
- SignWell: `https://www.signwell.com/`
- Dropbox Sign: `https://www.dropbox.com/sign`
