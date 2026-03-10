# Deal Pipeline & Integration Tracker

## Prompt

I'm CVP of Corporate & Business Development at Ripple. I run two workstreams simultaneously: **new deal pipeline** (partnerships, investments, and acquisitions under evaluation) and **post-close integration** for our 2025 acquisitions (Hidden Road, GTreasury, Rail, Palisade). The information for both lives in different places — CRM, email, Slack, internal trackers, Google Drive docs — and I spend hours every week manually stitching together a coherent view of where everything stands.

What I need is a **corporate development command center** — a single view that shows me the full picture: what's active, what's closing, what's integrating, what's stalled, and where deals and integrations create dependencies on each other.

Using my connected sources (Gmail, Slack, Google Drive) — or the attached `deal_pipeline.csv` and `integration_status.csv` as fallback — build me a Deal Pipeline & Integration Tracker.

### What I Need

**1. Active Deal Pipeline**
A stage-by-stage view of every active opportunity:
- **Deal name, type** (acquisition, strategic partnership, investment, licensing)
- **Stage** (Screening → Due Diligence → Negotiation → Approval → Closing)
- **Strategic rationale** — why this deal matters in one sentence
- **Deal value / investment size** — range or estimate
- **Key dates** — next milestone, expected close, any hard deadlines
- **Owner** — who on my team is running point
- **Status** — On Track / Needs Attention / At Risk / On Hold
- **Top blocker** — the one thing that could delay or kill this deal

Sort by urgency: deals closest to decision points first.

**2. Integration Status — 2025 Acquisitions**
For each of the four 2025 acquisitions, show:
- **Overall integration progress** — percentage complete, on/off track
- **Key milestones this quarter** — what's due and where it stands
- **Integration dimensions:** Technology, People, Customers, Product Synergies — RAG status for each
- **Budget vs. actuals** — are integration costs on plan?
- **Retention** — acquired team retention rate
- **Top risk** — the one thing keeping me up at night for this integration

**3. Cross-Deal Dependencies**
This is the part no one tracks well. Surface where:
- A new deal depends on an integration completing (e.g., "Partnership X assumes GTreasury cloud migration is done")
- Two integrations compete for the same resources (engineering, legal, compliance)
- A pipeline deal would change the priority of an active integration
- Timeline conflicts exist between deal milestones and integration milestones

**4. Weekly Action Items**
For the current week:
- Decisions I need to make
- Meetings to prep for (with context)
- Items where someone is waiting on me
- Deadlines that are approaching

**5. Stale Deal Detection**
Flag any deal or integration workstream where:
- No update has been logged in 10+ days
- A milestone has slipped twice
- The status hasn't changed in 3+ weeks

### Output Format
Interactive HTML dashboard. Use a card-based layout with:
- Pipeline section with deals as cards, organized by stage (kanban-style)
- Integration section with one panel per acquisition, showing dimension-level RAG status
- Dependencies section highlighting conflicts and resource contention
- Action items as a checklist at the top
- Color coding: Green (on track), Yellow (needs attention), Red (at risk), Gray (on hold)

---

## Stretch Goals

1. **Board-ready summary** — Generate a one-page corporate development update suitable for the board deck, covering pipeline highlights and integration progress.
2. **Resource contention map** — Visual showing which internal teams (engineering, legal, compliance, finance) are stretched across how many deals and integrations simultaneously.
3. **Deal scoring model** — Ask Claude to score pipeline deals by strategic fit, financial attractiveness, execution complexity, and resource availability.
