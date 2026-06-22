# Dimension Reference — All Assessments

Pooled reference for diagnostic dimensions across all four assessments. Working document. Not a page.

---

## Overview table

| Dimension | Engineering Effectiveness | Operating Model & Org Design | Technical Direction | AI Readiness |
|-----------|--------------------------|------------------------------|--------------------|-----------| 
| Organisational legibility | ✓ Service catalogue, contact points, knowledge concentration | ✓ Does the org chart reflect how work actually gets done? Who to go to for decisions, not just who owns a system | | |
| Delivery flow | ✓ DORA scoring — deployment frequency, lead time, change failure rate, MTTR | | | |
| Technology estate coherence | ✓ Current state — what is fragmentation costing in cognitive load and friction? | ✓ Converge vs align decision — what structure does the level of fragmentation require? | ✓ Target state strategy — converge, align, or deliberate separation? Path and timeline. | |
| Change absorption | ✓ Delivery mode + human capacity — can the org act on findings? | ✓ Is the operating model designed for learning and adaptation, not just output? | | |
| Toolchain integration | ✓ Are systems connected and feeding measurement? | | ✓ What integration is needed to reach the target measurement model? | ✓ Prerequisite for AI — agents need connected context to work effectively |
| Operating model clarity | | ✓ Stated vs lived model — the gap is the finding | | |
| Team topology | | ✓ Team types, structure, interaction modes, handoffs | | |
| Decision rights | | ✓ Who decides what, at what level — bottlenecks and escalations | | |
| Workforce composition | | ✓ Skills vs strategy match, role balance, consolidation opportunities | | |
| Strategic alignment | | ✓ Does the structure enable the strategy? Communication and feedback mechanisms. | ✓ Does the tech direction support the business strategy? Is technical risk visible upward? | |
| Direction credibility | | | ✓ Is there a target state, clearly articulated, with a believable path to get there? For acquisition-heavy orgs: is there a deliberate position on what to converge, align, or keep separate? | |

---

## Dimension detail

### Organisational legibility

Can the organisation see itself? Covers structural visibility (who owns what, team membership, contact points) and knowledge visibility (who actually understands what, not just who is nominally responsible). These are distinct — a service can have a named owner who doesn't understand it.

**Why it matters:** Without legibility, coordination fails — incidents take longer to resolve, duplication is invisible, onboarding relies on tribal knowledge, compliance is ungovernable.

**Signals of a problem:** MTTR longer than it should be, new joiners find the right person by asking around, the same capability gets built by multiple teams independently, changes to certain areas can only be made by one or two people.

---

### Delivery flow

How work moves from idea to production. DORA metrics are the primary signal: deployment frequency, lead time for changes, change failure rate, MTTR.

**Why it matters:** Delivery performance is the clearest indicator of whether the engineering system is working. Everything else eventually shows up here.

**Signals of a problem:** Releases infrequent or unpredictable, rollbacks common, incidents cluster around deployments, teams accumulate work rather than shipping continuously.

---

### Technology estate coherence

How fragmented is the technology landscape? The number of incompatible stacks, languages, and platforms in play affects cognitive load, standards consistency, the ability to move engineers between areas, and the scope of any platform investment. Fragmentation from organic growth is different from fragmentation from acquisitions — the cause affects the response.

**Why it matters:** Fragmented estates mean fragmented knowledge and inconsistent governance. Every cross-team dependency carries a translation cost.

**Signals of a problem:** Platform investments land in some areas but not others, engineers struggle to work outside their immediate area, standards compliance inconsistent, significant effort maintaining multiple versions of the same capability.

---

### Change absorption

Is the organisation — structurally and in terms of the people in it — capable of learning and improving? Covers structural readiness (delivery mode, slack, learning cycles) and human readiness (cognitive load, flow state, capacity to absorb new approaches). Also covers whether strategic context reaches teams and whether there are mechanisms for execution-level signal to travel upward.

**Why it matters:** Any assessment produces recommendations. Whether they land depends on whether the org can act on them. The org may look structurally ready while the people in it are running empty — both need to be true.

**Signals of a problem:** No protected time outside sprint delivery, retros cancelled when things get busy, previous initiatives stalled, same problems recur, engineers report high context-switching.

---

### Toolchain integration

Are the key systems — Git, Jira, CI/CD, observability, incident management — connected and feeding into measurement mechanics? Connectivity and instrumentation are distinct: systems can be in use alongside each other without surfacing useful signals.

**Why it matters:** When tools are siloed or uninstrumented, humans fill the gaps. This is also what makes data discovery hard during an assessment — not that tooling is absent, but that it is not set up to surface anything useful.

**Signals of a problem:** Managers spend significant time aggregating status manually, incident root cause requires correlation across disconnected systems, DORA metrics can only be approximated, data exists but extracting it requires bespoke effort each time.

---

### Operating model clarity

Is there a documented operating model, and does how the organisation actually works match it? The gap between stated and lived model is usually where the most important findings are.

**Why it matters:** Artefacts tell you the intended design. Interviews tell you the lived one. An undocumented model is fragile — it exists only in people's heads.

**Signals of a problem:** Leadership describes decision-making differently to each other, documented processes don't match how work flows, teams operate differently depending on which manager they have.

---

### Team topology

How are teams structured, what types are they, and how do they interact and hand off work?

**Why it matters:** Team structure determines cognitive load, flow of work, and the cost of dependencies. Teams structured around technology rather than outcomes create handoffs that slow delivery.

**Signals of a problem:** Teams frequently blocked waiting on others, platform teams overwhelmed with one-off requests, unclear ownership at team boundaries, team size too large for effective communication.

---

### Decision rights

Who decides what, at what level, and where are the bottlenecks and escalations?

**Why it matters:** Unclear decision rights create delays and inconsistency. The right level for a decision depends on who has the context and who lives with the consequences — this rarely matches what people say it is.

**Signals of a problem:** Decisions that should be quick take weeks, same decisions relitigated repeatedly, engineering teams feel they lack autonomy, senior leaders feel things happen without their knowledge.

---

### Workforce composition

Does the skills profile match the strategic direction? Covers role balance, skill gaps, onshore/offshore split, contractor vs permanent ratio, and consolidation opportunities.

**Why it matters:** A strategy that requires capabilities the org doesn't have is not a strategy. Workforce composition also affects resilience — key person dependency and over-reliance on contractors for core capability are risks.

**Signals of a problem:** Skills required for the stated strategy are absent, key roles filled entirely by contractors, significant knowledge concentration in individuals, offshore ratio misaligned with coordination requirements.

---

### Strategic alignment

Does the organisation's structure and operating model support where it is trying to go? Includes whether strategic context reaches execution level and whether execution-level signal travels back up to inform strategy.

**Why it matters:** Structure that made sense for a previous strategy becomes friction for a new one. Whether engineers know why they're building what they're building is a signal of alignment health.

**Signals of a problem:** Engineers unable to explain how their work connects to company goals, strategy documents that don't reflect what is actually being built, no forums for execution-level insight to reach decision-makers.

---

### Direction credibility

Is there a target state for the technology estate, is it clearly articulated, and is the path from current state to target believable? Having a strategy document is not the same as having a credible direction.

**Why it matters:** Without a credible direction, technology investments are made in isolation. Teams optimise locally. Technical debt accumulates without a framework for deciding what to address first. The estate drifts rather than evolves deliberately.

**Signals of a problem:** The tech strategy exists as a document nobody references, teams make architectural decisions independently without a shared framework, no clear prioritisation of what technical debt to address and why, roadmaps don't connect to a stated technical direction.

**Acquisition scenario:** When a company has grown through multiple acquisitions, this dimension carries extra weight. The question is whether there is a deliberate position on what to converge, what to align at the interface layer, and what to keep intentionally separate. These are three genuinely different responses to the same problem, and choosing between them requires explicit intent. Defaulting to "we'll integrate everything eventually" without deciding what that means in practice is itself a finding.
