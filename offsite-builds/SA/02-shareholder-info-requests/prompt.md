# Shareholder Info Request Manager

## Prompt

I'm Chief Legal Officer at Ripple. Every quarter-end, we receive information requests from our shareholders (institutional investors, board members, and early investors). These requests come in via email, they need data from multiple internal teams, and tracking them manually is a mess. I need a system to manage this process.

Using the attached `shareholder_requests.csv` (sample quarter-end requests), build me a tool that:

1. **Request Tracker Dashboard** (HTML)
   - List all incoming shareholder requests with: requester, request date, what they're asking for, which internal team(s) need to provide data, deadline, and current status (Received > Assigned > In Progress > Under Review > Sent)
   - Color-code by status and flag anything overdue or due within 48 hours
   - Show overall progress: X of Y requests complete, average response time

2. **Auto-Assignment** - Based on the type of information requested, suggest which internal team should handle it:
   - Financial data → CFO/Finance team
   - Product metrics → Product/Engineering
   - Legal/regulatory → Legal team (my team)
   - HR/headcount → People team
   - Market/competitive → Strategy team

3. **Response Template Generator** - For common request types, generate a draft response email that:
   - Acknowledges the request
   - Provides the requested data (using the synthetic data in the attached file)
   - Includes standard disclaimers (confidential, forward-looking statements, etc.)
   - Is formatted professionally for institutional investors

4. **Follow-Up Tracker** - Generate reminder emails for:
   - Internal teams who haven't provided their data by the internal deadline
   - Shareholders who asked follow-up questions
   - Requests where we're approaching the external deadline

Output as an interactive HTML dashboard with the ability to filter by shareholder, status, and deadline.
