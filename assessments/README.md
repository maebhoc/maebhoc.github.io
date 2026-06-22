# Assessments — How This Folder Works

This folder contains the content and working materials for the services on mbooth.dev. The site has two sections: a set of 2-week diagnostic assessments, and a separate AI-enabled SDLC engagement for software companies.

---

## The four content layers (per assessment)

| Layer | File pattern | Purpose | Audience |
|-------|-------------|---------|----------|
| Website outline | `[name].md` | Short pitch — what the assessment is, what you get. Converts to an HTML child page on mbooth.dev. | Prospective clients visiting the site |
| Dimension reference | `_dimensions.md` (pooled) | Why each lens matters. Working doc — not a page. | Internal reference when writing or reviewing website copy |
| Engagement guide | `[name]-engagement.md` | How the engagement actually runs — day by day, sponsor check-in guidance. Use in proposals and scoping conversations. | Prospects who have expressed interest; personal reference during engagements |
| Data map | `[name]-data-map.md` | What data and artefacts are needed, where they typically live, how to find equivalents. | Personal reference during the discovery phase |

---

## Section 1: Assessments (2-week sprints)

| Assessment | Status |
|-----------|--------|
| Engineering Effectiveness | Website outline drafted. HTML page built. Dimension reference in `_dimensions.md`. Engagement guide written. |
| Operating Model & Org Design | Website outline drafted. HTML page built. Dimensions in `_dimensions.md`. |
| Technical Direction | Website outline drafted. HTML page built. |
| AI Tooling | Website outline drafted. HTML page built. |
| Engineering People & Culture | Website outline drafted. HTML page built. |

---

## Section 2: AI-Enabled SDLC

A separate, bespoke engagement for software product companies. Not a 2-week sprint — scoped based on an initial discovery. Covers the full product development lifecycle from inception to live and beyond: how the right work is chosen, how to say no, build practices, testing strategy, review processes, skills profile across all stages. The AI lens applied to the whole system, not just tooling.

Not yet written. Design to follow after the five assessments are complete.

---

## File inventory

| File | Type | Assessment | Status |
|------|------|-----------|--------|
| `engineering-effectiveness.md` | Website outline | Engineering Effectiveness | Drafted |
| `engineering-effectiveness.html` | HTML page | Engineering Effectiveness | Built |
| `engineering-effectiveness-engagement.md` | Engagement guide | Engineering Effectiveness | Written |
| `operating-model.md` | Website outline | Operating Model | Drafted |
| `operating-model.html` | HTML page | Operating Model | Built |
| `technical-direction.md` | Website outline | Technical Direction | Drafted |
| `technical-direction.html` | HTML page | Technical Direction | Built |
| `ai-tooling.md` | Website outline | AI Tooling | Drafted |
| `ai-tooling.html` | HTML page | AI Tooling | Built |
| `engineering-people-culture.md` | Website outline | Engineering People & Culture | Drafted |
| `engineering-people-culture.html` | HTML page | Engineering People & Culture | Built |
| `_dimensions.md` | Dimension reference | All assessments (pooled) | Written — covers Eng Effectiveness, Operating Model, Technical Direction |
| `_index.md` | Session state / agent handoff | All | Current |
| `README.md` | This file | All | Current |

---

## Converting to HTML

When a website outline is ready, it becomes an HTML child page at `/assessments/[name].html` on mbooth.dev. The site is plain HTML — no static site generator. The markdown files are the editing layer; HTML is built from them when the content is settled.

---

## Cross-cutting decisions

All five assessments follow the same structural pattern on the website: what we assess (named dimensions) → how it works (short) → what you get (deliverables).

All are scoped as 2-week engagements. The pitch is: get in quickly, get a sense, produce a plan. Follow-on work — deeper dives, implementation support, the AI-enabled SDLC engagement — is a separate conversation.

The assessments cover HOW things are built and HOW the org is structured, not WHAT to build. Signals of weak communication and alignment are in scope as diagnostic findings. Product strategy is not.
