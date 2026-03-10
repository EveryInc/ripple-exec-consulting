# Competitive M&A Landscape

## Prompt

I'm CVP of Corporate & Business Development at Ripple. To evaluate new deals and defend our acquisition strategy to the board, I need a clear view of what our competitors are doing in M&A, partnerships, and strategic investments. Right now this intelligence is scattered across news alerts, analyst reports, Slack threads, and my own notes.

Using my connected sources (Gmail, Slack, Google Drive) — or the attached `competitive_deals.csv` as fallback — build me a Competitive M&A Landscape tracker.

### What I Need

**1. Competitor Deal Activity**
For each major competitor (SWIFT, Circle, Stellar, JPMorgan Kinexys, Visa B2B Connect, and any others active in our space):
- Recent acquisitions, investments, and strategic partnerships (last 12 months)
- Deal rationale and what it tells us about their strategy
- How it overlaps with or threatens Ripple's position

**2. Market Map**
A visual categorization of deals by strategic area:
- **Payments Infrastructure** (cross-border, B2B, real-time)
- **Digital Assets / Stablecoins** (issuance, custody, trading)
- **Treasury & Cash Management** (enterprise SaaS, bank connectivity)
- **Crypto Infrastructure** (prime brokerage, clearing, settlement)
- **Compliance & RegTech** (KYC, AML, transaction monitoring)

Show which players are active in which categories and where gaps or white space exists.

**3. Implications for Ripple**
For each significant competitive move:
- Does this change our competitive position?
- Does it validate or challenge our acquisition thesis?
- Should it accelerate, deprioritize, or create a new item in our pipeline?

**4. White Space Analysis**
Categories or capabilities where:
- No major competitor has made a move yet (first-mover opportunity)
- Multiple competitors are converging (crowded, proceed with caution)
- Ripple has a unique advantage through existing acquisitions

### Output Format
Interactive HTML dashboard with:
- A competitor-by-category matrix showing activity density
- A timeline of major deals in the last 12 months
- Sortable/filterable deal list
- Ripple's position highlighted relative to competitors

---

## Stretch Goals

1. **Deal thesis validator** — For any deal in our pipeline, ask Claude to compare it against competitive M&A activity and score whether the strategic rationale has strengthened or weakened.
2. **Board narrative** — Generate a 1-page competitive M&A summary for the quarterly board deck.
