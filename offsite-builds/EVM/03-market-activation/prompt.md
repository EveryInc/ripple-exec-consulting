# Market Activation Tracker

## Prompt

I'm SVP of Strategic Initiatives at Ripple. We've launched 8 new markets in the past 2 years and have more in the pipeline. I need a dashboard to track our global expansion at a glance.

Using the attached `markets.csv` data, build me an interactive HTML dashboard that includes:

1. **World Map View** - A visual map (or region-based grid) showing all markets color-coded by status: Active (green), Launching (yellow), Pipeline (blue), Regulatory Pending (orange). Show partner count and license status on hover/click.

2. **Market Detail Table** - Sortable table with all markets showing: region, country, status, license type, license status, number of active partners, ODL corridor status, monthly transaction volume, and launch date.

3. **Pipeline Funnel** - Visual funnel showing how many markets are in each stage: Pipeline > Regulatory Application > License Granted > Partner Onboarding > Active. Include average time to move between stages.

4. **Alerts Panel** - Surface markets where: license applications are overdue, partner activation is below target, volume is declining, or regulatory requirements have changed.

5. **Summary Stats** - Total active markets, total partners, total monthly volume, licenses pending, and a trend line showing market launches over time.

Single HTML file, Ripple brand colors (navy #1a237e, blue #2962ff, accent green #00c853 for active markets). Make it filterable by region and status.
