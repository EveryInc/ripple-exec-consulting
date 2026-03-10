# CEO Strategic Briefing

## Prompt

I'm CEO of Ripple. I run a company with five product lines (Payments, Custody, RLUSD, Prime, Treasury), recent acquisitions still integrating, 75 regulatory licenses across 40+ jurisdictions, and a leadership team of 8 direct reports. My inbox is a firehose. My calendar is back-to-back. And the information I actually need to make decisions is scattered across email, Slack, dashboards, and Google Drive documents that my team updates at different cadences.

What I don't need is another summary. I need a **strategic command view** — something that tells me what requires my attention, what's working, what's broken, and what's about to become a problem before it does.

Using my connected sources (Gmail, Calendar, Slack, Google Drive) — or the attached `bu_performance_summary.csv`, `ceo_inbox_highlights.csv`, and `stakeholder_calendar.json` as fallback — build me a CEO Strategic Briefing.

### What I Need

**1. Decisions Pending on Me**
The single most important section. Surface anything where:
- A direct report is waiting for my input or approval
- A deal, partnership, or regulatory decision has a deadline this week
- An escalation has come through that only I can resolve
- A board member or investor has asked me something directly

For each item: what it is, who's waiting, what the deadline is, and what the recommended action is based on context.

**2. Business Unit Pulse**
One-line status for each business line — Payments, Custody, RLUSD, Prime (Hidden Road), Treasury (GTreasury). For each:
- Key metric vs. target (one number that tells the story)
- Trend: improving, stable, or declining
- Flag anything that's off-track with a brief "why"

I don't want a full dashboard here — I want the 30-second scan that tells me where to dig in.

**3. External Radar**
What's happening outside the company that I need to know:
- Competitive moves (SWIFT, Circle, Stellar, JPMorgan Kinexys, Visa B2B Connect)
- Regulatory developments in our key markets
- Crypto market conditions that affect our business (XRP price, ETF flows, institutional sentiment)
- Media coverage of Ripple or our competitors

For each: what happened, why it matters to us, and whether I need to do anything about it.

**4. Stakeholder Prep**
For each meeting on today's calendar:
- Who I'm meeting and their current context (what they care about, what they last asked about)
- 2-3 key talking points informed by recent developments
- Anything I should avoid or handle carefully
- Documents I should review beforehand

For investor or media engagements: recent coverage, market narrative, and the framing I should use.

**5. People & Org Signals**
Things the CEO should know about the team:
- Key hires or departures this week
- Acquisition team retention signals
- Any Slack/email patterns suggesting a team is struggling (high volume, after-hours activity, escalation frequency)
- Cultural moments worth recognizing

**6. What Can Wait**
Items in my inbox or Slack that look urgent but aren't. For each, recommend: delegate (to whom), defer (until when), or drop.

### Output Format
Clean, scannable document. Use headers and bold text for key names, numbers, and dates. This is a 7 AM read — it needs to work on a phone screen. Decisions Pending on Me should always be first. Keep the full briefing under 4 pages.

---

## How This Is Different From a Dashboard

Dashboards show you data. This shows you **what to do about the data.** The difference:

1. **Cross-references sources** — Links your calendar to the relevant emails and Slack threads, so stakeholder prep isn't generic.
2. **Applies CEO-level priority logic** — Filters by decision authority, not just urgency. If someone else can handle it, it goes in "What Can Wait."
3. **Tracks the external environment** — A CEO briefing without competitive and regulatory context is incomplete.
4. **Learns your priorities** — After the first output, tell Claude what it got wrong. "I don't care about XRP price unless it moves more than 10%." "Always flag anything from the board." Each correction makes the next briefing smarter.

---

## Stretch Goals

1. **Weekly strategic digest** — A Friday version that synthesizes the week: decisions made, priorities shifted, pipeline changes, and what to watch next week.
2. **Board communication draft** — Based on the week's briefings, draft a concise board update email that BG can edit and send.
3. **Direct report 1:1 prep** — For each upcoming 1:1, generate a brief with that person's recent updates, open items, and suggested topics to raise.
