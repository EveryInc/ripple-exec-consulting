# Comms Inbox Organizer

## Prompt

I'm SVP of Marketing and Communications at Ripple. I use my email inbox as my filing system and I have thousands of emails. I need a way to quickly search, categorize, and surface what needs my attention.

Using the attached `inbox_sample.csv` (a sample export of recent emails), build me a tool that:

1. **Daily Digest View** - Organize today's emails into categories:
   - **Needs My Response** - emails directly asking me for input, approval, or decision
   - **FYI / Keep Track** - emails I'm CC'd on or that are informational
   - **Vendor/External** - agency, vendor, or partner communications
   - **Media & Press** - journalist inquiries, media opportunities, press mentions
   - **Internal Approvals** - contracts, POs, budget requests awaiting sign-off
   - **Delegatable** - things my team should handle, not me directly

2. **Priority Scoring** - Rate each email 1-5 based on:
   - Sender importance (CEO/President = 5, direct report = 4, cross-functional = 3, external = 2, unknown = 1)
   - Time sensitivity (deadline today = 5, this week = 3, no deadline = 1)
   - Topic criticality (crisis/media = 5, event logistics = 3, routine = 1)

3. **Action Summary** - For each email that needs my response, draft a 1-sentence summary of what's needed and a suggested response approach (approve, push back, delegate to [person], schedule meeting, etc.)

4. **Search & Filter** - Make the output filterable by category, priority, sender, and date range.

Output as a clean, interactive HTML dashboard. Show the highest-priority items at the top with clear visual hierarchy.
