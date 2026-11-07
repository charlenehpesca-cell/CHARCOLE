# MEMORY.md — Pau Parreno

Facts about this client that change over time. Rules go in this folder's CLAUDE.md.

## Active projects

- GHL CRM audit — report delivered 2026-10-30, in review — https://claude.ai/artifact/Xx8Chs2ox1D9At8ejsPjaE

## Decisions

- YYYY-MM-DD: [decision and who made it]

## Contacts

- [Name] — [role] — [how they prefer to be contacted]

## Notes

- GHL sub-account: "Joy Pauline C. Parreño" (Quezon City). Sun Life advisor (PH). Custom objects Policies + Claims from GHL insurance template; one pipeline "Potential Clients".
- 2026-10-30 audit: servicing workflows found only as contact-based drafts (Charlene says the live ones are on the Policies object); contact-level policy fields duplicate the Policies object; a third of policies not linked to contacts; no phone/SMS set up. Details in the report link above (kept out of this repo because it is publicly readable).
- Em and Ralph do the monthly Sun Life policy data refresh and policy imports.
- Consultation booking flow: client requests a time → request email to client + booking-request alert to Pau and team → Pau checks availability → team sets the appointment to Confirmed → client gets the confirmation email with meeting details.
- Policies link to contacts automatically when Policyholder Email matches the contact email.
- New policy flow: add policy with status Approved (email matching the contact), then change status to Premium paying, which auto-enrols the client in 90-Day Journey, 52-Week Nurture, Milestones, Holidays and Annual Review. Those servicing workflows live on the Policies object; Charlene is deleting the old contact-based drafts (2026-11-02).
- 2026-11-03 workflow review (18 live workflows): Premium paying starts Welcome, 90-Day, 52-Week and Holidays 2027. Plan Milestones (30 days after Issue Date) and Annual Review (yearly, 335 days after Issue Date) run from Issue Date, not status. Policy Record Created links the contact by email only at creation. Lapsed and Surrendered remove the policy from the other servicing workflows. Application In-Progress sets Application Submission Date automatically. Nothing runs on Reactivated. "old Marketing Workflows" folder is to be ignored.
- Open issues flagged to Charlene 2026-11-03: Welcome email and 52-Week triggers use "status is Premium paying" with re-entry on (welcome may resend when a Premium-paying policy is edited); no restart for Reactivated policies; Annual Review has no status filter (reaches lapsed policies).
- 2026-11-07 automation health check (read-only): no action errors since Nov 3 tests. Found enrollments stuck "Paused due to draft mode" since Nov 2 (workflows were toggled to draft around then; republishing did not resume them): 52-Week Nurture (bulk-enrolled Oct 26 existing clients, ~629), Annual Review (3), 90-Day (1, Sun Safer Life). Holidays, Lapsed, Surrendered, Milestones not affected. Welcome email duplicate confirmed (Sun Safer Life got it Oct 22 and Oct 23). New Reply Received alert skipped every time ("no user assigned for the contact"). New draft "(Policy) Premium Payment Reminder" (7 days before payment due) has 5 real policies paused in it. "test only" policy still enrolled in 52-Week/90-Day. Annual Review trigger still has no status filter; no Reactivated workflow.
- 2026-11-07 fixes (Charlene approved): New Reply Received alert now goes to Pau, Em Navarro and Ralph Dumayas (was contact owner, always skipped). Reactivated status now enrols the policy in Welcome, 90-Day, 52-Week and Holidays (trigger "Policy Status has changed to Reactivated"); Welcome workflow's first step removes the policy from Lapsed and Surrendered. Annual Review now starts with an "Active policy?" check (Premium paying / Paid-Up / Reactivated; anything else ends). Welcome/90-Day/52-Week/Holidays triggers already use "has changed to Premium paying" (fixed since Nov 3), re-entry on. "test only" policy deleted (restorable 2 months).
- Still open 2026-11-07: enrollments paused by draft mode do not resume — neither "force to next step" nor Draft→Publish released them (90-Day: Sun Safer Life; Annual Review: 3; 52-Week: ~629 bulk-enrolled Oct 26). Charlene resolved it herself on 2026-11-07; enrollments now moving.

