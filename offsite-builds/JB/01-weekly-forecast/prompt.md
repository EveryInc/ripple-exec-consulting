# Weekly Financial Forecast Summary

## Prompt

I'm CFO of Ripple. Every week I need to review our financial forecast and produce a summary for the executive team. This currently takes hours of manual work pulling data together.

Using the attached `weekly_financials.csv` data, build me a tool that:

1. **Reads the weekly financial data** and produces a clean, formatted executive summary report (as an HTML file I can open in my browser or print to PDF).

2. **The report should include:**
   - **Headline Numbers**: Total revenue (actual vs. forecast), total expenses, EBITDA, cash position, and week-over-week change for each.
   - **Revenue Breakdown by Business Line**: Ripple Payments, Ripple Custody, RLUSD, Ripple Prime, Ripple Treasury - actual vs. forecast with variance % and a visual bar chart.
   - **Expense Variance Analysis**: Any expense category where actuals exceed forecast by more than 10% should be flagged in red with an explanation field.
   - **Cash Flow Waterfall**: A visual showing starting cash, inflows, outflows, and ending cash position.
   - **Key Risks & Flags**: Auto-detect and surface: revenue lines trending below forecast, expense categories running hot, cash burn rate changes, and any line item with >15% variance.
   - **3-Week Trend**: Show the last 3 weeks of data with trend arrows (improving/stable/declining) for each major metric.

3. **Format it for exec consumption** - clean typography, Ripple brand colors (navy #1a237e, blue #2962ff), charts where appropriate. This should look like something I could present in a staff meeting.

Generate the report as a single HTML file.
