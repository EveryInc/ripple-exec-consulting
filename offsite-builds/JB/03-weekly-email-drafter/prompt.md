# Weekly Email Drafter

## Prompt

I'm CFO of Ripple. Every week I send a financial update email to the executive team (BG, ML, SA, EVM, KH, MK, and others). Writing this email from scratch each week takes 45-60 minutes even though the format is similar. I want to automate the first draft.

Using the attached `weekly_metrics.csv` data, draft a weekly financial update email that follows this format:

**Subject line:** "Weekly Financial Update - W/E [date]"

**Structure:**
1. **Opening line** - One sentence on overall performance (ahead/behind/on track vs. plan)
2. **Headline Numbers** (bullet points) - Total revenue, EBITDA, cash position, each with actual vs. forecast and the delta
3. **What's Working** (2-3 bullets) - Business lines or line items that beat forecast, with brief context on why
4. **What Needs Attention** (2-3 bullets) - Items below forecast or trending in the wrong direction, with enough context to understand the issue
5. **Cash & Liquidity** - One paragraph on cash position, burn rate, and any notable changes
6. **Looking Ahead** - 2-3 things to watch next week (upcoming client closes, expense milestones, etc.)
7. **Closing** - Brief, professional sign-off

**Tone guidelines:**
- Direct and concise - executives skim, not read
- Lead with insight, not data - explain what the numbers mean
- Flag risks early but don't catastrophize
- Celebrate wins briefly
- No jargon the non-finance execs wouldn't understand

Write the email as plain text (not HTML) that I can paste directly into Gmail. Also generate a short "TL;DR" version (3 sentences max) that I can post in the #exec-team Slack channel.
