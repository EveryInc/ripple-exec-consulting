# Weekly Pipeline & Usage Intelligence Report

## Prompt

I'm President of Ripple. I need a weekly report that surfaces the key insights from our sales pipeline and customer product usage - not just raw data, but what the data is telling us. Currently this requires pulling from multiple systems and teams.

Using the attached `pipeline_data.csv` and `usage_data.csv`, generate a weekly intelligence report that includes:

1. **Pipeline Summary Dashboard** (HTML)
   - Total pipeline value by stage (Prospect > Qualified > Proposal > Negotiation > Closed Won/Lost)
   - Pipeline by product line and by region
   - Week-over-week changes: new opportunities added, deals advanced, deals lost
   - Weighted pipeline forecast for next 30/60/90 days
   - Conversion rates by stage with trend indicators

2. **Key Insights** (narrative section)
   - Top 5 deals to watch (largest, most likely to close, at risk of slipping)
   - Product demand signals: which products are seeing the most pipeline growth?
   - Regional patterns: where is momentum building or stalling?
   - Competitive losses: why are we losing deals and to whom?

3. **Usage Intelligence** (from product data)
   - Active vs. contracted clients by product line
   - Usage trends: which clients are ramping up? Which are going quiet?
   - Feature adoption rates for key capabilities (ODL, RLUSD settlement, cross-margining)
   - Churn risk signals: clients with declining usage patterns

4. **Recommended Actions** - Based on the data, what should leadership focus on this week? (e.g., "Schedule executive sponsor call for [deal]", "Investigate declining usage at [client]", "Fast-track [product feature] based on demand signal")

Output as a polished HTML report. Make it the kind of thing I can read in 10 minutes over morning coffee and walk into any meeting informed.
