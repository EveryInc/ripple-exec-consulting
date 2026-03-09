# Executive Program Follow-Up Engine

## Prompt

I'm VP of Strategic Initiatives at Ripple. One of my responsibilities is executive programs — offsites, training sessions, board prep coordination, and leadership development initiatives. After every session, there are action items, commitments, and follow-ups scattered across notes, emails, and Slack. Tracking who committed to what — and whether they actually did it — is manual and easy to let slip.

I want a follow-up engine that takes post-session notes and turns them into an accountability system.

### How It Works

**Input:** Meeting notes, session summaries, or action item lists from an exec session (upload a doc, paste notes, or pull from Google Drive).

**Output:**

### 1. Action Item Extraction
From the session notes, extract every commitment and action item:
- **Who** committed to it (or was assigned)
- **What** they committed to do
- **When** it's due (explicit deadline or inferred from context)
- **Context** — why this matters / what it's connected to
- **Status** — Not Started / In Progress / Done / Overdue

### 2. Accountability Dashboard
A clean view grouped by person showing:
- Their total action items from this session
- How many are complete vs. outstanding
- Any items that are overdue
- Items with dependencies on other people's actions

### 3. Follow-Up Drafts
For items approaching their deadline or overdue, generate:
- A brief, professional nudge message (email or Slack) I can send
- Tone: helpful, not nagging. "Checking in on X — let me know if you need anything to move this forward."
- Include the original context so the recipient doesn't have to dig back through notes

### 4. Weekly Follow-Up Report
A summary I can send to the session organizer or exec sponsor:
- Items completed since last report
- Items still outstanding with status
- Items at risk of slipping
- Recommended escalations

### Output Format
Interactive HTML with a per-person view, a timeline view, and exportable follow-up messages.

---

## Try It With Today's Session

After this offsite, you'll have real action items to track. Use this tool on the session notes:

1. Upload the session notes or facilitator debrief
2. Let Claude extract every commitment ("JB said he'd automate the weekly forecast," "ML needs to finish board deck section by Wednesday," etc.)
3. Generate the accountability dashboard
4. Draft follow-up messages for next week

This is the tool that makes sure the offsite actually leads to behavior change — not just a good afternoon.

---

## Stretch Goals

1. **Recurring check-ins** — Set up a weekly cadence where Claude checks in on outstanding items and generates the follow-up report automatically
2. **Cross-session tracking** — Track action items across multiple sessions (this offsite, the next exec sync, board prep meetings) in a single view
3. **Completion trends** — Over time, show completion rates by person and by session type. Who follows through? Which types of sessions generate the most actionable outcomes?
