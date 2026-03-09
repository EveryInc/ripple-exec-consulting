# Your Daily Briefing: Synthesize My Chaos

## Exercise Overview

You're an executive at Ripple. Every morning, you face the same challenge: dozens of emails, Slack threads across multiple channels, and a packed calendar — all before your first meeting. The signal is buried in noise.

In this exercise, we'll build a **Daily Briefing** that pulls from your email, Slack, and calendar to produce a single, structured view of what actually matters today.

This isn't about drafting emails or summarizing text. It's about **synthesis** — connecting dots across sources that you'd normally hold in your head.

---

## What You'll Build

A personalized daily briefing that answers five questions:

1. **What needs my attention right now?** — Action items, approvals, decisions that are blocking someone
2. **What's happening today?** — Calendar overview with context on each meeting (who, why, what to know going in)
3. **What happened overnight that I should know about?** — Key Slack and email threads, filtered to what's relevant
4. **What's falling through the cracks?** — Items from yesterday/this week that don't have a clear owner or next step
5. **What can I ignore?** — FYIs, newsletters, threads where I'm CC'd but don't need to act

---

## Step-by-Step

### Step 1: Connect Your Sources (Already Done)
Your Claude Cowork instance has Gmail, Google Calendar, Slack, and Google Drive connectors pre-configured by IT. You're ready to go.

For this group demo, we'll use **sample data** so everyone works from the same inputs. You can switch to your real data during your individual build later.

### Step 2: Upload the Sample Data
Upload these three files to this conversation:
- `sample_inbox.csv` — A morning's worth of email threads
- `sample_slack.csv` — Recent Slack messages across key channels
- `sample_calendar.json` — Today's meeting schedule

### Step 3: Describe What You Want
Paste this prompt into Claude (then we'll refine it together):

---

> I'm an executive at Ripple. I've uploaded my email inbox, Slack messages, and today's calendar. Build me a daily briefing that synthesizes all three sources into a single actionable view.
>
> Structure it as:
>
> **1. Immediate Actions** — Things that need a decision or response from me today. For each item, tell me: what it is, who's waiting, and what the deadline or consequence of delay is.
>
> **2. Today's Meetings** — For each meeting on my calendar: who's attending, what it's about, any relevant context from recent emails or Slack threads about this topic, and 2-3 things I should know going in.
>
> **3. Overnight Digest** — Key updates from Slack and email since yesterday evening. Skip anything purely informational unless it changes something I care about. Group by theme, not by source.
>
> **4. Follow-Up Tracker** — Items from this week where someone committed to a deliverable or next step but I haven't seen a follow-up yet. Flag anything overdue.
>
> **5. Low Priority / Safe to Skip** — Threads where I'm CC'd, FYI-only messages, newsletters, and anything that doesn't require action. One-line summaries so I can scan and move on.
>
> Format this as a clean, scannable document. Use bullet points, not paragraphs. Bold the key names and deadlines. Keep it under 2 pages.

---

### Step 4: Refine Together
Once Claude generates the first briefing, we'll work through these refinements as a group:

- **Prioritization logic** — How should Claude decide what's "immediate" vs. "low priority"? What signals matter to you? (sender seniority? keywords like "urgent"? threads you're directly addressed in?)
- **Meeting prep depth** — Do you want a quick context line or a full brief for each meeting?
- **Tone and format** — Does this feel like something you'd actually read at 7 AM? What would you change?
- **What's missing?** — What would make this 10x more useful for your specific role?

### Step 5: Make It Yours (Stretch)
If time permits, try switching from sample data to your **real** connected sources. Ask Claude to pull from your actual Gmail, Calendar, and Slack to generate today's real briefing.

---

## Key Concepts We're Practicing

| Concept | How It Shows Up |
|---------|----------------|
| **Multi-source synthesis** | Combining email + Slack + calendar into one view |
| **Structured output** | Getting Claude to produce a specific, scannable format |
| **Iterative refinement** | Starting broad, then tuning the output to your preferences |
| **Context connectors** | Using MCP connectors to pull from real tools (stretch goal) |

---

## Facilitator Notes
- This exercise is about the **synthesis** capability, not the drafting capability. If participants say "I could just read my email," redirect: "Yes, but could you cross-reference it with your calendar and Slack in 30 seconds?"
- The "aha" moment is when Claude connects an email thread to an upcoming meeting they hadn't prepared for.
- Encourage participants to challenge the output: "What did it miss? What did it get wrong?" This builds trust through verification, not blind acceptance.
