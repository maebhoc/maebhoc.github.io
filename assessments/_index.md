# Assessment Pages — Working Index

State of play for the mbooth.dev assessment services pages.
Use this to hand off to a new agent or resume a session.

---

## What we're building

Four 2-week assessment services for mbooth.dev. Each is a standalone engagement with optional follow-on work (deeper dives, or helping implement what the assessment surfaces). The pitch: get in quickly, get a sense, produce a plan within 2 weeks.

The assessments cover HOW things are built, not WHAT to build. Signals of weak communication, alignment, and feedback mechanisms are in scope as diagnostic findings — but product strategy is not.

All four follow the same structural pattern on the website: what we assess (named dimensions), how it works (2-week shape), what you get (deliverables).

---

## Files in this folder

| File | What it is |
|------|------------|
| `engineering-effectiveness.md` | Draft website copy — Assessment 1. User is currently editing. |
| `_dimension-reference.md` | Working doc: the "why" behind each Engineering Effectiveness dimension. Use to sense-check website copy framing. Not a page. |
| `_index.md` | This file. |

When HTML pages are ready to build, they go in the main site as child pages (e.g. `/assessments/engineering-effectiveness.html`).

---

## Assessment 1 — Engineering Effectiveness

**Status:** Draft written (`engineering-effectiveness.md`), user is editing.

**Five dimensions:**
1. Legibility — can the org see itself? Service ownership, catalogue, contact points, who owns what
2. Flow health — deployment frequency, lead time, change failure rate, MTTR
3. Stack coherence — can tooling be applied consistently, or is it patchwork? (Note: not primarily an AI story — about fragmented knowledge, governance, and cognitive load)
4. Absorption capacity — is the org structured for continuous delivery and learning, or in permanent project mode? Includes whether teams have mechanisms to receive strategic context and surface feedback upward.
5. Toolchain integration — are the key systems connected, or siloed?

**Methodology decisions:**
- Data discovery is time-boxed and breadth-first, not exhaustive. Estimate coverage %, find outliers, repeat until the picture is clear.
- The difficulty in finding metrics is itself a maturity signal.
- Confidence levels are attached to each dimension score based on data quality.
- Source material: `interview-prep-ai-sdlc.md` (5-layer measurement stack, company walkthroughs, proxy methods). Spreadsheet + diagnostic report HTML also exist in `WORK/assessments/Engineering Effectiveness/`.

**Deliverables:**
1. Engineering effectiveness scorecard — organisation-wide and per team
2. Measurement source map — what was assessed, where metrics came from, confidence level per signal
3. Measurement maturity rating (0–5 scale)
4. Prioritised recommendations
5. 90-day plan skeleton

---

## Assessment 2 — Operating Model & Org Design

**Status:** Dimensions agreed in conversation. Not yet written to file.

**Five dimensions:**
1. Operating model clarity — is there a documented model, and does how the org actually works match it?
2. Team topology — how teams are set up, what types they are, how they interact and hand off work
3. Decision rights — who decides what, at what level, and where are the bottlenecks and escalations?
4. Workforce composition — skills profile, role balance, gaps, consolidation opportunities
5. Strategic alignment — does the structure support the strategy? Includes: do the mechanisms exist for strategic context to reach execution level, and for execution-level signals to travel back up?

**Methodology decisions:**
- Primarily artefact and interview driven (org charts, op model docs, strategy papers, leadership conversations), not metrics driven.
- The gap between the stated operating model and how things actually work is usually where the most important findings are. Artefacts tell you the intended design; interviews tell you the lived one.
- The equivalent of "friction in finding metrics": if there's no written op model, that's a signal. If nobody can explain decision rights consistently, that's a signal.
- This is the primary home for communication and alignment diagnostic signals: do engineers know why they're building what they're building, does strategy reach execution, does customer feedback reach teams?
- A transcript of the specific engagement that prompted this work exists. It should be used as a sanity check AFTER the bare bones are built, not as the starting point, to avoid the output looking fabricated for that engagement.

---

## Assessment 3 — Technical Direction

**Status:** Named only. Not yet discussed in detail.

**Working description:** Where is the technology going? Current state architecture, technical debt, build vs buy decisions, platform direction. Primarily technical interviews and artefact review (architecture docs, ADRs, roadmaps).

**Primary buyer:** CTO, VP Engineering.

---

## Assessment 4 — AI Readiness

**Status:** Named only. Not yet discussed in detail.

**Working description:** How ready is the organisation to adopt AI across the SDLC? Tooling, culture, safety, governance, skill gaps. Timely and differentiating — most organisations are asking this question right now.

**Primary buyer:** CTO, VP Engineering, sometimes CISO.

---

## Cross-cutting decisions

**Two-week structure (applies to all four):**
- Days 1–2: Kick-off + discovery (mapping what exists, where data/artefacts live, coverage)
- Days 3–7: Data/artefact collection + structured interviews
- Days 8–10: Analysis and scoring
- Days 11–14: Report, recommendations, readout

**Breadth-first discovery (applies to all four):**
The discovery phase is time-boxed, not exhaustive. The goal is characterisation, not completeness. Friction in the discovery process is part of the diagnosis.

**What's out of scope:**
"Are we building the right thing?" — product strategy, customer research, product-market fit. Diagnostic signals that comms and alignment are broken are in scope. Fixing the product strategy is not.

**Website approach:**
Drafts in markdown in this folder. Convert to HTML child pages when content is settled. No static site generator — plain HTML site. Markdown is the editing layer.
