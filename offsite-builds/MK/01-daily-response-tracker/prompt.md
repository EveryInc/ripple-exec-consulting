# Daily Response Tracker & To-Do Generator

## Prompt

I'm SVP of People, Places, and IT at Ripple. My inbox and Slack are constantly overloaded. I need a daily check-in tool that tells me: what do I owe people a response to, and what should my to-do list look like today?

Using the attached `pending_items.csv` (a sample of recent emails and Slack messages that need my attention), build me a tool that:

1. **Response Tracker** - Show me everything I owe someone a response to, organized by:
   - **Overdue** (should have responded already - red)
   - **Due Today** (expected response today - yellow)
   - **This Week** (no hard deadline but shouldn't sit longer - green)

   For each item show: who it's from, what channel (email/Slack), when it was received, what they're asking for, and a suggested response (1-2 sentences).

2. **Daily To-Do List** - Generate a prioritized to-do list for today based on:
   - Items I owe responses to
   - Meetings on my calendar today (prep needed?)
   - Recurring weekly tasks (e.g., people leads update doc, BG weekly update)
   - Deadlines approaching this week

   Rank by: CEO/President requests first, then direct report needs, then cross-functional, then external.

3. **Delegation Suggestions** - For items that could be handled by someone on my team, suggest who should take it and draft a quick forwarding message.

4. **Daily Summary Stats** - Show: total pending items, average response time, items closed yesterday, new items today, and a "inbox zero" progress bar.

Output as a clean HTML dashboard I can open every morning. Make it look like a personal command center - high information density but scannable.
