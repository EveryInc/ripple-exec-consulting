# Editorial Assistant

## Prompt

I'm SVP of Marketing and Communications at Ripple. I don't originate much content anymore, but I edit everything - emails, press releases, tweets, briefing docs, event copy, brand campaigns. I need an AI editorial assistant that can take a first pass before I do my review.

Using the attached `drafts_to_edit.md` file (which contains several draft pieces across different formats), review each one and provide:

1. **For each draft, produce:**
   - **Format**: What type of content this is (press release, social post, exec email, event copy, etc.)
   - **Audience**: Who this is for
   - **Overall Assessment**: 1-2 sentences on quality and readiness (scale: Ready to Send / Needs Minor Edits / Needs Significant Rework)
   - **Tone & Voice Check**: Is this consistent with Ripple's brand voice? (Professional, authoritative, forward-looking, not hype-y or overly crypto-bro. Ripple positions itself as enterprise infrastructure, not speculative crypto.)
   - **Clarity & Concision**: Flag any sentences that are unclear, too long, or use unnecessary jargon
   - **Factual Accuracy Flags**: Anything that looks wrong or unverifiable (stats, claims, dates)
   - **Suggested Edits**: A clean revised version with tracked changes explained in brackets
   - **Headline/Subject Line Alternatives**: 2-3 options if the current one could be stronger

2. **Output format**: For each draft, show the original and the revised version side by side (or in sequence), so I can quickly compare. Use a clean HTML format with color-coded highlights: green for additions, red strikethrough for deletions, yellow for factual flags.

Generate as a single HTML file I can open in my browser.

---

## Tone & Voice Training

The biggest lever for making AI-edited content sound like *you* (not a robot) is teaching Claude your voice. Here's how:

### Step 1: Feed Claude Your Writing Samples
Before asking Claude to edit anything, give it 3-5 examples of writing you're proud of — emails, memos, social posts, anything that sounds like you. Then say:

> "Analyze these writing samples and describe my communication style. What patterns do you see in tone, word choice, sentence structure, and formality level? Summarize my voice in 5 bullet points."

Claude will generate a voice profile you can review and correct.

### Step 2: Set Voice Guidelines
Once you've validated the voice profile, use it as a constraint for all future edits:

> "When editing the drafts below, match this voice profile:
> - Professional but warm — never stiff or corporate
> - Direct — lead with the point, not the preamble
> - Confident but not arrogant — state positions clearly without hedging
> - No jargon — if a term wouldn't make sense to a smart non-crypto person, rephrase it
> - Active voice always — never 'it was decided,' always 'we decided'"

### Step 3: Before/After Calibration
For your first few edits, ask Claude to show you:
1. The original draft
2. The "generic AI edit" (what it would produce without voice training)
3. The "voice-matched edit" (using your profile)

Comparing #2 and #3 shows you exactly how much the voice training matters. This is the difference between "AI sounds robotic" and "AI sounds like me."

### Example Voice Guide
You can also upload a mini style guide (see `sample_voice_guide.md` if provided). A simple version:

```
RIPPLE COMMS VOICE GUIDE
- Tone: Professional, warm, direct. Never corporate jargon.
- We say: "Ripple enables..." not "Ripple is a leading provider of..."
- We say: "enterprise infrastructure" not "crypto" (unless specifically about XRP/RLUSD)
- Headlines: Action-oriented, specific. Not "Ripple Announces Partnership" → "Ripple and Santander Launch Brazil-Mexico Payment Corridor"
- Numbers: Always provide context. Not "$500M market cap" → "$500M market cap, doubling since launch in December"
- Avoid: "excited to announce," "thrilled," "game-changing," "revolutionary," "synergies"
```

### Why This Matters
Without voice training, Claude produces competent but generic prose. With voice training, it produces a first draft that's 80% you — which means your editing time drops from "rewrite everything" to "tweak and approve." That's the difference between AI being useful and AI being a tool you actually use.
