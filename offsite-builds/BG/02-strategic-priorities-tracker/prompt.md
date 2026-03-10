# Strategic Priorities Tracker

## Prompt

I'm CEO of Ripple. We have 8-10 company-level strategic priorities at any given time — acquisition integrations, product launches, regulatory milestones, major partnerships, and organizational initiatives. Each one has an owner on my leadership team, but I don't have a single view of where they all stand. I find out something is off-track when it shows up in my inbox as an escalation.

Using my connected sources (Gmail, Slack, Google Drive) — or the attached `strategic_priorities.csv` as fallback — build me a Strategic Priorities Tracker.

### What I Need

**1. Priority Dashboard**
For each strategic priority:
- **Priority name and owner** (which direct report owns this)
- **Status:** On Track / Needs Attention / At Risk / Complete
- **Progress:** percentage or milestone-based
- **Target date** and whether it's slipping
- **Last update:** when was this last meaningfully updated, and by whom
- **Key metric** — the one number that tells me if this is working

**2. Attention Required**
Separate section showing only the priorities that need my involvement:
- Decisions pending on me
- Items that have slipped more than 2 weeks
- Priorities where the owner hasn't provided an update in 10+ days
- Cross-priority conflicts (two priorities competing for the same resource)

**3. Quarterly Progress View**
A visual showing where each priority started the quarter vs. where it is now. I want to see velocity, not just current status.

**4. Dependencies Map**
Which priorities depend on each other? If GTreasury cloud migration slips, what else is affected? If the FCA conditions aren't met on time, what deals are at risk?

### Output Format
Interactive HTML dashboard with:
- Card-based layout for each priority with RAG status, owner, and key metric
- A filterable view (by owner, by status, by business unit)
- Sparkline-style progress indicators
- "Attention Required" section pinned at the top
- Clean enough to project in a leadership meeting

---

## Stretch Goals

1. **Weekly CEO update generator** — From the tracker, auto-generate a weekly email to the leadership team summarizing cross-company priorities, what's on track, and what needs escalation.
2. **Board priorities view** — A simplified version showing only board-level priorities with talking points for each.
3. **Historical trend** — Track how priority status has changed over the last 4 weeks to identify patterns (e.g., "this priority has been Yellow for 3 weeks straight").
