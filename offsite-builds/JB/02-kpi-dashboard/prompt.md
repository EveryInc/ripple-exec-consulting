# Executive KPI Dashboard

## Prompt

I'm CFO of Ripple. I need a single dashboard that gives me a cross-functional view of how all five business lines are performing, updated weekly. Right now this information lives in 5+ different spreadsheets and reports.

Using the attached `kpi_data.csv`, build me an interactive HTML dashboard that includes:

1. **Top-Level Scorecard** - A row of key company-wide metrics at the top: total weekly revenue, total active institutional clients, cumulative payment volume, RLUSD market cap, XRP price, and employee headcount. Each with a week-over-week trend indicator.

2. **Business Line Performance Cards** - One card per business line (Payments, Custody, RLUSD, Prime, Treasury) showing their top 3-4 KPIs with actual vs. target, RAG status (Red/Amber/Green), and a sparkline trend over the last 8 weeks.

3. **Cross-Functional Alerts** - Auto-flag any KPI that is: >10% below target (red), 5-10% below target (amber), or >10% above target (notable positive, blue highlight). This should be a filterable list.

4. **Trend Charts** - Clickable/expandable line charts for each KPI showing the 8-week trend. Allow comparison of multiple KPIs on one chart.

5. **Business Line Comparison** - A stacked bar chart showing revenue contribution by business line over the last 8 weeks, so I can see how the revenue mix is evolving.

Make this a single polished HTML file with Ripple brand colors. It should feel like a Bloomberg terminal for Ripple's business - dense but clear.
