# Boilerhaus Launch Issue Map

Use these as the first issue batch for `BoilerHAUS/boilerhaus-ops`.

## Priority guide

- `P0`: blocks legal setup, money movement, or a real launch
- `P1`: strongly needed for launch discipline
- `P2`: useful after the core launch path is running

## Issue list

| # | Priority | Milestone | Title | Why it matters | Done when |
| --- | --- | --- | --- | --- | --- |
| 1 | P0 | Company formation | Confirm Boilerhaus legal name, fallback name, and share structure | Filing should not start until the name path, ownership, directors, and registered office plan are explicit. | Legal name decision is documented, fallback is chosen, and the initial share structure is written down. |
| 2 | P0 | Company formation | File federal incorporation for Boilerhaus | The company cannot bank, contract, or invoice as a corporation until the filing is complete. | Certificate and articles are saved and the corporation is active. |
| 3 | P0 | Company formation | Complete post-incorporation setup: bylaws, officers, shares, and ISC register | Incorporation alone is incomplete without the internal corporate records and control register. | Bylaws are adopted, shares are issued, officers are appointed, and ISC information is created and filed. |
| 4 | P0 | Company formation | Complete Ontario operating-name and registry filings for ScopeHouse | Federal incorporation does not remove the need to handle Ontario-facing operating-name requirements. | Ontario filings needed for Boilerhaus and `ScopeHouse` are confirmed and completed or explicitly ruled out in writing. |
| 5 | P0 | Finance and compliance | Add CRA access and document GST HST and payroll decisions | The company needs CRA access before it can manage taxes cleanly. | Business number access is live, GST HST decision is documented, and payroll readiness is recorded. |
| 6 | P0 | Finance and compliance | Open business bank account and define founder reimbursement flow | Personal and company money should separate immediately after incorporation. | Bank account is open, signing authority is clear, and reimbursement rules are documented. |
| 7 | P0 | Finance and compliance | Choose bookkeeping system and create the first chart of accounts | Clean books matter from day one and become painful if delayed. | One bookkeeping system is chosen and a launch-ready chart of accounts exists. |
| 8 | P0 | Finance and compliance | Finalize invoicing, payment collection, and proposal workflow | Launch requires a way to send proposals, request payment, and track receivables. | First proposal template, invoice template, and payment collection path are ready for use. |
| 9 | P1 | Operating system | Set up company email, aliases, and admin ownership | Business communications and account recovery should not depend on ad hoc forwarding alone. | Primary inboxes, forwarding rules, and admin ownership are documented and tested. |
| 10 | P1 | Operating system | Build security baseline for domains, GitHub, finance, and email | Admin access is one of the first real business risks. | Password manager is chosen, 2FA is enabled, and critical accounts are inventoried with owners. |
| 11 | P1 | Operating system | Define the document system across GitHub and Nextcloud | Docs, contracts, receipts, and customer files need a clear home. | The split between repo docs and file storage is documented and the folder structure exists. |
| 12 | P1 | Go-to-market foundation | Finalize the founder-led service offer and pricing hypotheses | Early revenue likely comes from service or pilot work before a scaled SaaS motion. | Offer scope, pricing range, delivery steps, and buyer fit are documented. |
| 13 | P1 | Go-to-market foundation | Build the live pipeline tracker and first target account list | Launch work needs a visible funnel, not scattered contacts. | Tracker fields are live and the first batch of target accounts is loaded with next actions. |
| 14 | P1 | Go-to-market foundation | Finalize discovery, demo, and follow-up scripts | Sales conversations drift without a repeatable structure. | Scripts exist, are short enough to use live, and connect to qualification and next steps. |
| 15 | P1 | Go-to-market foundation | Publish website, contact, and legal basics | The company needs a credible public surface before active outreach scales. | Contact path is public and the basic site pages needed for trust are identified and launched. |
| 16 | P1 | Launch readiness and cadence | Stand up the weekly business review and launch dashboard | The company needs one fixed review loop for learning, revenue, and blockers. | A weekly review owner, schedule, and dashboard fields are defined and used once. |
| 17 | P1 | Launch readiness and cadence | Run a launch readiness review and close every remaining P0 blocker | A launch decision should happen against a checklist, not gut feel. | The launch checklist is reviewed, blockers are assigned, and the go or not-yet decision is recorded. |

## Suggested opening order

1. Open all `P0` issues first.
2. Open `P1` issues once the legal filing is moving.
3. Leave `P2` items for later unless they start blocking revenue or operations.

## Issue template

Use `.github/ISSUE_TEMPLATE/work-item.md` when turning any row above into a live issue.
