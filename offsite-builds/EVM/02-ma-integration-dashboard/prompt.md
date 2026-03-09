# M&A Integration Tracker Dashboard

## Prompt

I'm SVP of Strategic Initiatives at Ripple. I'm overseeing integration of our 2025 acquisitions: Hidden Road ($1.25B - prime brokerage), GTreasury ($1B - treasury management), Rail ($200M - B2B stablecoin payments), and Palisade (custody/wallet-as-a-service). I also need to track our 2023 Metaco acquisition ($250M - institutional custody).

Using the attached `integration_milestones.csv` data, build me an interactive HTML dashboard that shows:

1. **Acquisition Overview Cards** - One card per acquisition showing: deal value, close date, integration phase (Planning/In Progress/Complete), overall health (on track/at risk/blocked), team lead, and a progress bar showing % of milestones completed.

2. **Milestone Gantt View** - A timeline visualization of all integration milestones across acquisitions. Color-code by status (complete/on track/at risk/blocked). Allow filtering by acquisition and by workstream (Technology, People, Product, Legal, Finance, Go-to-Market).

3. **Cross-Product Synergy Tracker** - A matrix showing which product integration synergies have been identified, which are in progress, and which are complete. For example: "RLUSD as collateral on Hidden Road" or "Metaco custody integrated with GTreasury."

4. **Blockers & Risks Panel** - A prioritized list of current blockers and risks across all integrations, with owner, severity, and days open.

Make this a single interactive HTML file with Ripple brand colors (navy #1a237e, blue #2962ff). Include a summary header showing total acquisitions, total deal value, overall integration progress %, and count of open blockers.
