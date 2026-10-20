---
name: pmm-discover
description: >
  This skill should be used when the user wants to "run discovery on [company]",
  "research [company] for me", "set up the PMM context for [company]",
  "I'm targeting [company] — do the discovery", "start the PMM framework for [company]",
  "do audience analysis for [company]", or any request to begin product marketing
  research where no prior context document exists. Executes the PMA Discover phase:
  audience analysis and ICP prioritization, competitive and ecosystem mapping,
  product analysis, JTBD canvas, TAM mapping, and business case.
metadata:
  version: "0.2.0"
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

**Three research pillars (MKT1):** Discover must cover all three, not just the first two:
1. **Audience** — TAM, ICPs at company and persona level, and how the audience behaves
2. **Market, ecosystem & competitors** — alternatives, complements, and the voices that shape buying decisions
3. **Product** — the primary problem solved today, and features → use cases → benefits

**Research is not positioning.** Discover goes deep and gathers evidence; Define condenses it into a positioning statement. Don't write positioning here — but do hand Define the inputs it needs (ICP tiers, the primary problem, candidate comparators).

**Research is ongoing.** The Context Document is a living file, not a one-time report. Audiences, markets, and products shift; date what you verify so later phases know what may be stale.

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

#### Research reliability rules (apply to all desktop and AI-assisted research)

Errors compound: one bad data point flows into the matrix, the insights, and the business case. Before and during research:

- **Fix canonical URLs first.** List the exact homepage, pricing, careers, and review-site URLs for each company before researching. Never guess a URL from a company name.
- **Define attributes up front.** Give every matrix row a concrete definition before filling it, so every company is assessed the same way.
- **Blank and flag, don't guess.** If a data point can't be found, leave it blank and mark it ❓. For yes/no fields, "unknown" is a valid third answer — never default to "no."
- **Distrust suspiciously round numbers** (customer counts, revenue, headcount). They are often invented.
- **Cite a source for every data point** — URL plus date accessed — so findings can be rechecked.
- **Spot-check before scaling.** When researching more than ~5 companies, verify the first few rows and every outlier by hand before completing the rest.
- **Watch for empty pages.** Pages that render with JavaScript can look blank to fetch tools; if a page returns little content, say so rather than concluding the information doesn't exist.
- **Drop the hard data point.** If one attribute is far harder to collect than the rest, cut it rather than building fragile workarounds.

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
- Main jobs-to-be-done — including goals the audience has independent of any product, and adjacent workflows beyond the one the product replaces
- Pain points and unmet needs
- Buying triggers
- Evaluation criteria
- Decision-making process and stakeholders, including buyer roles (economic buyer, champion, user, blocker)
- Why customers choose you / delay / choose competitors
- Language customers naturally use to describe the problem

**Audience behavior (MKT1 — do not skip; this is what channel strategy is built on later):**
- Where they get information (publications, newsletters, podcasts, analysts, search, LLMs)
- Communities and peer networks they're active in, online and in person
- Full tool stack — SaaS products, spreadsheets, and templates they rely on (these are also potential partners)
- Content and format preferences (long-form, video, templates, events, peer recommendations)
- Who they trust and listen to (influencers, advisors, service providers)

**ICP composition** — define each ICP at two levels:
- *Company:* industry, size, stage, geography, tech stack
- *Persona:* role, buyer role, jobs-to-be-done, pain points, behaviors

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
- TAM mapping (see below) — preferred over TAM/SAM/SOM
- ICP prioritization (see below)
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

**TAM mapping (MKT1 coverage approach):** Rather than an analyst-style TAM/SAM/SOM number, map the total addressable market by company type and role, and mark which segments the company can credibly target **now** versus **later**. This produces a usable targeting map rather than a size estimate. If a top-down market-size figure is needed for the business case, add it as a single sourced number in Step 5 — don't build SAM/SOM layers.

**ICP prioritization — required output.** Tier every ICP identified:

| Tier | Meaning |
|---|---|
| **Core** | Proven ICPs driving most of today's business |
| **Scaling** | Working ICPs you plan to grow into; a small share of business today |
| **Testing** | Emerging ICPs you're experimenting with |
| **Not a priority today** | Considered and explicitly deprioritized, so the team knows it was a choice |

Name **one primary audience** — go narrow. In job hunt mode, tier from public evidence (case studies, logos, job postings, pricing pages) and mark the tiers as hypotheses.

**Templates:**
- Market landscape template (trends, segment dynamics, demand drivers, barriers, opportunity implications)
- TAM coverage map (company type × role, now vs later)
- ICP tiering table (Core / Scaling / Testing / Not a priority today)
- Segment attractiveness scorecard
- Trend analysis summary
- Opportunity assessment template

---

#### 2C. Competitive and ecosystem intelligence

Non-negotiable in Discover. A PMM must know not just who competitors are, but how they win — and who else in the ecosystem shapes the buyer's decision. Buyers compare you to competitors, to alternatives like spreadsheets and services, and to tools they already use, and they're influenced by analysts, communities, media, and advisors. Competitor-only research misses half the picture.

##### Competitors

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
| Business model | | | | |
| Company size, stage, funding | | | | |
| Estimated customer count | | | | |
| Notable/referenceable customers | | | | |
| Geographies | | | | |
| Positive review themes | | | | |
| Negative review / complaint themes | | | | |
| Core product suite | | | | |
| Defining features | | | | |
| Value drivers / claimed outcomes | | | | |
| Pricing model and tiers | | | | |
| Homepage positioning (who it's for / what it is / why better) | | | | |
| GTM motion / growth engines (sales-led, PLG, partner, community, etc.) | | | | |
| Content types and channels | | | | |
| Perceived strengths | | | | |
| Perceived weaknesses | | | | |
| How they solve the audience's problem | | | | |

Every cell follows the research reliability rules: sourced, dated, or blank and flagged ❓.

##### Complements and frenemies (ecosystem map)

Know your complements like you know your competitors. Map the players who share your audience but don't compete with you:

- **Complements:** integration and technology partners, communities, influencers, affiliates, agencies and consultancies, customers you could co-market with
- **Frenemies:** players between partner and competitor that shape the narrative — analysts, media, regulators, service providers

Discovery prompts: What are the audience's source-of-truth platforms? Who influences their buying decisions? Who do they already pay for adjacent work? Who has data, reputation, or reach the company lacks?

| Player | Type (complement / frenemy) | Category | Size (L/M/S) | Audience overlap | Potential value exchange | Risks or costs |
|---|---|---|---|---|---|---|
| | | | | | | |

Map 5–10 of the most relevant players. Quality over quantity — a few strong partners beat many transactional ones.

**Templates:**
- Competitor profile template (target audience, positioning, messaging, strengths, weaknesses, pricing clues)
- Ecosystem map (complements and frenemies, with audience overlap and value exchange)
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

#### 2E. Product analysis

The third MKT1 pillar. A PMM must know the product well enough to connect it to the audience's problem — without letting product detail lead the research.

**Core methods:**
- Demo or free trial (sign up if possible)
- Product documentation, help center, and API docs
- Changelog and release notes (reveals direction and investment areas)
- Product walkthroughs with PM / product ops (build mode)
- Review-site feature mentions — what customers actually use

**Required outputs:**
- **Primary problem solved today**, in one sentence, in the customer's language — not the roadmap's
- **Features → use cases → benefits map:**

| Feature / capability | Use case it enables | Benefit to the audience | Which ICP it matters to |
|---|---|---|---|
| | | | |

- **How it differs from alternatives** — evidence-based differences only; claimed differentiation goes in the competitor matrix
- **Recent and likely-next investments** (from the changelog and job postings)

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
- ICP tiers and the one primary audience
- Buyer motivations and blockers
- Market opportunity
- Competitive whitespace
- Ecosystem opportunities (complements worth partnering with; frenemies shaping the narrative)
- Marketing advantages — built-in tailwinds such as network effects, ecosystem relationships, or viral/shareable features
- Messaging gaps
- Commercial risks and opportunities

**The "so what" filter** — every major insight must answer one of these:
- So what does this mean?
- Why does it matter commercially?
- What should we do differently because of it?

**Discovery Summary format:**

*The audience in one sentence:*
"We are building for [audience type] who struggle with [core problem] and currently solve it by [alternative]."

*ICP tiers:*
Core / Scaling / Testing / Not a priority today, with the primary audience named.

*Primary problem solved today:*
One sentence, in the customer's language.

*What makes this market interesting:*
2–3 observations about the opportunity (size, growth, timing, underserved need).

*Competitive whitespace:*
Where competitors are weak or absent relative to this audience's most important needs.

*Candidate comparators (handoff to Define):*
The 2–3 alternatives the primary audience actually weighs — a named competitor, the status quo / "old way," or building it themselves — with the evidence for each. Do not pick one here; Define chooses the comparator and product type.

*Ecosystem opportunities:*
Top 2–3 complements or frenemies and why they matter.

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
- Which customer/segment to prioritize (reference the ICP tiers — confirm or adjust the primary audience)
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
- Market potential (TAM coverage now vs later, growth, timing; one sourced top-down size figure if needed)
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
`[Company] — PMM Context`

**If Google Drive is connected:**
Create a Google Doc with this title. Structure with clear headers per section. Share the link.

**If not connected:**
Save as `[company-slug]-pmm-context.md` and present via file card.

This document is read by all downstream skills before they execute. If a downstream skill is invoked without it, prompt the user to run Discover first.

**Keep it living:** add a "Last verified" date to each section and a "Sources" list at the end. When a downstream phase finds a fact has changed, update the Context Document rather than letting phases drift apart.

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
- Audit competitors and map the ecosystem
- Analyze the product (demo, docs, changelog)
- Map the TAM and tier ICPs

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
- Balanced across audience, market/ecosystem, product, and internal inputs
- Narrow — one primary audience, clearly tiered against the rest
- Sourced — every data point traceable, every gap flagged
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
| Persona template | Role, buyer role, goals, pains, motivations, objections, behavior (info sources, communities, tools, content preferences) |
| TAM coverage map | Company type × role, targetable now vs later |
| ICP tiering table | Core / Scaling / Testing / Not a priority today; primary audience |
| Market analysis template | Market trends, segment dynamics, demand drivers, barriers, opportunity implications |
| Competitor profile template | Target audience, positioning, messaging, business model, stage, GTM motion, content, strengths, weaknesses, pricing clues |
| Ecosystem map | Player, complement/frenemy, category, size, audience overlap, value exchange, risks/costs |
| Product analysis | Primary problem, features → use cases → benefits → ICP, differences vs alternatives |
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
- Do not stop at competitors — map complements and frenemies too
- Do not leave ICPs unranked — every ICP gets a tier, and one is named primary
- Do not build SAM/SOM layers — map TAM coverage instead
- Do not guess data — blank and flag anything you can't source
- Do not write positioning in Discover — hand Define the candidate comparators instead

---

## Downstream skills this feeds into

The Context Document is read by:
- **PMM Define** — uses JTBD canvas, persona profiles, ICP tiers, primary problem, product analysis, candidate comparators, and competitive whitespace
- **PMM Strategize** — uses ICP tiers, TAM coverage map, audience behavior, ecosystem map (partner and channel options), competitive matrix, and business case
- **PMM Get Set** — uses competitive matrix, persona profiles, and features → use cases → benefits map for sales enablement
- **PMM Grow** — uses JTBD outcomes as post-launch success criteria

---

## Reference frameworks

**Primary (structural backbone):**
- PMA Product Marketing Framework — Discover phase
- PMA Jobs-to-Be-Done Canvas
- PMA Competitor Intel Checklist
- PMA B2B Persona Questions
- PMA Market Sizing Template (optional — single top-down figure for the business case)
- PMA Business Case Template
- PMM-GPT best practice guidance (PMA, 2026)

**Secondary (philosophical lens and operating practices):**
- MKT1 / Emily Kramer — audience-focused product marketing; specifically:
  - Product marketing research pillars, TAM & ICP mapping, ICP tiers, ecosystem map (MKT1 Field Guide to B2B Startup Marketing, Part 2)
  - Research-before-positioning and the primary-problem output (MKT1 Guide to Positioning)
  - Complements and frenemies (MKT1 Guide to Ecosystem Marketing)
  - Audience behavior beyond firmographics (MKT1, How to build your growth marketing strategy)
  - Research reliability rules (MKT1, The Claude Code research playbook behind the State of Marketing Reports)
- SVPG / Martina Lauchengco (Loved) — PMM's role in product/market fit from the market side
