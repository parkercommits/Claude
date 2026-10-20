---
name: pmm-discover
description: >
  This skill should be used when the user wants to "run discovery on [company]",
  "research [company] for me", "set up the PMM context for [company]",
  "I'm targeting [company] — do the discovery", "start the PMM framework for [company]",
  "do audience analysis for [company]", or any request to begin product marketing
  research where no prior context document exists. Executes the PMA Discover phase:
  audience analysis, competitive intelligence, JTBD canvas, market sizing, and business case.
metadata:
  version: "0.1.0"
  author: "Parker Lyons"
---

# PMM Discover Skill

## Trigger conditions
Invoke this skill when the user says any of the following (or close variants):
- "Run discovery on [company]"
- "Research [company] for me"
- "Set up the PMM context for [company]"
- "I'm targeting [company] — do the discovery"
- "Start the PMM framework for [company]"
- "Do audience analysis for [company]"
- Any request to begin product marketing work on a company where no prior context document exists

---

## Framework & philosophy

This skill executes the **Discover phase of the PMA Product Marketing Framework** — the foundation for all subsequent PMM work.

**The goal of Discover is to replace assumptions with evidence.** A strong PMM uses this phase to answer three core questions:
1. Who is the customer and what problem do they actually care about?
2. What is happening in the market and competitive landscape?
3. Is there a commercially viable opportunity worth pursuing?

If Discover is done well, the rest of the framework gets faster, sharper, and more credible. If it's rushed, weak assumptions infect positioning, launches, and growth plans later.

**Pro tip baked into this skill:** Start with the strategic decision that needs to be made, then work backward to the research required. That keeps Discover lean, credible, and useful — not a research dump.

**Audience-first lens (MKT1):** When applying any template or framework, always ask "who is this for and what's their problem?" before "what does the product do." This makes the PMA methodology more effective.

---

## Engagement modes

Before executing, confirm which mode applies:

- **Build mode** — Working at or for this company. Outputs are real deliverables. Steps 1–5 all apply, including the internal audit (Step 3). Flag where internal data is needed that can't be gathered from desktop research.
- **Job hunt mode** — Targeting this company as a prospective employer. All outputs based on public information only. Step 3 (internal audit) is skipped or replaced with a "what I'd want to audit" checklist. Add ⚠️ **Job Hunt Mode** to the top of every output — all findings are hypotheses to validate in interviews.

---

## The five-step Discover process

### Step 1 — Align on the business question and hypotheses

Before any research begins, define what you're trying to learn. Without this, teams gather lots of data but don't produce decisions.

**Confirm the business context. Ask:**
- Is this a new product or feature launch?
- A repositioning effort?
- Expansion into a new segment or market?
- Response to flat growth or competitive pressure?

**Document current assumptions** from product, sales, leadership, and customer-facing teams. Then turn them into testable hypotheses.

Examples of well-formed hypotheses:
- "Mid-market IT buyers see integration complexity as the main adoption blocker"
- "Buyers choose competitors because our ROI story is unclear, not because of missing functionality"
- "Segment X has higher urgency and willingness to pay than Segment Y"

**Templates for this step:**
- Research brief (objective, business question, target audience, methodology, timeline, stakeholders)
- Hypothesis log (assumption / evidence for-against / how it will be tested)
- Stakeholder interview template (current beliefs, pain points, open questions, success criteria)

**Key output:** A research plan with business questions, hypotheses, target audiences, methods, and timeline. In job hunt mode: a list of hypotheses about the company's market position to test in interviews.

---

### Step 2 — Conduct customer and market research

This is the heart of Discover. Combine qualitative and quantitative research to get both depth and pattern recognition.

**Qualitative research** is best for: understanding motivations, exploring pain points, uncovering language and nuance, shaping hypotheses.
**Quantitative research** is best for: validating patterns at scale, sizing opportunities, prioritizing segments, giving leadership confidence.
Start qualitative, then use quantitative to validate and prioritize.

---

#### 2A. Customer research

Goal: understand buyers, users, decision criteria, pain points, language, triggers, and objections.

**Core methods (build mode):**
- Customer interviews
- Prospect interviews
- Win-loss interviews
- Customer advisory conversations
- Sales call reviews
- Support ticket analysis
- Product usage analysis with PM/product ops

**Core methods (job hunt / desktop research mode):**
- G2, Capterra, Reddit, LinkedIn reviews and comments
- Case study analysis — note titles, company types, pain points described
- Homepage and pricing copy — what language does the company use?
- Job postings for the company — reveals what problems they're solving
- Community discussions (Slack groups, forums, LinkedIn posts about the category)

**What to learn:**
- Main jobs-to-be-done
- Pain points and unmet needs
- Buying triggers
- Evaluation criteria
- Decision-making process and stakeholders
- Why customers choose you / delay / choose competitors
- Language customers naturally use to describe the problem

**Templates:**
- Customer interview guide (background, problem exploration, buying journey, alternatives, language capture)
- Win-loss interview guide (trigger, shortlist, selection criteria, perceived pros/cons, decision drivers)
- Buyer/user persona template (role, goals, pains, motivations, objections, buying influence)
- Voice-of-customer capture sheet
- Interview synthesis template

---

#### 2B. Market research

Goal: assess whether the opportunity is real beyond a few anecdotes.

**Core methods:**
- TAM/SAM/SOM sizing
- Industry trend analysis
- Category research (maturity, dynamics)
- Segment analysis
- Survey research
- Analyst and secondary research review
- Internal historical performance review (build mode)

**What to learn:**
- Market trends shaping demand
- Category maturity
- Segment attractiveness
- Buying behavior shifts
- Macro risks and tailwinds
- Where the company can differentiate commercially

**Templates:**
- Market landscape template (trends, segment dynamics, demand drivers, barriers, opportunity implications)
- Segment attractiveness scorecard
- Market sizing template (TAM/SAM/SOM with sources)
- Trend analysis summary
- Opportunity assessment template

---

#### 2C. Competitive intelligence

Non-negotiable in Discover. A PMM must know not just who competitors are, but how they win.

**Core methods:**
- Competitor website and messaging analysis
- Demo and trial reviews (sign up if possible)
- Review site analysis (G2, Capterra — especially negative reviews)
- Sales feedback collection (build mode)
- Win-loss data mining (build mode)
- Pricing and packaging review
- Battlecard inputs from the field (build mode)

**What to learn:**
- Competitor positioning and claimed differentiation
- Feature strengths/weaknesses
- Pricing posture
- Ideal customer profile focus
- Common reasons they win or lose

**Competitive Intelligence Matrix** — populate for 3–5 competitors (always include "status quo / do nothing / spreadsheets" as a row):

| Activity | [Company] | Competitor 1 | Competitor 2 | Competitor 3 |
|---|---|---|---|---|
| Target customers (segments/verticals) | | | | |
| Estimated customer count | | | | |
| Notable/referenceable customers | | | | |
| Geographies | | | | |
| Positive review themes | | | | |
| Negative review / complaint themes | | | | |
| Core product suite | | | | |
| Defining features | | | | |
| Value drivers / claimed outcomes | | | | |
| Pricing model and tiers | | | | |
| Perceived strengths | | | | |
| Perceived weaknesses | | | | |
| How they solve the audience's problem | | | | |

**Templates:**
- Competitor profile template (target audience, positioning, messaging, strengths, weaknesses, pricing clues)
- Messaging teardown template
- SWOT or alternatives analysis (PMA Competitor SWOT: coda.io/@product-marketing-alliance-pma)
- PMA Competitor Intel Checklist: coda.io/@product-marketing-alliance-pma/pma-competitor-intel-checklist

---

#### 2D. Jobs-to-Be-Done Canvas

Using the **PMA JTBD framework** — answer all 8 questions for the primary audience segment:

| # | Question | Answer |
|---|---|---|
| 1 | What's the job-to-be-done? (Based on customer evidence, not internal assumptions) | |
| 2 | Who's carrying out the job? (Note if user ≠ buyer in B2B) | |
| 3 | Why do they want to do this job? (Pains, gains, motivation) | |
| 4 | When and where do they do the job? (Frequency, context) | |
| 5 | How does the job get done? (Process, barriers) | |
| 6 | How does the customer feel? (Desired emotions after completion) | |
| 7 | What other jobs do they use the product for? (Secondary jobs) | |
| 8 | What outcomes are essential? (Must-haves vs. nice-to-haves) | |

Source: PMA Jobs-to-Be-Done Canvas — coda.io/@product-marketing-alliance-pma/pma-jobs-to-be-done-canvas

---

### Step 3 — Audit what already exists internally

*(Build mode only — skip for job hunt mode, replace with "what I'd want to audit" checklist)*

A lot of Discover work is not net-new research. It's connecting what the business already knows but hasn't synthesized.

**Review:**
- Existing personas
- Current messaging and positioning
- Prior launch retrospectives
- CRM and pipeline trends
- Lost deal reasons
- Product adoption data
- NPS, CSAT, support themes
- Sales call recordings
- Existing enablement materials and website copy

**Best-practice questions to ask:**
- What assumptions are already baked into our messaging?
- What evidence supports them?
- Where are we seeing friction in the funnel?
- Are there discrepancies between what marketing says and what customers care about?

**Templates:**
- Messaging audit template (current claims, target audience fit, proof points, inconsistencies, gaps)
- Funnel friction audit
- Asset inventory worksheet
- Internal insight synthesis doc

**Key output:** A gap analysis showing — what the company believes / what the evidence says / what still needs validation.

**For job hunt mode:** Instead of the audit, document what you *would* want to audit. Frame it as: "If I were joining this team, the first things I'd want to review are X, Y, Z — here's what I'd expect to find and why." This becomes a strong interview talking point.

---

### Step 4 — Synthesize findings into strategic insight

This is where PMMs create value. Discover is not about handing over a pile of research — it's about translating research into decisions.

**Synthesis themes to address:**
- Core customer problem
- Most promising segments
- Buyer motivations and blockers
- Market opportunity
- Competitive whitespace
- Messaging gaps
- Commercial risks and opportunities

**The "so what" filter** — every major insight must answer one of these:
- So what does this mean?
- Why does it matter commercially?
- What should we do differently because of it?

**Discovery Summary format:**

*The audience in one sentence:*
"We are building for [audience type] who struggle with [core problem] and currently solve it by [alternative]."

*What makes this market interesting:*
2–3 observations about the opportunity (size, growth, timing, underserved need).

*Competitive whitespace:*
Where competitors are weak or absent relative to this audience's most important needs.

*Messaging gaps:*
Where current messaging doesn't match what customers actually care about.

*Open questions:*
3–5 things that couldn't be confirmed from available research. Flag these explicitly.

**Templates:**
- Insight synthesis template (key findings, evidence, implications, recommended action)
- Opportunity canvas
- Segment prioritization framework
- Jobs-to-be-done summary
- Executive readout deck

**Key output:** A concise insight narrative that helps leadership and cross-functional teams align on the opportunity.

---

### Step 5 — Build the business case and recommendation

The final step of Discover is not "here's what we learned." It's "here's what we should do next."

**The recommendation must cover:**
- Which customer/segment to prioritize
- Which problem/opportunity is worth pursuing
- Why it matters now
- Why your company can win
- Risks, unknowns, and dependencies
- What moves into Strategize next

**Business case structure:**
- Opportunity (what's the problem/market)
- Target segment (who specifically)
- Customer problem (what they struggle with)
- Strategic fit (why this company is positioned to win)
- Market potential (size, growth, timing)
- Competitive advantage (why you, not them)
- Risks (what could go wrong)
- Recommendation (go / no-go / prioritization)

**Templates:**
- PMA Business Case Template: coda.io/@product-marketing-alliance-pma
- Go/no-go recommendation memo
- Opportunity prioritization matrix
- Executive summary deck

**Key output:** A clear go-forward recommendation with evidence and next-step decisions.

---

### Step 6 — Create the Context Document

Compile all outputs into a single document titled:
`[Company] — PMM Context | Discover Phase`

**If Google Drive is connected:**
Create a Google Doc with this title. Structure with clear headers per section. Share the link.

**If not connected:**
Save as `[company-slug]-pmm-context.md` and present via file card.

This document is read by all downstream skills before they execute. If a downstream skill is invoked without it, prompt the user to run Discover first.

---

## Week-by-week operating model

For a standard Discover engagement:

**Week 1 — Frame**
- Align stakeholders on business question
- Document assumptions
- Write hypotheses
- Finalize research plan

**Weeks 2–4 — Gather**
- Interview customers/prospects
- Run win-loss research
- Review internal data (build mode)
- Audit competitors
- Assess market and segments

**Weeks 4–5 — Synthesize**
- Cluster findings, identify patterns
- Distinguish signal from noise
- Develop key insights and implications

**Weeks 5–6 — Recommend**
- Build business case
- Prioritize opportunity
- Align leadership
- Hand off into Strategize

*For job hunt mode or quick scans: compress to 1–2 days of desktop research with clear flags on what's unverified.*

---

## What good Discover looks like

A strong Discover phase is:
- Evidence-led rather than opinion-led
- Cross-functional but PMM-owned from a commercial/marketability lens
- Focused on decisions, not just research activity
- Balanced across customer, market, competitor, and internal inputs
- Synthesized into action, not left as raw notes

A weak Discover phase looks like:
- Too much reliance on internal opinions
- No direct customer conversations
- Feature-level thinking instead of market/problem thinking
- Competitive analysis that is shallow or outdated
- Outputs that describe findings but don't recommend action

---

## Full template toolkit

| Template | Key fields |
|---|---|
| Research brief | Objective, business question, target audience, methodology, timeline, stakeholders |
| Hypothesis log | Assumption, evidence for/against, how it will be tested |
| Stakeholder interview template | Current beliefs, pain points, open questions, success criteria |
| Customer interview guide | Background, problem exploration, buying journey, alternatives, language capture |
| Win-loss interview guide | Trigger, shortlist, selection criteria, perceived pros/cons, decision drivers |
| Persona template | Role, goals, pains, motivations, objections, buying influence |
| Market analysis template | Market trends, segment dynamics, demand drivers, barriers, opportunity implications |
| Competitor profile template | Target audience, positioning, messaging, strengths, weaknesses, pricing clues |
| Messaging audit template | Current claims, audience fit, proof points, inconsistencies, gaps |
| Insight synthesis template | Key findings, evidence, implications, recommended action |
| Business case template | Opportunity, target segment, customer problem, strategic fit, market potential, competitive advantage, risks, recommendation |

PMA Coda template library: coda.io/@product-marketing-alliance-pma

---

## What NOT to do

- Do not skip the hypothesis step — without it, research becomes a data dump
- Do not skip the internal audit in build mode — it often contains half the insights you need
- Do not present findings without a "so what" — every insight needs a commercial implication
- Do not skip Behavior/Buying information in persona research — it is the most commonly omitted and most useful for GTM
- Do not map competitors feature-by-feature only — always include how they solve the audience's problem

---

## Downstream skills this feeds into

The Context Document is read by:
- **PMM Define** — uses JTBD canvas, persona profiles, and competitive whitespace
- **PMM Strategize** — uses competitive matrix, market sizing, and business case
- **PMM Get Set** — uses competitive matrix and persona profiles for sales enablement
- **PMM Grow** — uses JTBD outcomes as post-launch success criteria

---

## Reference frameworks

**Primary (structural backbone):**
- PMA Product Marketing Framework — Discover phase
- PMA Jobs-to-Be-Done Canvas
- PMA Competitor Intel Checklist
- PMA B2B Persona Questions
- PMA Market Sizing Template
- PMA Business Case Template
- PMM-GPT best practice guidance (PMA, 2026)

**Secondary (philosophical lens):**
- MKT1 / Emily Kramer — audience-focused product marketing
- SVPG / Martina Lauchengco (Loved) — PMM's role in product/market fit from the market side
