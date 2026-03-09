# KPI Dashboard: Business Unit Performance View

## Prompt

I'm the CEO of a business unit within Ripple — we run an enterprise treasury management SaaS platform (acquired in late 2025). I report to Ripple's CEO and CFO and need to present clear performance metrics both to my team and to Ripple leadership. I want a KPI dashboard that gives me a real-time view of my business.

Using the attached data files (`kpi_data.csv` for core business metrics, and optionally `salesforce_export.csv` for pipeline data), build me a dashboard that covers:

### 1. Business Health Metrics
- **ARR** — Current annual recurring revenue, trend vs. prior quarter, and vs. plan
- **Net Revenue Retention** — Expansion, contraction, and churn broken out
- **Customer Count** — Total active customers by segment (Enterprise, Mid-Market, SMB)
- **New Logos** — New customers won this quarter with deal size and segment
- **Gross Margin** — Revenue vs. COGS trend

### 2. Product & Adoption
- **Feature Adoption Rates** — % of customers using key platform capabilities (cash forecasting, payment hub, bank connectivity, risk management)
- **Platform Usage** — DAU/MAU ratio, average session duration, API call volume
- **NPS / Customer Satisfaction** — Current score and trend

### 3. Pipeline & Growth
- **Sales Pipeline** — Deals by stage, weighted pipeline value, expected close dates
- **Win Rate** — By segment and deal size
- **Average Deal Size** — Trend over last 4 quarters
- **Top Deals** — 5 largest active opportunities with status

### 4. Integration with Ripple
- **Integration Milestones** — Status of product integrations (Ripple Custody, RLUSD settlement, cross-border payments connector)
- **Synergy Pipeline** — Cross-sell opportunities identified through Ripple's existing customer base
- **Shared Customer Count** — Customers using both GTreasury and Ripple products

### 5. Operational Health
- **Support Ticket Volume** — Trend, resolution time, escalation rate
- **Implementation Pipeline** — New customer onboarding status and timeline
- **Engineering Velocity** — Sprint completion rate, release cadence (optional)

**Output as a single interactive HTML dashboard.** Use a clean, modern design with:
- Card-based layout for each KPI with the number, trend arrow, and RAG status
- A section for each category above
- Sparkline-style trend charts where applicable
- Color coding: Green (on/above target), Yellow (within 5% of target), Red (below target)

---

## Stretch Goals (If Time Permits)

1. **Drill-down capability** — Click on a KPI card to see the underlying data
2. **Executive summary** — Auto-generate a 3-sentence narrative summary of the dashboard ("ARR is growing at X%, driven by...")
3. **Connect to Tableau** — If your Tableau connector is working, pull real data instead of the sample CSV
4. **Alerts view** — A separate panel showing only metrics that need attention (Yellow or Red status)
