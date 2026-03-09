# Team Update Aggregator & 1:1 Agenda Builder (CFO Edition)

## Prompt

I'm CFO at Ripple. I have direct reports leading FP&A, Accounting, Treasury, Tax, and Investor Relations — plus the newly integrated GTreasury business unit. They send me updates via email and Slack throughout the week: close process status, audit prep, forecast variances, investor questions, treasury positions, and GTreasury integration updates. Before my 1:1s, I spend 20-30 minutes per person reviewing messages to build an agenda. With 6 reports, that's 2+ hours a week on meeting prep alone.

Using the attached `team_updates.csv` (a week of updates from my finance team), build me a system that:

### 1. Aggregate by Person
Group all updates from each direct report and extract:
- Key deliverables completed this week
- Active workstreams with current status
- Blockers or issues needing CFO input
- Decisions they need from me
- Budget or forecast variances I should know about
- Items mentioned previously but not followed up on (potential dropped balls)

### 2. Generate 1:1 Agendas
For each direct report, create a structured 1:1 agenda:
- **Follow-ups from last week** — Items previously marked "pending" or "in progress"
- **Their updates** — Summarized from this week's messages
- **Discussion items** — Things requiring conversation, not just status
- **Decisions needed** — Specific decisions with context and my options
- **Budget/forecast flags** — Any variances, overruns, or reforecasts
- **My items for them** — Placeholder section I can fill in

### 3. Finance Operations Dashboard
A single cross-team view of all active finance workstreams:
- **Monthly/quarterly close** — Status, timeline, blockers
- **Audit & compliance** — External audit prep, regulatory filings, SOX
- **Treasury & cash management** — Cash positions, investment portfolio, debt facilities
- **Tax** — Active matters, upcoming filings, transfer pricing
- **Investor relations** — Upcoming events, analyst questions, shareholder communications
- **GTreasury integration** — Financial integration milestones, combined reporting
- Color-code by status: on track (green), needs attention (yellow), escalation (red)

### 4. Stale Item Tracker
Flag items appearing for 3+ weeks without resolution. These are stuck and need escalation or a decision to deprioritize.

### Output
Generate as a clean HTML document with:
- A tab/section for each direct report's 1:1 agenda
- The cross-team finance operations dashboard
- A stale items summary at the top

---

## Stretch Goal: Claude Code Track

If you're comfortable with Claude Code (or want to try it), here's an advanced challenge:

**Automate this as a recurring workflow:**
1. Write a script that pulls updates from Gmail API (filter by sender + date range)
2. Processes them through the aggregation logic above
3. Outputs the formatted 1:1 agendas and dashboard
4. Runs on a schedule (e.g., Sunday evening, ready for Monday morning)

This turns a manual weekly task into a zero-touch system. Ask your facilitator about Claude Code if you want to explore this track.
