# Team Update Aggregator & 1:1 Agenda Builder

## Prompt

I'm Chief Legal Officer at Ripple. I have 6 direct reports across different legal functions (litigation, regulatory, corporate, IP, compliance, and employment). They send me updates via email and Slack throughout the week. Before my 1:1s, I spend 20-30 minutes per person manually reviewing messages to build an agenda. I want to automate this.

Using the attached `team_updates.csv` (a week's worth of updates from my direct reports), build me a tool that:

1. **Aggregates by Person** - Group all updates from each direct report and extract:
   - Key accomplishments this week
   - Active matters/projects with status
   - Blockers or issues needing CLO input
   - Decisions they need from me
   - Items they mentioned but didn't follow up on (potential dropped balls)

2. **Generates 1:1 Agendas** - For each direct report, create a structured 1:1 agenda:
   - **Follow-ups from last week** (based on prior items marked "pending")
   - **Their updates** - summarized from this week's messages
   - **Discussion items** - things that need conversation, not just a status update
   - **Decisions needed** - specific decisions I need to make, with context
   - **My items for them** - placeholder section I can fill in

3. **Cross-Team View** - Show me a single dashboard of all active legal matters across all reports:
   - Regulatory matters by jurisdiction
   - Active litigation/disputes
   - M&A legal workstreams
   - Compliance initiatives
   - Color-code by urgency: routine (green), needs attention (yellow), escalation (red)

4. **Tracking** - Flag items that have appeared for 3+ weeks without resolution as "stale" - these are likely stuck and need escalation.

Output as a clean HTML document with a tab or section for each direct report's 1:1 agenda, plus the cross-team view.
