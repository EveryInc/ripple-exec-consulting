# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **curriculum repository** for an executive AI training offsite at Ripple. It contains structured exercises, sample data, and facilitator guides for teaching Ripple's leadership team to use Claude Cowork (with MCP connectors) and optionally Claude Code.

There is no application code, build system, or test infrastructure. The deliverables are **Markdown prompts, CSV/JSON sample data, and facilitator documentation**.

## Repository Structure

```
offsite-builds/
├── GROUP/daily-briefing/    # Shared opening exercise (60 min, 11:30-12:30)
├── EVM/                     # SVP Strategic Initiatives
├── JB/                      # CFO
├── KH/                      # SVP Marketing & Comms
├── MK/                      # SVP People, Places, IT
├── ML/                      # President
├── RN/                      # CEO, GTreasury BU
└── SA/                      # CLO
```

Each executive folder contains:
- `README.md` — Participant profile, primary vs. stretch exercises, facilitator notes, support level
- Numbered exercise directories (`00-*` = primary build, `01-*`+ = optional/stretch)
- Each exercise has `prompt.md` + sample data files (`.csv`, `.json`, `.md`)

## Key Conventions

**Exercise numbering:** `00-*` directories are the primary build for the 45-minute individual session. Higher numbers are stretch/follow-up. The GROUP exercise is the opening 60-minute guided build.

**Sample data design:** All data is fictional but uses realistic Ripple context — real team names, plausible business topics (RLUSD, FCA licensing, GTreasury integration, Hidden Road acquisition). No real PII or sensitive financials.

**Prompt structure:** Every `prompt.md` follows the pattern: context (who am I, what's my challenge) → structured output spec → stretch goals. Prompts are designed to be paste-ready — participants upload sample data files and paste the prompt directly into Claude Cowork.

**Connector fallback pattern:** Exercises assume MCP connectors (Gmail, Calendar, Slack, Google Drive) are pre-configured. Sample data files serve as the fallback when connectors aren't available. The workflow should be identical regardless of data source.

**README format:** Each README includes survey response, session build (primary + optional), and facilitator notes (support level, approach, risks, what to do if they finish early).

## Session Schedule

**Date:** March 10, 2026 | 11:00 AM – 3:00 PM ET
**Location:** Mindspace coworking, Wynwood, Miami (near Arlo Wynwood)
**Post-session:** Company meeting immediately follows in same room. Some execs fly to NYC after. Must end cleanly at 3:00.

| Time | Session | What We Prep |
|------|---------|-------------|
| 11:00-11:15 | Welcome & Orientation | — |
| 11:15-11:30 | Macro Overview — AI Products | — |
| 11:30-12:30 | **Claude Desktop Guided Build** (60 min) | GROUP exercise: "Your Daily Briefing" |
| 12:30-13:00 | Lunch | — |
| 13:00-13:45 | **Mid-day Demos** (45 min) | Participants demo group builds |
| 13:45-14:30 | **Guided Build Time** (45 min) | Individual builds (primary exercises) |
| 14:30-15:00 | **Final Demos** (30 min) | Participants demo individual builds |

**Primary tool:** Claude Cowork with MCP connectors (Gmail, Calendar, Slack, Google Drive)
**Optional advanced track:** Claude Code (for JB and any other power users)
**Facilitators:** Mike + Natalia (trainers), Srahman (Ripple internal support)

## Participant Map

| Initials | Role | Primary Exercise | Complexity | Support Level |
|----------|------|-----------------|------------|---------------|
| EVM | SVP Strategic Initiatives | Virtual Chief of Staff | Medium | Self-directed (AI champion, has experimented) |
| JB | CFO | Team Update Aggregator (Finance) | Hard | Self-directed (power user, point at Code) |
| KH | SVP Marketing & Comms | Contract/PO → Editorial + Voice | Easy-Medium | Needs support (most AI-reluctant, "robotic" concern) |
| MK | SVP People, Places, IT | Weekly Leadership Update | Medium | Self-directed (lone power user, knows what she wants) |
| ML | President | Board Content Generator | Medium-Hard | Needs support (casual, may not have submitted survey) |
| RN | CEO, GTreasury BU | KPI Dashboard | Medium-Hard | Self-directed (team already uses Claude, near-power-user) |
| SA | CLO | Meeting Prep Workflow | Easy | Needs support (skeptical, "doesn't see a need — don't push") |

### Facilitator Assignments (45-min individual build)
- **Natalia** floats between ML, KH, and SA (needs more hands-on support)
- **Srahman** supports RN (knows internal systems and connector status)
- **Mike** covers the room, leads demos, checks in on everyone
- **JB** gets pointed at Code and let loose
- **MK and EVM** move quickly with light check-ins

## Connector & Data Status

MCP connectors (Gmail, Calendar, Slack, Google Drive) are pre-configured by IT for all participants. The group exercise uses dummy data for safety; individual builds can use real connected data.

| Participant | Connector Notes |
|------------|----------------|
| RN | **Salesforce:** No official connector — working API workaround. **Tableau:** Working. **Fallback:** CSV in Google Drive pre-session. |
| SA | Some execs paused at calendar edit/delete permissions. Srahman addressed internally — handle briefly if it resurfaces. |
| All others | Standard connectors (Gmail, Calendar, Slack, Drive) should work. |

## Session Risks

1. **Permissions anxiety** — Execs paused at calendar edit/delete permissions during setup. Srahman handled it but it could resurface. Brief response, don't let it derail.
2. **KH's AI-writing skepticism** — Most reluctant participant. Tone/voice exercise designed specifically for this. Have before/after examples ready.
3. **ML's survey gap** — May not have provided input ("not big on forms"). Board prep aligns with Srahman's relay, but be ready to adapt.
4. **Salesforce connector for RN** — No official connector. Tableau is backup, CSV is fallback. Fallback must be seamless.
5. **Tight room** — Conference room at Mindspace coworking. Physical proximity fine for support but may feel cramped.
6. **Hard stop at 3:00** — Company meeting immediately follows. Session must end cleanly.

## Dominant Theme: "Synthesize My Chaos"

5 of 7 survey respondents expressed the same core need: synthesizing information across multiple sources (email, Slack, calendar, documents) into actionable output. This is the through-line for the group exercise and most individual builds.

## Content Guidelines

- Frame exercises around **synthesis across sources**, not drafting or summarization
- Avoid "draft a first version" framing — participants already know AI can draft text. Srahman says that's underwhelming.
- Every exercise should produce a visible "wow" moment within 10-15 minutes, with refinement as stretch
- Include iterative refinement steps — the first output is a starting point, not the final product
- Respect participant attitudes: SA is skeptical (don't push), KH worries AI sounds robotic (show voice training), JB is a power user (point him at Code)
- For Medium-Hard and Hard builds: prompts should be pre-staged and paste-ready, sample data small enough to upload quickly
- All sample data uses realistic Ripple context (RLUSD, FCA, GTreasury, Hidden Road, etc.) but zero real PII or sensitive financials

## Ripple Business Context (for realistic sample data)

- **Acquisitions (2025):** Hidden Road (prime brokerage), GTreasury ($1B — treasury management SaaS), Rail (B2B payments), Palisade (crypto infrastructure)
- **Products:** Payments (cross-border), Custody, RLUSD (stablecoin, $500M+ market cap), Prime (via Hidden Road), Treasury (via GTreasury)
- **Key regulatory milestones:** UK FCA license (with conditions), Luxembourg CSSF (clean), Dubai DFSA, Singapore MAS, 40+ jurisdictions
- **SEC case:** Fully resolved and closed — historic outcome for Ripple
- **Leadership:** BG (CEO), ML (President), JB (CFO), SA (CLO), EVM (SVP Strategy), KH (SVP Marketing), MK (SVP People/IT), RN (CEO GTreasury BU)
