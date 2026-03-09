# JB — CFO

## Survey Response
- **Tools interested in:** Claude Cowork, Claude Code
- **Tasks to hand off to AI:**
  1. Weekly Forecast
  2. Company KPI Dashboards
  3. Skill Builder for Weekly Emails

## Session Build

### Primary: Exercise 00 — Team Update Aggregator & 1:1 Agendas (Finance Edition)
**Complexity:** Hard | **Estimated time:** 35-45 min (initial aggregation ~15 min, then refinement + Code track)

Ingests finance team updates (email/Slack from FP&A, Accounting, Treasury, Tax, IR, and GTreasury BU), extracts key items, generates structured 1:1 agendas and a cross-team finance operations dashboard. Adapted from the legal team pattern but reframed for CFO-specific workflows: close process, audit prep, forecast variances, treasury positions, investor relations.

**Claude Code stretch goal:** Automate the aggregation as a recurring script, or build a CLI tool that pulls from Gmail API directly. Jon is a power user and AI advocate — point him at Code and let him run.

### Optional Deep-Dives (Stretch / Follow-Up)

#### 1. Weekly Financial Forecast Summary
Auto-generate a polished weekly forecast report from raw financial data. Highlights revenue trends, expense variances, cash position changes, and flags items that need CFO attention. Produces both a structured report and a one-page executive summary.

#### 2. Executive KPI Dashboard
A cross-functional KPI dashboard pulling metrics from all five Ripple business lines (Payments, Custody, RLUSD, Prime, Treasury) into one unified view with trend indicators, RAG status, and drill-down capability.

#### 3. Weekly Email Drafter
Takes raw KPI and financial data and drafts a compelling, concise weekly update email for the executive team. Learns a consistent voice and format, highlights what matters, and flags what needs discussion.

## Facilitator Notes
- **Support level:** Self-directed. Jon is a power user and AI advocate — "could point him at Code. Let him run."
- **Claude Code track:** The prompt includes a stretch goal section for Code. If Jon finishes the Cowork build early, redirect him to automating the workflow with Code. This is the optional advanced track for the session.
- **If he finishes everything:** The Weekly Forecast (Exercise 01) and KPI Dashboard (Exercise 02) are natural extensions and directly align with his survey responses.
