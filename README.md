# Jazz CRM Project — Sales OS Build Log

## Workspace
**CRM Workspace ID:** 6082827

---

## Boards

| Board | ID | Status |
|---|---|---|
| VA New Lead Intake | 18405162437 | Live |
| Sales Pipeline | 18405119757 | Live |
| Active Deals | 18405119784 | Live |
| Calls & Meetings | (linked) | Live |
| Follow-Ups | (linked) | Live |
| Proposals Board | 18405368752 | Live — Phase 2 |
| Agreements Board | 18405368877 | Live — Phase 4 |

---

## Phase 1 — Complete

- Lead Intake Form (VA New Lead Intake board) — all fields live
  - Company Website, Crowdfunding Campaign (Y/N), Crowdfunding Portal, Raise Page Link, Founder/POC LinkedIn, Company Social Media Links
- Sales Pipeline board with full group structure
- Calls & Meetings board (linked to Pipeline)
- Follow-Ups board (linked to Pipeline)

---

## Data Migration — Complete

**Source:** 2025 Deals board (ID: 8929621580)
**Owner filter:** Jazz Parker (user ID: 59898497)
**Destination:** CRM Workspace boards

### Group Mapping Applied

| Source Group | Destination Group | Board |
|---|---|---|
| Emailed items | Contacted | Sales Pipeline |
| Booked Call | Call Booked | Sales Pipeline |
| Missed Call | Call Booked | Sales Pipeline |
| Proposal Sent | Proposal Sent | Sales Pipeline |
| Warm | Replied/Engaged | Sales Pipeline |
| Proposal Review (2nd Call) | — (empty) | — |
| Agreements Sent | Negotiation/Decision | Sales Pipeline |
| Agreement Review Call (3rd Call) | — (empty) | — |
| Slow | Replied/Engaged | Sales Pipeline |
| Silent | Contacted | Sales Pipeline |
| Lost | Closed Lost | Sales Pipeline |
| Closed / Won 2025 | Active Deals Won | Active Deals |
| Partnership Deals | Negotiation/Decision | Sales Pipeline |
| Extras/Doubles | Skipped | — |

**Estimated items migrated: ~500+ Jazz-owned deals**

---

## Process Insights Doc

Created in CRM Workspace: **"Sales Process Insights & Notes"**
Doc ID: 39485403 | [Open Doc](https://digitalnicheagency-company.monday.com/docs/18405368686)

Key insights captured:
1. One call straight to agreement = red flag
2. Invoice trigger protocol + billing caveats
3. Testing phase required before any new automation goes live

---

## Roadmap

### Phase 2 — Complete
- [x] **Proposals Board** (ID: 18405368752)
  - Groups: Requested → In Progress (VA Building) → Rep Review → Approved — Ready to Send → Sent to Client → Accepted → Declined
  - Columns: Rep (Owner), Assigned VA, Due Date, Proposal Value, Linked Pipeline Deal, Proposal Link, Date Sent, Notes

### Phase 3 — Post-Proposal
- [ ] Review Call path (→ Calls & Meetings)
- [ ] Direct Agreement path (→ Agreements)

### Phase 4 — Agreement & Contract Flow — Complete
- [x] **Agreements Board** (ID: 18405368877)
  - Groups: Agreement Requested → Drafting / In Review → Sent for Signature → Signed — Active → Voided / Declined
  - Client fields: Company Name, Client First Name, Client Last Name, Client Email, CC Holder Name, CC Holder Email, Term (Months), Agreement Date
  - Services (checkbox + price each): Strategy Plan, Creative Development, Retainer, Media Spend & Media Management, Outreach, Podcast Outreach Service, Content Marketing, Other Services
  - **Total Price** (formula — auto-sums all 8 service prices)
  - Internal tracking: Sales Rep, Lead Source, PandaDoc Link, Date Sent for Signature, Date Signed, Invoice Status, Linked Pipeline Deal, Linked Proposal, Notes
- [x] **Agreement Request Sheet** form view (View ID: 245725151, Token: 5a0af06b7df2df43dd906bc6bb2f0ed5)
  - All 19 fields configured, ordered, and required/optional set correctly
  - Each service checkbox followed immediately by its price field
  - Items land in "Agreement Requested" group on submit
  - Internal columns hidden from form
- [x] **PandaDoc Integration Guide** — doc created (ID: 39486235)
  - Full field mapping table (all fields → PandaDoc template variables)
  - Step-by-step setup: install app, build template, configure automation
  - Two automations documented: create+send on submit, sync status on sign

### Phase 5 — Payment & Close
- [ ] PandaDoc signed → QuickBooks auto-invoice
- [ ] Payment sync back to monday.com
- [ ] Zapier/Make automation layer

---

## Key IDs Reference

| Resource | ID |
|---|---|
| CRM Workspace | 6082827 |
| Jazz Parker (User) | 59898497 |
| Sales Pipeline Board | 18405119757 |
| Active Deals Board | 18405119784 |
| VA New Lead Intake Board | 18405162437 |
| 2025 Deals Board (source) | 8929621580 |
| Proposals Board | 18405368752 |
| Agreements Board | 18405368877 |
| Agreement Request Sheet (Form View) | 245725151 |
| Contacted Group | group_mm1qtgy3 |
| Replied/Engaged Group | group_mm1qk7aq |
| Call Booked Group | group_mm1q551y |
| Proposal Sent Group | group_mm1qpfy1 |
| Negotiation/Decision Group | group_mm1qcx2k |
| Closed Lost Group | group_mm1qdm24 |
| Active Deals Won Group | group_mm1qna03 |
