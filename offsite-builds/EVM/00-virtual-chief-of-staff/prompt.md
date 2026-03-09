# Virtual Chief of Staff: Daily Executive Briefing

## Prompt

I'm SVP of Strategic Initiatives at Ripple. My day is a mix of competitive intelligence, M&A integration oversight, market activation across 50+ jurisdictions, and strategic partnerships. I get context from every direction — email, Slack, calendar, internal dashboards — but I have no chief of staff to synthesize it for me.

I've tried building something like this before and got stuck. The problem wasn't getting Claude to summarize — it was getting it to **connect dots across sources** and **prioritize what actually needs my attention** vs. what's noise.

Using my connected sources (Gmail, Calendar, Slack) — or the attached `sample_day.json` as a fallback — build me a Virtual Chief of Staff briefing that runs every morning.

### What I Need

**1. Today's Priority Stack**
Not just a to-do list. Rank my priorities by **impact and urgency**, considering:
- Deadlines that are today or this week
- Items where I'm the bottleneck (someone is waiting on me)
- Strategic opportunities with time sensitivity (partnership windows, competitive moves to respond to)
- Things that were flagged yesterday but I didn't act on

For each priority, give me: the item, who's involved, what I need to do, and what happens if I don't do it today.

**2. Meeting Prep Briefs**
For each meeting on today's calendar:
- **Context:** Why is this meeting happening? Link to recent emails or Slack threads about this topic.
- **Key people:** Who's attending and what's their current stance/interest?
- **My talking points:** 2-3 things I should raise based on recent developments.
- **Decision needed?** Is there a decision expected from this meeting? What's the context?
- **Prep materials:** Any documents or data I should review before walking in.

**3. Strategic Radar**
Things that aren't urgent today but I need to keep on my radar this week:
- Competitive moves (from news, Slack, or internal competitive intel channels)
- M&A integration milestones coming up
- Market activation updates across key jurisdictions
- Partnership pipeline changes

**4. Follow-Up Accountability**
Items from the past 3 days where:
- I said I'd do something and haven't yet
- Someone committed to delivering something to me and hasn't
- A thread went quiet without resolution

For each: what it was, who's involved, and how many days it's been.

**5. What I Can Delegate or Skip**
Messages, threads, and meetings where my involvement isn't critical. For each, suggest who else could handle it or whether I can simply acknowledge and move on.

### Output Format
Clean, scannable document. Use headers, bullet points, and bold for key names/dates. I read this at 7 AM on my phone — make it skimmable. No more than 3 pages.

---

## How This Is Different From What You Tried Before

If you've attempted a "daily briefing" prompt and got a generic summary — that's because a flat summary treats all inputs equally. This prompt does three things differently:

1. **Cross-references sources** — It links your calendar to relevant email/Slack threads, so meeting prep is contextual, not generic.
2. **Applies priority logic** — It uses urgency + impact + bottleneck signals to rank, not just recency.
3. **Tracks accountability** — It looks backward at commitments, not just forward at tasks.

The key to making this work well: **iterate on the priority logic.** After the first output, tell Claude what it got wrong. "That item isn't urgent because X." "You missed Y because it was in a Slack DM, not email." Each correction makes the next briefing better.

---

## Stretch Goals

1. **Weekly digest mode** — Ask Claude to generate a Friday summary of the week: what got done, what's still open, what shifted strategically.
2. **Competitive alert trigger** — Set up a pattern where Claude flags specific competitor moves (e.g., "alert me whenever SWIFT, Stellar, or Circle announces a new partnership").
3. **Delegation assistant** — For items you mark as "delegate," have Claude draft the handoff message to the right person.
