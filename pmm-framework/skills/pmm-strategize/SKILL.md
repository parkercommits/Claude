---
name: pmm-strategize
description: >
  This skill should be used when the user wants to "build the GTM strategy for [company/product]",
  "help me strategize [launch/product/segment]", "run the Strategize phase",
  "build a go-to-market plan", "define our GTM motion", "set objectives and KPIs for [launch]",
  "help me plan pricing and packaging", or "build the launch operating plan".
  Executes the PMA Strategize phase: 8 workstreams covering strategic point of view,
  OKRs/KPIs, GTM strategy, pricing/packaging, sales readiness, launch governance,
  validation planning, and budget/resourcing.
metadata:
  version: "0.1.0"
  author: "Parker Lyons"
---

# PMM Strategize Skill

## Trigger conditions
Invoke this skill when the user says any of the following (or close variants):
- "Build the GTM strategy for [company/product]"
- "Help me strategize [launch/product/segment]"
- "Run the Strategize phase"
- "Build a go-to-market plan"
- "Define our GTM motion"
- "Set objectives and KPIs for [launch]"
- "Help me plan pricing and packaging"
- "Build the launch operating plan"
- Any request to develop commercial strategy after Discovery is complete

**Prerequisite:** The Discover phase Context Document should exist before this skill runs. If it doesn't, prompt the user to run Discover first — or ask them to provide key discovery outputs directly (target audience, core problem, competitive context, market opportunity).

---

## Framework & philosophy

This skill executes the **Strategize phase of the PMA Product Marketing Framework.**

**The goal of Strategize is to turn insight into a coherent commercial plan.**

If Discover answers "What opportunity is real, for whom, and why?" — Strategize answers:
- What are we trying to achieve?
- Where will we play and how will we win?
- What GTM approach gives us the best chance of success?
- What must be true operationally for launch and adoption to work?

**The phase relationship:**
- Discover creates evidence
- Strategize creates choices
- Define (positioning) creates narrative
- Get Set (launch) activates the plan
- Grow optimizes it over time

**The PMM's role in Strategize:** PMM leads the strategic thread that connects product, sales, marketing, CS, and support — but does not become the default owner of every executional task. The job is to force strategic clarity on audience, use case, motion, pricing, readiness, and success metrics before execution starts. Strategy is decision-making, not planning.

---

## Engagement modes

- **Build mode** — Working at or for this company. All 8 workstreams apply. Access to internal data (CRM, pipeline, sales input, product roadmap).
- **Job hunt mode** — Targeting this company as a prospective employer. Build a hypothetical GTM strategy based on public information. Flag all assumptions clearly. This becomes a powerful interview artifact: "Here's the GTM strategy I'd recommend if I joined." Mark all outputs ⚠️ **Job Hunt Mode**.

---

## The eight Strategize workstreams

### Workstream 1 — Translate insights into a strategic point of view

Before building a GTM plan, turn research into a clear strategic recommendation. This is where PMM acts as the architect of product-market fit, not just a messenger between teams.

**Actions:**
- Reconfirm the core opportunity from Discover
- Define the commercial problem to solve: low awareness? poor conversion? weak differentiation? slow activation? poor retention?
- Identify the highest-potential audience and use case
- Clarify what changed or what's newly true in the market (why now)
- Define strategic constraints: budget, product maturity, sales model, legal/compliance, launch timing
- Make an explicit recommendation on where to focus — and where NOT to focus

**Questions to answer:**
- Which segment should we prioritize first?
- Which use case is most commercially valuable?
- What buyer pain is urgent enough to drive action?
- What is our likely adoption path?
- What risks could weaken launch success?
- What would make this a bad bet?

**Templates:** Strategic recommendation memo, Opportunity assessment, Segment prioritization framework, Use-case prioritization matrix, Risk and dependency log, Executive strategy brief

**Key output:** A strategic point of view stating who to target, what problem/use case to lead with, why now, why your company can win, and what constraints shape the plan.

**Good:** Clear choices with explicit tradeoffs, evidence-backed, leadership can immediately understand "why this, why now, why us."
**Weak:** Strategy is just a research summary, no prioritization, team tries to target everyone.

---

### Workstream 2 — Set measurable objectives and success criteria

Define what success actually means. Most GTM failures come from confusing activities with outcomes.

**Actions:**
- Define success across the full funnel: awareness → acquisition → conversion → activation → adoption → retention → expansion
- Separate leading indicators from lagging indicators
- Calibrate objectives to the initiative type: new category play, new product launch, feature launch, segment expansion, repositioning
- Align on stage gates for launch readiness and post-launch success
- Set metric ownership across teams

**Useful frameworks:**
- **OKRs** (Objective + Key Results)
- **North Star Metric + supporting KPIs**
- **AARRR** (Acquisition / Activation / Retention / Revenue / Referral)
- **Leading vs. lagging indicator mapping**
- **Stage-gate planning** (product readiness, GTM readiness, sales readiness, post-launch readiness)

**Example metrics a PMM may define:**
Pipeline created, qualified demand from target segment, trial starts / demo requests, activation rate, time to first value, conversion to paid, attach / adoption rate, win rate in target segment, competitive win rate, retention at 30/60/90/180 days, expansion revenue, message pull-through in sales calls, enablement completion and confidence.

**Templates:** GTM objectives framework, KPI tree, Launch scorecard, Stage-gate checklist, Metric definitions document, Success criteria worksheet

**Key output:** A measurement framework with business goal, KPIs, targets, owners, reporting cadence, and stage gates.

**Good:** Metrics connect to company goals, teams know what they own, success is measurable before launch starts, mix of near-term and long-term indicators.
**Weak:** "Success" = launching on time, no agreed KPIs, only vanity metrics, post-launch measurement is an afterthought.

---

### Workstream 3 — Build the go-to-market strategy

The heart of Strategize. PMM should own the GTM strategy even when cross-functional teams execute parts of it.

#### 3A. Audience strategy
- Primary target segment (narrow — resist the urge to list everyone)
- Secondary segment, if any
- Buyer vs. user focus
- Priority personas and buying committee roles
- Expansion path after initial traction

#### 3B. Use-case strategy
- Lead use case and use-case hierarchy
- Problem statement by audience
- Most compelling moment of value
- Which use case is best for launch vs. later expansion

#### 3C. Route-to-market
Choose the motion based on ACV, implementation complexity, buyer education needs, urgency, and internal sales capacity:
- **Self-serve / Product-led** — low ACV, high volume, users discover value themselves
- **Sales-led** — higher ACV, complex buying committee, needs human touchpoints
- **Partner-led** — reach via channel, reseller, or ecosystem
- **Hybrid** — PLG for initial adoption + sales overlay for expansion

#### 3D. Acquisition strategy
Match channels to the segment and buying motion — don't just list every channel:
- Paid acquisition
- Content / SEO
- Product-led loops
- Outbound sales
- Partner ecosystem
- Events / community
- Lifecycle / customer marketing
- Field marketing / ABM

For each prioritized channel, define: audience fit, expected role in the buyer journey, resource requirements, message implications, risks.

#### 3E. Conversion and onboarding strategy
Strategize is not just top-of-funnel:
- First-touch experience
- Handoffs between marketing → sales → CS → product
- Onboarding requirements
- Time to first value
- Proof points needed to reduce friction
- Retention risks created by poor launch assumptions

#### 3F. Internal communication and readiness strategy
- Who internally needs to know what, and when
- Who approves what
- What readiness milestones exist
- How launch dependencies will be managed

**Useful frameworks:** STP (Segmentation / Targeting / Positioning), Bowling pin strategy (one segment/use case first, then expand), GTM motion design, Customer journey mapping, Persona × channel mapping, Barrier analysis (awareness / credibility / adoption / switching barriers).

**Templates:** GTM strategy template, Audience and segment plan, Buyer journey map, Channel strategy worksheet, Route-to-market decision framework, Internal communication plan, Dependency tracker, Risk register, Launch workback plan.

**Key output:** A documented GTM strategy defining who you're targeting, which problem/use case you lead with, which motion you use, which channels you prioritize, how buyers move from awareness to value realization, and what internal orchestration is required.

**Good:** Narrow focus, GTM motion fits the product and segment, onboarding/retention implications built in early, channel choices tied to buyer behavior.
**Weak:** "We'll use all channels," no clarity on motion, strategy ends at lead generation, no internal coordination plan.

---

### Workstream 4 — Define pricing, packaging, and offer strategy

One of the most strategic and most commonly underdeveloped parts of Strategize. PMM should ensure pricing and packaging reflect value, buyer expectations, and market realities.

**Actions:**
- Clarify what is being sold: product, feature, module, bundle, service
- Recommend packaging options based on segment needs, use-case fit, willingness to pay, and adoption path
- Pressure-test pricing against: market norms, alternatives, value delivered, implementation effort, procurement friction
- Define launch offers if needed: beta access, early adopter pricing, limited-time incentives, bundled onboarding
- Identify packaging barriers: too many SKUs, confusing tiers, value buried in upper plans, misalignment with buyer mental models

**Useful frameworks:**
- Value-based pricing
- Good / Better / Best packaging
- Willingness-to-pay research
- Price metric evaluation (seat-based, usage-based, outcome-based, tier-based)
- Competitive price corridor analysis
- Van Westendorp price sensitivity analysis (when appropriate)

**Templates:** Pricing strategy brief, Packaging matrix, Price/value hypothesis log, Offer design template, Pricing objection map, Monetization recommendation memo.

**Key output:** A pricing and packaging recommendation with pricing logic, packaging rationale, offer strategy, expected commercial impact, and known risks/assumptions.

**Good:** Pricing tied to value and segment fit, packaging supports adoption and upsell, sales/onboarding implications understood, objections anticipated.
**Weak:** Pricing copied from competitors without strategic reasoning, packaging is feature-dump-driven, sales gets pricing the week before launch.

---

### Workstream 5 — Plan sales and customer-facing readiness

Strong strategy includes enablement planning early — not as a last-minute launch task. PMM owns the *what* and the value narrative; enablement mechanics often owned by others.

**Actions:**
- Map the buyer journey to the sales journey
- Identify core objections and proof needs
- Determine which conversations reps must be able to lead
- Define enablement priorities by role: SDRs, AEs, SEs, partners, CS, support
- Scope launch materials: sales decks, pitch narrative, demo talk track, battlecards, objection handling, customer email templates, FAQ
- Plan readiness sessions and certification if needed
- Establish a field feedback loop after launch

**Useful frameworks:**
- Readiness by role mapping
- Proof-point mapping
- Buyer question ladder
- Sales narrative architecture (pain → impact → value → proof → differentiation → next step)
- MEDDICC / Challenger / Consultative selling alignment depending on sales org style

**Templates:** Sales readiness plan, Enablement brief, Field messaging guide, Objection handling template, PMA Battlecard template (coda.io/@product-marketing-alliance-pma), Demo storyline template, Internal FAQ template.

**Key output:** A readiness plan with roles to enable, assets required, training timing, owner by deliverable, and field feedback mechanism.

**Good:** Enablement tailored by role, sellers understand buyer value not just features, materials align with GTM strategy, feedback from field built into iteration plans.
**Weak:** One generic launch deck for everyone, feature-heavy materials with no commercial story, readiness measured by attendance only.

---

### Workstream 6 — Build the launch operating plan and cross-functional governance

Strategize must become operational enough to guide execution. PMM facilitates cross-functional coordination without becoming the project manager for every function.

**Actions:**
- Create a cross-functional launch team with clear ownership across: product, PMM, demand gen, content, sales, enablement, CS, support, operations, legal/compliance
- Define launch tier and level of effort:
  - **Tier 1** — Major launch, high visibility, broad market change
  - **Tier 2** — Important segment or product launch
  - **Tier 3** — Smaller release or feature update
- Build a workback plan with dates, owners, dependencies, and approval flows
- Assign RACI responsibilities
- Document launch risks and mitigation plans
- Align on launch gates and sign-off criteria
- Plan beta or pilot activities where needed

**Useful frameworks:** RACI, Launch tiering, Workback planning, Stage-gate governance, RAID log (Risks / Assumptions / Issues / Dependencies), Beta/pilot planning, Retrospective loop design.

**Templates:** PMA Launch Plan template (coda.io/@product-marketing-alliance-pma), PMA Launch Checklist, PMA Launch Tiers template, RACI matrix, RAID log, Beta test plan, Cross-functional meeting cadence plan, Readiness tracker.

**Key output:** A cross-functional operating plan showing who does what, when it needs to happen, what dependencies exist, and what "launch-ready" means.

**Good:** Accountability is explicit, PMM owns strategic orchestration not every task, launch scope matches business importance, risks visible early.
**Weak:** PMM becomes project manager for every function, no one knows who owns critical work, every launch treated as Tier 1.

---

### Workstream 7 — Plan experiments, beta, and validation

The strongest Strategize phases don't assume the first launch plan is perfect. They de-risk assumptions before full-scale launch.

**Actions:**
- Identify which assumptions are still unproven: message resonance, onboarding friction, pricing sensitivity, channel performance, use-case appeal
- Decide whether a beta, pilot, soft launch, or limited rollout makes sense
- Define learning goals for the test
- Establish what would trigger: broader rollout / strategy revision / pause/no-go
- Collect structured feedback from users, buyers, sales, CS, support

**Useful frameworks:** Hypothesis-led testing, Beta program design, Soft launch / phased rollout, Pre-mortem analysis, Test-and-learn loops.

**Templates:** Beta plan, Test hypothesis sheet, Pilot evaluation scorecard, Pre-mortem worksheet, Go/no-go checklist.

**Key output:** A validation plan for testing critical assumptions before scaling.

**Good:** Team knows what's still uncertain, learning goals explicit, feedback directly informs launch refinement.
**Weak:** Beta used as a vague marketing teaser, no defined success criteria, feedback anecdotal and unsynthesized.

---

### Workstream 8 — Secure budget, resourcing, and executive alignment

Strategy without feasibility is aspiration. Ensure the GTM plan is resourced and approved.

**Actions:**
- Estimate required budget by channel and launch activity
- Identify team bandwidth constraints
- Clarify must-have vs. nice-to-have work
- Build scenarios: minimum viable launch / recommended plan / high-investment plan
- Align executives on tradeoffs and expected return
- Confirm what is feasible this cycle

**Useful frameworks:** Scenario planning, Impact vs. effort prioritization, Must/Should/Could, Budget-to-outcome planning, Decision memo structure.

**Templates:** GTM budget planner, Resource plan, Scenario planning worksheet, Executive decision memo, Prioritization matrix.

**Key output:** An approved resourcing and budget plan.

**Good:** Budget supports the strategy, clear priorities if resources tighten, leadership has explicitly approved tradeoffs.
**Weak:** Teams assume resources will appear later, strategy is overbuilt relative to capacity.

---

## Recommended minimum artifact stack

These seven documents are usually enough to move cleanly into Define and launch execution:

| # | Artifact | What it covers |
|---|---|---|
| 1 | Strategy brief | The big choices and rationale |
| 2 | GTM strategy doc | Target, motion, channel, buyer journey, onboarding |
| 3 | KPI and success framework | Objectives, metrics, owners, targets |
| 4 | Pricing and packaging brief | Monetization strategy |
| 5 | Sales/readiness brief | Who needs what to be ready |
| 6 | Launch plan + RACI | Milestones and ownership |
| 7 | Risk/dependency log | What could derail execution |

---

## Week-by-week operating model

**Week 1 — Focus the strategy**
- Confirm opportunity and target audience from Discover
- Prioritize segment and lead use case
- Write the strategic recommendation
- Align leadership on strategic direction

**Week 2 — Define success and GTM approach**
- Establish objectives and KPIs
- Choose GTM motion
- Map buyer journey
- Prioritize channels
- Identify onboarding and retention implications

**Week 3 — Shape commercial mechanics**
- Define pricing/packaging recommendation
- Outline sales narrative needs
- Identify objections and proof points
- Scope enablement and support needs

**Week 4 — Build the operating plan**
- Create launch plan
- Assign owners through RACI
- Identify risks and dependencies
- Align on stage gates and readiness criteria

**Week 5 — Validate and finalize**
- Decide on beta/pilot if needed
- Lock budget and resourcing
- Secure executive signoff
- Hand off into Define (positioning) / Get Set (launch execution)

---

## Decision framework for pressure-testing strategy

When reviewing the strategy, these are the most important questions:

| Dimension | Key questions |
|---|---|
| **Audience** | Is this the most valuable segment to win first? Are we targeting buyer, user, or both? |
| **Problem/use case** | Is this problem painful, urgent, and easy to communicate? Does this use case showcase value quickly? |
| **Differentiation** | Can we win with a clear commercial story? Do we have proof that buyers will care? |
| **Motion** | Is the route to market appropriate for deal size and complexity? Can our current teams support this motion? |
| **Readiness** | Is the product mature enough? Can sales, CS, and support deliver a good experience? |
| **Economics** | Does pricing reflect value and fit buyer expectations? Is the plan feasible with available budget? |
| **Measurement** | What metrics will tell us early if this is working? What would trigger an adjustment? |

---

## Common mistakes to avoid

1. **Moving into execution too quickly** — jumping from research to launch checklists without making clear strategic decisions
2. **Targeting too broadly** — trying to please multiple segments, use cases, and stakeholders at once
3. **Ignoring product maturity** — designing an ambitious GTM for a product that isn't operationally ready
4. **Treating strategy as marketing-only** — underinvolving sales, CS, support, and product in readiness planning
5. **Underthinking onboarding and retention** — optimizing for lead generation, then being surprised by poor activation or churn
6. **Leaving pricing too late** — positioning value without confirming how value will be monetized
7. **Failing to define ownership** — assuming cross-functional alignment without formal accountability

---

## What good Strategize looks like

A strong Strategize phase is:
- **Choiceful** — makes real decisions, not broad statements
- **Commercially grounded** — links strategy to revenue, adoption, retention, or pipeline
- **Cross-functional** — aligns product, sales, marketing, CS, and support early
- **Feasible** — matches budget, product maturity, and internal capacity
- **Customer-centered** — keeps the buyer/user journey central, not internal preferences
- **End-to-end** — considers acquisition AND onboarding, adoption, and retention
- **Measurable** — defines KPIs and stage gates before launch
- **Owned but not over-owned by PMM** — PMM leads strategy, doesn't become the dump for every task

A weak Strategize phase has: no real prioritization, GTM plan is a list of activities, vague success metrics, channel plan based on habit not behavior, pricing decided too late, reactive feature-heavy enablement, no RACI or governance, no readiness criteria, no risk mitigation, no onboarding/retention plan.

---

## What NOT to do

- Do not start Strategize without a completed Discover output — strategy without evidence is guesswork
- Do not let "targeting everyone" survive past Workstream 1
- Do not leave pricing for the product team to handle alone — PMM must be in the room
- Do not conflate launch project management with GTM strategy ownership
- Do not skip the beta/validation plan — it is the difference between an educated launch and a costly assumption

---

## Downstream skills this feeds into

The Strategize outputs (particularly the GTM strategy doc, KPI framework, and launch plan) are read by:
- **PMM Define** — uses audience strategy, use-case prioritization, and competitive positioning to build the messaging architecture
- **PMM Get Set** — uses the launch plan, RACI, sales readiness plan, and enablement brief to execute
- **PMM Grow** — uses KPIs and success criteria to measure post-launch performance and prioritize optimization

---

## Reference frameworks

**Primary (structural backbone):**
- PMA Product Marketing Framework — Strategize phase
- PMA GTM Template (coda.io/@product-marketing-alliance-pma)
- PMA Launch Tiers (coda.io/@product-marketing-alliance-pma)
- PMA Internal Roadmap Template (coda.io/@product-marketing-alliance-pma)
- PMA OKR Toolkit (coda.io/@product-marketing-alliance-pma)
- PMA Guide to Pricing Models (coda.io/@product-marketing-alliance-pma)
- PMM-GPT best practice guidance (PMA, 2026)

**Secondary (philosophical lens):**
- MKT1 / Emily Kramer — audience-first strategy; packaging around ICP needs not feature bundles
- SVPG / Martina Lauchengco (Loved) — GTM as equal partner to product discovery
