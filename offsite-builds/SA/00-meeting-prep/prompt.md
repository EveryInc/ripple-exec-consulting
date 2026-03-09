# Meeting Prep Workflow

## Prompt

I'm Chief Legal Officer at Ripple. I have back-to-back meetings most days — with my direct reports, cross-functional partners, external counsel, regulators, and board members. For each meeting, I need to walk in prepared: who's in the room, what we're discussing, what happened last time, and what decisions are on the table.

Right now I do this manually — scanning emails, checking Slack, reviewing my notes. It takes 15-20 minutes per meeting and I have 5-6 meetings a day. That's 90 minutes of prep I'd rather spend on actual legal work.

Using my connected sources (Gmail, Calendar, Slack) — or the attached sample files as a fallback — build me a meeting prep workflow.

### How It Should Work

Give me a calendar event (or pull from my actual calendar), and for each meeting produce:

**1. Meeting Brief**
- **Purpose:** Why is this meeting happening? One sentence.
- **Last meeting:** What happened last time we met on this topic? Key outcomes or open items.
- **Current status:** What's changed since last time? (Pull from recent emails/Slack about this topic or these attendees.)

**2. Attendee Context**
For each attendee:
- Their role and relationship to me
- Last time I interacted with them (email, Slack, or meeting)
- Any open items between us (things they owe me, things I owe them)
- One thing to be aware of (e.g., "just returned from parental leave" or "their team is going through reorg")

**3. Talking Points**
- 3-5 suggested talking points based on recent activity
- Any decisions that need to be made in this meeting
- Questions I should ask based on open threads or unresolved items

**4. Background Documents**
- Links or references to relevant documents, prior meeting notes, or email threads
- Any attachments that were shared related to this topic in the past week

### Output Format
One page per meeting. Clean headers, bullet points. I scan this on my phone between meetings — make it fast to read.

---

## Sample Data Files

- `sample_meetings.json` — 4 upcoming meetings with attendee lists and topics
- `attendee_context.csv` — Background info on attendees (role, last interaction, open items)

Upload these files if your calendar connector isn't available, or use them as examples to see the output format before switching to real data.

---

## The Real Value

If your calendar is connected, try this: ask Claude to prep you for your **actual next meeting**. No uploading files, no copy-pasting — just "What should I know before my 2pm call?"

That's the goal: zero-effort prep that's better than what you'd do manually.
