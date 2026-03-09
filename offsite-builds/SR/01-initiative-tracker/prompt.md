# Cross-Functional Initiative Tracker

## Prompt

I'm VP of Strategic Initiatives at Ripple. I coordinate across Business Development, Corporate Development, Corp Strategy & Ops, Marketing, and other functions. At any given time I'm tracking 8-12 major initiatives — M&A integrations, market expansion programs, executive programs, strategic partnerships, and internal transformation projects. Each has a different owner, different cadence, and different stakeholders.

My problem: I get updates from everywhere — email, Slack, docs, meetings — but there's no single view that tells me "here's where everything stands right now." I build this manually in a spreadsheet every week and it takes 2+ hours.

Using my connected sources (Gmail, Slack, Google Drive) — or by uploading status update emails/docs — build me an initiative tracker that:

### 1. Initiative Portfolio View
For each active initiative, show:
- **Initiative name** and one-line description
- **Owner** — who's the primary DRI?
- **Status** — On Track / At Risk / Blocked / Complete
- **Last update** — When was the last status update received and from whom?
- **Key milestone** — What's the next major milestone and when?
- **Dependencies** — What does this initiative depend on from other teams?
- **Escalations** — Anything that needs SVP/C-level attention?

### 2. Cross-Initiative Dependencies
Map the dependencies between initiatives. For example:
- GTreasury integration depends on Custody API (product team)
- LATAM market expansion depends on Santander LOI (legal sign-off)
- Hidden Road benefits transition depends on benefits harmonization decision (People team)

Flag dependency chains where a delay in one initiative cascades to others.

### 3. Weekly Status Synthesis
From the raw updates I receive, generate a weekly status report I can send to EVM and the exec team:
- **Executive summary** — 3-5 bullet TL;DR of the week
- **Green initiatives** — On track, no action needed (one line each)
- **Yellow/Red initiatives** — What's at risk, why, and what's the ask
- **Decisions needed** — Specific decisions with context and who needs to make them
- **Looking ahead** — Key milestones in the next 2 weeks

### 4. Stale Initiative Detection
Flag any initiative where:
- No status update received in 7+ days
- A milestone date has passed without a completion update
- An escalation was raised but no response received

### Output
Generate as an interactive HTML dashboard with:
- Card-based portfolio view (sortable by status, owner, last update)
- Dependency map visualization
- Exportable weekly status report

---

## Sample Initiatives to Track

If you don't have connected sources, use these as seed data:

| Initiative | Owner | Status | Notes |
|-----------|-------|--------|-------|
| Hidden Road Integration | Corp Dev + Product | At Risk | License transfers in HK/UAE slow |
| GTreasury Integration | Product + Finance | On Track | Custody API beta targeting April |
| Rail Integration | Corp Dev + Legal | At Risk | NY/CA/TX license transfers delayed, $300K overrun |
| Palisade Integration | Engineering + Legal | On Track | AGPL dependency issue being resolved |
| LATAM Corridor Expansion (Santander) | BD + Legal | On Track | LOI signed, legal review in progress |
| APAC Banking Partnership | BD + Compliance | On Track | NDA stage, signing expected in 2 weeks |
| RLUSD Growth Program | Product + Marketing | On Track | $500M market cap hit, Mastercard pilot live |
| FCA Post-Conditions Compliance | Legal + Regulatory | On Track | Compliance officer nomination pending CLO sign-off |
| Executive AI Training Program | Strategic Initiatives | On Track | March 10 session confirmed, connectors configured |
| Analyst Day Planning | IR + Marketing | Pending Decision | Proposed May timing, $150K budget needs CFO approval |

---

## Stretch Goal

Connect to a shared Google Sheet or Notion database where initiative owners update their own status. Claude pulls from that source weekly and generates the synthesis automatically — zero manual aggregation.
