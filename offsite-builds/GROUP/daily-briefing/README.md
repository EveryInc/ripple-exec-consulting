# Group Exercise: Your Daily Briefing

**Session slot:** 11:30 AM - 12:30 PM (60 minutes)
**Tool:** Claude Cowork with MCP connectors (Gmail, Calendar, Slack, Google Drive)

---

## Overview

This is the opening guided build for the entire group. Participants work together through a shared exercise that demonstrates multi-source synthesis — combining email, Slack, and calendar data into a single actionable daily briefing.

The theme is **"Synthesize My Chaos"** — the dominant need expressed by 5 of 7 survey respondents.

---

## Timing Guide

| Time | Activity | Facilitator Action |
|------|----------|-------------------|
| 11:30 - 11:35 | Intro & framing (5 min) | Mike sets context: "Every morning you face 50 emails, 30 Slack threads, 6 meetings. What if you could get a single briefing that connects all of it?" |
| 11:35 - 11:45 | Upload data & first prompt (10 min) | Walk group through uploading sample files and pasting the prompt from `prompt.md` |
| 11:45 - 12:00 | Review output together (15 min) | Project Claude's output. Ask: "What did it get right? What's missing? What would you change?" |
| 12:00 - 12:15 | Refinement round (15 min) | Group suggests improvements. Demonstrate iterative prompting — priority logic, format changes, meeting prep depth |
| 12:15 - 12:25 | Live connector demo (10 min) | Switch from sample data to a real connected source (Mike's or a volunteer's). Show the "aha" moment of pulling real data |
| 12:25 - 12:30 | Wrap-up & bridge to individual builds (5 min) | "Now you'll build something like this — but tailored to your specific role and workflow." |

---

## Files

| File | Purpose |
|------|---------|
| `prompt.md` | The exercise brief — step-by-step instructions for participants |
| `sample_inbox.csv` | 15 dummy email threads (action items, FYIs, approvals, team updates) |
| `sample_slack.csv` | 10 dummy Slack messages across #exec-team, #product-updates, #legal-regulatory, DMs |
| `sample_calendar.json` | A day of 5 meetings with attendees, agendas, and prep context |

---

## Talking Points

- **Why synthesis, not summarization:** "AI can summarize a single email. The real value is connecting your 9am meeting to the Slack thread from last night and the email approval that's blocking the agenda."
- **The 5-question framework:** What needs action? What's today? What happened overnight? What's slipping? What can I skip?
- **Trust through verification:** "Don't trust the briefing blindly. Check it against what you know. That's how you calibrate it to your standards."

---

## Common Participant Questions

- **"Can it pull from my real email?"** — Yes, connectors are pre-configured. We use sample data for the group demo so everyone's on the same page. You'll switch to real data in your individual build.
- **"How does it know what's urgent?"** — It doesn't, initially. That's what refinement is for. You teach it your priority logic: "Anything from Brad is always high priority. Anything CC-only is low."
- **"What about confidentiality?"** — Claude processes data in your session only. Nothing is stored or used for training. IT has reviewed and approved the connector permissions.

---

## Facilitator Notes

- **Do NOT frame this as "drafting."** The value prop is synthesis across sources, not text generation. If someone says "I could just read my email," redirect: "But could you cross-reference it with your Slack and calendar in 30 seconds?"
- **Pause for reactions** after the first output. Let participants react naturally — the best insights come from their surprise at what Claude noticed (or missed).
- **Bridge to individual builds** at the end: each participant's exercise uses this same pattern (multi-source synthesis) but tailored to their role.
- **If connectors fail during live demo:** pivot gracefully to the sample data. "This is why we always have a sample data fallback — same workflow, guaranteed to work."
