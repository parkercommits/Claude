---
name: pmm-strategize
description: "This skill should be used when the user wants to \"build the GTM strategy for [company/product]\", \"help me strategize [launch/product/segment]\", \"run the Strategize phase\", \"build a go-to-market plan\", \"define our GTM motion\", \"set objectives and KPIs for [launch]\", \"help me plan pricing and packaging\", or \"build the launch operating plan\". Executes the PMA Strategize phase: 8 workstreams covering strategic point of view (revenue levers, marketing advantages, working positioning and perceptions), goals and KPIs, GTM strategy and growth engines, pricing/packaging, sales readiness, launch governance, validation planning, and budget/resourcing.\n"
metadata:
  version: "0.5.0"
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

**Prerequisite:** The Discover phase Context Document should exist before this skill runs. If it doesn't, prompt the user to run Discover first — or ask them to provide key discovery outputs directly (target audience, core problem, competitive context, market opportunity). Strategize relies especially on Discover's ICP tiers, audience behavior, ecosystem map, candidate comparators, and candidate marketing advantages.

**Inherit or build (scope).** PMA's Strategize plans an initiative — usually a launch. MKT1's strategy work is company-level: what drives growth for the whole business. Strategize needs both, but should not rebuild the company level every time:
- **If the company already has a marketing strategy** (prioritized marketing advantages, ranked revenue levers, perceptions, ICP tiers, positioning), inherit it. Check the initiative against it and flag conflicts.
- **If it doesn't** — common at startups, and always true in job hunt mode — draft a light version in Workstream 1 and mark it as a working draft.

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

**The three drivers of marketing strategy (MKT1).** Every strategy should rest on:
1. **Product marketing research** — audience, market/ecosystem, and product (from Discover)
2. **Business model and GTM motion** — self-serve vs. sales-led, deal size, adoption path
3. **Marketing advantages** — the company's built-in tailwinds

You can't copy another company's strategy, because its audience, model, and advantages differ. Copying tactics without fit is what MKT1 calls "random acts of marketing."

---

## Engagement modes

- **Build mode** — Working at or for this company. All 8 workstreams apply. Access to internal data (CRM, pipeline, sales input, product roadmap).
- **Job hunt mode** — Targeting this company as a prospective employer. Build a hypothetical GTM strategy based on public information. Flag all assumptions clearly. This becomes a powerful interview artifact: "Here's the GTM strategy I'd recommend if I joined." Mark all outputs ⚠️ **Job Hunt Mode**.

---

## Inputs and connections

Start from the **Engagement setup** and the Discover section of the Context Document. Re-check which tools are connected (see `skills/pmm-director/references/connections.md`); ask only for what's missing. If MKT1 tools (`mkt1_*`) are connected, use them for the steps that name one, following `skills/pmm-director/references/mkt1-tools.md`.

**MKT1 tools in Strategize:** `mkt1_revenue_levers` (1A), `mkt1_marketing_advantages` (1B), `mkt1_big_bets` and `mkt1_kpo_goals` (Workstream 2), and `mkt1_channel_strategy` (3D). Run them in that order: levers and advantages feed the big bets, and big bets become the project goals. Each step below says what to keep from the plugin's own method alongside the tool.

### Company profile and existing work (build mode)

If the team has a company profile (created by `pmm-setup`), read sections 7 (GTM plan), 5 (Pricing and packaging), 2 (Audiences and ICP tiers), and 8 (Teams, tools, and processes) before starting, and skip any question they already answer. If section 8 lists frameworks or experts the team has adopted for this kind of work, use their structure and vocabulary, mapped onto this phase's steps (see "When sources disagree" in the Director).

**Audit before you build.** If the team already has the current marketing or GTM plan, calendar, roadmap, and pricing sheet, start from them. Inherit them (see "Inherit or build" above), check this initiative against them, and flag conflicts — don't draft a parallel strategy.

**Propose profile updates; don't make them silently.** When this phase produces something durable — revenue lever ranking, marketing advantages, big bets on the calendar, and pricing changes — show the proposed change to the section owner and add a change-log line once they agree. If there's no profile, suggest `pmm-setup` once, then continue without it.

### Where each input comes from

| Input | Job hunt mode — where it comes from | Build mode — where it comes from |
|---|---|---|
| Company-level strategy to inherit (advantages, levers, perceptions) | Public signals: executive interviews, investor updates, the job posting | **Docs and wiki** — marketing strategy, annual plan, board decks the user can share |
| Business model, GTM motion, deal size | Pricing page, sales vs. self-serve signup, careers page (sales roles) | **CRM** — deal size, cycle length, win rate by segment and motion |
| Revenue lever maturity | Public signals of expansion, upmarket moves, new segments | **CRM** and **product analytics** — new logo vs. expansion mix, retention |
| Growth engine performance | Content footprint, events, partner pages, social presence | **Web and marketing analytics** — traffic and conversion by source; **CRM** campaign influence |
| Pricing and packaging | Pricing page, review-site pricing comments | **Docs** — pricing documentation; **CRM** — discounting patterns |
| What's shipping | Changelog, public roadmap, release notes | **Roadmap and issues** — upcoming releases and scope |

In build mode, pull scoped samples (e.g., the last 2–4 quarters) and cite the tool and date range for each figure. Follow the guardrails in `skills/pmm-director/references/connections.md`.

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

#### 1A. Rank the four revenue levers (MKT1)

Make "where to focus" concrete. Stack-rank, 1–4, no ties, by where marketing can have the biggest impact in the next 6–12 months. Use these four names exactly; MKT1's tools and templates use them:

| Lever | What it means | Current maturity (investing / starting / nothing yet) |
|---|---|---|
| **Grow TOF with existing audience** | More market share with Core-tier ICPs | |
| **Grow TOF with new audience** | Reach new segments, channels, geographies, or use cases (Scaling or Testing ICPs) | |
| **Increase value per customer** | Pricing, upsell, expansion, retention, moving upmarket | |
| **Improve efficiency** | Better conversion, lower acquisition cost, faster cycles, less waste | |

For each lever, write one or two sentences on **why it ranks there** and a directional **what to focus on**. For the top one or two levers, state how this initiative moves them. Levers ranked 3–4 become explicit non-goals unless the initiative clearly serves them. Relying only on top-of-funnel volume gets harder as the TAM saturates.

**Connect levers to ICP tiers.** The existing-audience lever is about Core ICPs; the new-audience lever is about Scaling or Testing ICPs. Say which.

**Typical patterns** (starting points, not answers): an early-stage company still proving fit usually leads with the existing audience, then efficiency. One whose Core audience is saturated leads with the new audience. High churn puts value per customer first. Plenty of pipeline with weak conversion puts efficiency first. A new product that opens a new audience puts that audience first.

**Name the trap** — the most likely way this team misallocates effort given its ranking. Common ones: ranking efficiency first without enough volume to optimize; ignoring value per customer because marketing "only does acquisition"; ranking by what sales can do rather than what marketing can move.

**With MKT1 tools:** run `mkt1_revenue_levers` and write the result to **REVENUE LEVERS**. Keep the maturity column above and the line on how this initiative moves the top levers; the tool doesn't add them.

#### 1B. Identify and prioritize marketing advantages (MKT1)

Marketing advantages are strengths or positive dynamics in the business, product, team, or story that accelerate growth — tailwinds. Examples: network effects, a free plan or free tool, integrations and an ecosystem, a strong community, a compelling founder or company story, market timing (a new regulation or shift), a clear vertical wedge, unusual customer love. Most successful later-stage companies leverage two or more.

**Look across four kinds of advantage** so the list isn't only product features. Use these as prompts, not boxes to fill; a company's real advantage often combines several, or fits none of them:
- **Product-driven:** virality or network effects; a free plan or trial with a fast first-value moment; an obvious, major differentiator; integrations that create lock-in or distribution
- **Ecosystem-driven:** partners with a real incentive to recommend or resell; an audience that seeks a community; market tailwinds such as a new regulation or technology shift
- **Fuel-driven (content and creative):** a company or founder story the ICP finds credible; an audience hungry for education where the company has a distinct point of view; raw material no one else has — customer love, proprietary data, a contrarian take
- **Engine-driven (distribution):** a narrow wedge with a path to expand; a channel already working at a viable acquisition cost beyond founder effort; an audience that seeks live or in-person experiences

**The test:** an advantage changes what you'd do in go-to-market. If it doesn't, or if competitors have the same thing, it's a requirement, not an advantage.

**Run the exercise** (start from Discover's candidate advantages):
1. List the advantages.
2. Rate each: **strength today**, **potential strength** if fully used (low / medium / high), and **maturity** — nascent (not yet used in marketing), testing (campaigns running), or scaled (a proven, repeatable growth driver).
3. Check competitors: do they have the same advantage, and use it the same way? If everyone has it, it isn't an advantage.
4. Note combinations — advantages that reinforce each other.
5. Prioritize each high / medium / low, and keep the 1–3 that could change the growth trajectory; several listed advantages often collapse into one compound advantage.
6. Name the projects that would accelerate each priority advantage (these feed big bets in Workstream 2).

**With MKT1 tools:** run `mkt1_marketing_advantages` — its identify mode works through discovery questions with the user; its review mode pressure-tests a list the team already has. Write the confirmed 1–3 advantages to **MARKETING ADVANTAGES**, and keep step 6 above (the projects that would accelerate each), which feeds the big bets.

**Watch-outs:** an advantage doesn't drive growth on its own — it needs investment. Some need company-wide buy-in (product for network effects; GTM teams for ecosystem). Some can be built deliberately (a free plan, a vertical wedge); others, like a compelling story, are hard to force. If the company has no advantages, say so — it signals a product, business, or GTM problem, not a marketing one.

#### 1C. Draft the working positioning hypothesis and perceptions

Strategy choices rest on a view of how the product wins, so draft one now; Define tests and finalizes it.

- **Positioning hypothesis:** product type (vertical solution / new way / 10x better / buy vs. build), one comparator, and the three answers — who it's for, what it is, why it's better than the comparator. Start from Discover's candidate comparators and primary audience. Optionally add a "one year out" version.
- **Working perceptions:** 3–4 beliefs you want the audience to repeat back, written in their voice, each tagged market / company / product / community and strong / emerging / not yet driven. These anchor the big bets in Workstream 2.

Keep both short and mark them **working drafts**. Define (Steps 3, 4, and 11) owns the final versions and logs what changed — and, when MKT1 tools are connected, runs `mkt1_positioning` and `mkt1_perceptions` for them. Here, a light draft from Discover's inputs is enough.

**Templates:** Strategic recommendation memo, Revenue lever stack-rank, Marketing advantages worksheet, Working positioning hypothesis, Working perceptions, Opportunity assessment, Segment prioritization framework, Use-case prioritization matrix, Risk and dependency log, Executive strategy brief

**Key output:** A strategic point of view stating who to target, what problem/use case to lead with, why now, why your company can win, and what constraints shape the plan — plus ranked revenue levers, prioritized marketing advantages, a working positioning hypothesis, and working perceptions.

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

**Set goals across three types — KPIs aren't a plan on their own (MKT1 KPO goals):**
- **K — KPIs:** the metrics above, derived from the top-ranked revenue levers
- **P — Projects:** 1–3 **big bets** — initiatives that could drive outsized impact. Treat the launch itself as a big bet. Each big bet names its target ICP tier, the perception it drives, the marketing advantage it accelerates, its growth engine(s), the content it needs, and its success criteria.
- **O — Ops:** foundational work the plan depends on — tools, tracking, hiring, workflows, repeatable processes

Also list **non-goals** (what this initiative deliberately won't do), plus dependencies and risks. Without projects and ops goals, growth stays linear.

**Keep the goal set small and connected.** Five to eight goals in total — usually two or three KPIs, two or three projects (the big bets), and one or two ops goals. Tag each goal with the marketing advantage, perception, and revenue lever it supports; if a goal connects to none, ask why it's a goal. Targets nobody has set stay "TBD," never invented.

**Make each big bet a real campaign.** A big bet combines **fuel** (a specific content or creative idea), an **engine** (a named distribution channel), and a **specific audience** (a Core or Scaling ICP). It should connect to at least three of: an advantage it accelerates, the ICP it targets, a perception it reinforces, and a top-two revenue lever. Then score each bet:

| Check | Question |
|---|---|
| Big enough? | Could it change the growth trajectory, or compound if it works? A one-off is a tactic. |
| All components? | Is the fuel specific, the engine named, the audience specific? |
| Fits the model? | Does the engine fit the GTM motion? For events, outbound, or partner bets, are there tiered target accounts? |
| Aligns with strategy? | Which advantage, ICP, perception, and lever does it connect to? |

Mark each ✅ or ⚠️, and for each ⚠️ ask the question that would fix it rather than dismissing the idea. For events and partner bets, measure **account-stage progression** for target accounts (unaware → engaged → evaluating), not just sourced pipeline — these channels are rarely the first or last touch.

**With MKT1 tools:** run `mkt1_big_bets` (write to **BIG BET CAMPAIGNS**), then `mkt1_kpo_goals` (write to **KPO GOALS**). Keep the non-goals, dependencies, and risks, and each big bet's content needs and success criteria; the tools don't add them.

**Templates:** GTM objectives framework, KPO goals sheet (KPIs / Projects / Ops / non-goals; MKT1's Marketing goals tracker is a good base), Big bet brief and scorecard, KPI tree, Launch scorecard, Stage-gate checklist, Metric definitions document, Success criteria worksheet

**Key output:** A measurement framework with business goal, KPIs, targets, owners, reporting cadence, and stage gates — plus 1–3 big bets, ops goals, and non-goals.

**Good:** Metrics connect to company goals, teams know what they own, success is measurable before launch starts, mix of near-term and long-term indicators.
**Weak:** "Success" = launching on time, no agreed KPIs, only vanity metrics, post-launch measurement is an afterthought.

---

### Workstream 3 — Build the go-to-market strategy

The heart of Strategize. PMM should own the GTM strategy even when cross-functional teams execute parts of it.

#### 3A. Audience strategy
Start from Discover's ICP tiers rather than re-deriving segments:
- **Primary audience** — the one Core-tier ICP this initiative leads with (narrow — resist the urge to list everyone)
- **Effort by tier** — rough share of time and budget for Core / Scaling / Testing; "Not a priority today" gets none
- Buyer vs. user focus
- Priority personas and buying committee roles
- **Expansion path** — the plan to move Scaling and Testing ICPs up a tier after initial traction
- **Compare with time allocation today** (from Discover's ICP tiers) and say what shifts
- **Playbook by tier** — which content types and engines each tier gets, so lower tiers don't get the full treatment. A simple grid works: content and channels down the side, tiers across the top.
- **Per-segment message notes** for each priority segment: what the product replaces for them, what it is, and why it's better for them, plus the discovery questions and timing signals (funding, a new GTM push, a regulation date) that tell sales a prospect is ready. Define Step 6 and Get Set Step 4 build on these.

#### 3B. Use-case strategy
- Lead use case and use-case hierarchy
- Problem statement by audience
- Most compelling moment of value
- Which use case is best for launch vs. later expansion

#### 3C. Route-to-market
Choose the motion based on ACV, implementation complexity, buyer education needs, urgency, and internal sales capacity:
- **Pure self-serve** — low ACV, high volume; buyers sign up, try, and buy without talking to anyone
- **Self-serve dominant hybrid** — most revenue self-serve, with a sales-assisted tier for bigger deals
- **Balanced hybrid** — meaningful revenue from both; marketing needs scale and precision
- **Sales-led dominant hybrid** — most revenue through sales, with a free or low-cost entry point feeding pipeline
- **Pure sales-led** — every deal goes through sales; higher ACV, buying committee, knowable target accounts

Partner-led reach (channel, reseller, ecosystem) sits on top of any of these as a growth engine (3D), not a separate motion.

**Classify from what you can observe**, especially in job hunt mode:

| Signal | Self-serve leaning | Hybrid | Sales-led leaning |
|---|---|---|---|
| Deal size and time to close | Lower; fast sign-up | Wide range | Higher; longer cycle |
| Plans and pricing | Free and paid plans shown | Range of plans | Paid, often "contact us" |
| Adoption | Bottom-up, by users | Both | Top-down, by an executive |
| Homepage call to action | Sign up | Both | Request a demo |
| Marketing KPIs | Sign-ups, product-qualified leads | All | Qualified pipeline |
| Team mix | Marketing larger than sales | Similar | Sales larger than marketing |

**Check that marketing fits the motion (MKT1):** e.g., gated content and demo-only CTAs fight an easy-to-adopt self-serve product; pure self-serve content won't carry a six-figure, committee-led deal. If changing the motion is on the table, estimate the company-wide impact (billing, RevOps, onboarding) before recommending it.

#### 3D. Acquisition strategy — choose growth engines (MKT1)
Don't list every channel. Group channels into engines and choose a focused set:

| Engine | What it includes | Tends to fit when… |
|---|---|---|
| **Inbound** | Content, SEO, AEO/LLM visibility, social, paid search | The audience actively searches for or learns about the problem |
| **Outbound** | SDR/AE prospecting, ABM, targeted paid | High-value accounts, a defined target list, sales-led motion |
| **Product virality** | Free plans, invites, sharing, product-led loops | The product has network effects or is naturally shared |
| **Events** | Webinars, conferences, field events, dinners | The audience values in-person or peer learning |
| **Ecosystem** | Integrations, partners, communities, influencers, agencies, affiliates | The product connects to tools the audience already uses, or others reach the audience credibly |
| **Lifecycle** | Onboarding, nurture, customer marketing, expansion | After the top of funnel — activation, retention, expansion (and virality if used for referrals) |

**Choose engines from the three drivers:** audience behavior and ecosystem (from Discover), GTM motion (3C), and marketing advantages (1B). Then:
- Run a **focused set** now, but plan for a **mix over time** — single channels saturate, decline, or get disrupted
- **Pair engines that reinforce each other** (content feeding outbound follow-up; events supporting outbound)
- **Don't invest in virality or outbound before the product supports it**
- Don't silo engines between teams (e.g., marketing's inbound and sales' outbound sending prospects conflicting messages)

**Score each engine 1–5 for fit** — 5 means several drivers point to it; 1 means they point away. It isn't a stack rank; several engines can share a score. Layer three lenses:
- **GTM motion:** self-serve needs scale (inbound, product virality); sales-led needs precision against a knowable list of accounts (outbound, events, ecosystem); hybrids need both.
- **Market type** (from Discover): a **new category** has little search demand, so inbound is weak and events and product experience do the educating; a **vertical** has a bounded, knowable audience, so outbound, ecosystem, and events lead and virality rarely compounds; a **free plan or trial** favors inbound and virality over outbound.
- **Marketing advantages:** each advantage speeds certain engines — integrations favor ecosystem; a credible founder story favors inbound thought leadership and events; a regulatory or market deadline favors inbound education, events, and urgency in outbound.

**Senior buyers and rip-and-replace purchases:** when the buyer is a C-level executive, or buying means replacing a core system, trust comes from experiences and recommendations. Events and ecosystem lead; outbound's job is to get target accounts into them.

For each engine scored 3 or more, name two to four specific tactics and why they fit. Recommend one or two **engine pairings** that reinforce each other (for example, outbound inviting target accounts to an event, or co-hosted events with a partner), each with a concrete example for this company. For sales-led motions, track account stages and campaign influence at the account level, not just leads.

**With MKT1 tools:** run `mkt1_channel_strategy` and write the result to **CHANNEL STRATEGY**. Keep the per-engine details below; the tool doesn't add resourcing or risks.

For each chosen engine, define: audience fit, expected role in the buyer journey, resource requirements (including the content it needs — see Workstream 8), message implications, risks.

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

**Useful frameworks:** STP (Segmentation / Targeting / Positioning), Bowling pin strategy (one segment/use case first, then expand), MKT1 ICP tiers, MKT1 growth engines, GTM motion design, Customer journey mapping, Persona × engine mapping, Barrier analysis (awareness / credibility / adoption / switching barriers).

**Templates:** GTM strategy template, Audience and segment plan (with a playbook by tier), Buyer journey map, Channel strategy worksheet (engine fit scores, tactics, pairings), Route-to-market decision framework, Internal communication plan, Dependency tracker, Risk register, Launch workback plan.

**Key output:** A documented GTM strategy defining who you're targeting, which problem/use case you lead with, which motion you use, which channels you prioritize, how buyers move from awareness to value realization, and what internal orchestration is required.

**Good:** Narrow focus, GTM motion fits the product and segment, onboarding/retention implications built in early, engine choices tied to buyer behavior and marketing advantages.
**Weak:** "We'll use all channels," channels copied from another company, no clarity on motion, strategy ends at lead generation, no internal coordination plan.

---

### Workstream 4 — Define pricing, packaging, and offer strategy

One of the most strategic and most commonly underdeveloped parts of Strategize. PMM should ensure pricing and packaging reflect value, buyer expectations, and market realities.

**Actions:**
- Clarify what is being sold: product, feature, module, bundle, service
- Recommend packaging options based on segment needs, use-case fit, willingness to pay, and adoption path
- Pressure-test pricing against: market norms, alternatives, value delivered, implementation effort, procurement friction
- Define launch offers if needed: beta access, early adopter pricing, limited-time incentives, bundled onboarding
- Identify packaging barriers: too many SKUs, confusing tiers, value buried in upper plans, misalignment with buyer mental models
- Decide the **plans and pricing page** approach (below)

**Plans and pricing page (MKT1):**
- Have one. A plans page clarifies what the product is and which packages exist, even without prices. Exceptions: a single plan, or a product not yet defined.
- Show at least some prices — often the lowest tier. Hiding prices drives evaluators to competitors that show theirs, doesn't stop buyers finding prices elsewhere, and moves sticker shock into sales calls.
- Avoid "fake" gating — a form or chat that leads to a demo request without ever revealing price.
- Keep the model simple; avoid pages full of sliders, calculators, and toggles. If the model is complex, add an FAQ or a short note on pricing philosophy.
- The pricing page should reinforce the positioning hypothesis. If a page with prices isn't converting, suspect price/expectation mismatch, weak value messaging, or an overcomplicated model.
- If transparency is contested internally, test it: plans-only → lowest tier shown → full pricing, measuring conversion through the funnel.
- Note market norms: usage-based pricing is spreading, especially for AI products where usage drives cost. Check what the comparator and alternatives charge on.

**Useful frameworks:**
- Value-based pricing
- Good / Better / Best packaging
- Willingness-to-pay research
- Price metric evaluation (seat-based, usage-based, outcome-based, tier-based)
- Competitive price corridor analysis
- Van Westendorp price sensitivity analysis (when appropriate)

**Templates:** Pricing strategy brief, Packaging matrix, Price/value hypothesis log, Offer design template, Pricing objection map, Plans and pricing page decision, Monetization recommendation memo.

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
- Estimate required budget by engine and launch activity
- Identify team bandwidth constraints
- **Check fuel vs. engine balance (MKT1):** "fuel" is what you create (messaging, content, creative); "engine" is the channels that distribute it. For each chosen engine, confirm there is capacity to produce the content it needs. Startups often over-invest in one side — channels with nothing to say, or content no channel distributes.
- Clarify must-have vs. nice-to-have work
- Build scenarios: minimum viable launch / recommended plan / high-investment plan
- Align executives on tradeoffs and expected return
- Confirm what is feasible this cycle

**Useful frameworks:** Scenario planning, Impact vs. effort prioritization, Must/Should/Could, Budget-to-outcome planning, Decision memo structure.

**Templates:** GTM budget planner (MKT1's Marketing budget & efficiency metrics sheet includes a budget calculator), Fuel and engine balance exercise, Resource plan, Scenario planning worksheet, Executive decision memo, Prioritization matrix.

**Key output:** An approved resourcing and budget plan.

**Good:** Budget supports the strategy, clear priorities if resources tighten, leadership has explicitly approved tradeoffs.
**Weak:** Teams assume resources will appear later, strategy is overbuilt relative to capacity.

---

## Recommended minimum artifact stack

These eight documents are usually enough to move cleanly into Define and launch execution:

| # | Artifact | What it covers |
|---|---|---|
| 1 | **Strategy on a page** | Prioritized marketing advantages, ICP tiers and primary audience, working perceptions, working positioning hypothesis, ranked revenue levers, KPO goals and big bets. Modeled on MKT1's marketing decision dashboard. |
| 2 | Strategy brief | The big choices and rationale |
| 3 | GTM strategy doc | Target, motion, growth engines, buyer journey, onboarding |
| 4 | KPI and success framework | KPIs, big bets, ops goals, non-goals, owners, targets |
| 5 | Pricing and packaging brief | Monetization strategy and pricing page approach |
| 6 | Sales/readiness brief | Who needs what to be ready |
| 7 | Launch plan + RACI | Milestones and ownership |
| 8 | Risk/dependency log | What could derail execution |

**Write "Strategy on a page" into the Context Document** (a Strategize section beneath Discover's) so Define, Get Set, and Grow read the same inputs. Put the strategy inputs under their section names — **REVENUE LEVERS**, **MARKETING ADVANTAGES**, **BIG BET CAMPAIGNS**, **KPO GOALS**, **CHANNEL STRATEGY** — so they match MKT1's tools and templates.

---

## Week-by-week operating model

**Week 1 — Focus the strategy**
- Confirm opportunity, ICP tiers, and primary audience from Discover
- Inherit or draft the company-level inputs: revenue levers, marketing advantages
- Prioritize segment and lead use case
- Draft the working positioning hypothesis and working perceptions
- Write the strategic recommendation
- Align leadership on strategic direction

**Week 2 — Define success and GTM approach**
- Establish KPO goals: KPIs, big bets, ops goals, non-goals
- Choose GTM motion and check marketing fits it
- Map buyer journey
- Score growth engines for fit; choose engines and pairings
- Design and score big bets
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
- Lock budget and resourcing; check fuel vs. engine balance
- Write "Strategy on a page" into the Context Document
- Secure executive signoff
- Hand off into Define (positioning) / Get Set (launch execution)

---

## Decision framework for pressure-testing strategy

When reviewing the strategy, these are the most important questions:

| Dimension | Key questions |
|---|---|
| **Audience** | Is this the most valuable segment to win first? Are we targeting buyer, user, or both? |
| **Problem/use case** | Is this problem painful, urgent, and easy to communicate? Does this use case showcase value quickly? |
| **Differentiation** | Can we win with a clear commercial story? Do we have proof that buyers will care? Is there one clear comparator? |
| **Advantages** | Which marketing advantages does this plan accelerate? Are they real advantages, or things every competitor has? |
| **Focus** | Which revenue levers does this move? What are the explicit non-goals? |
| **Motion** | Is the route to market appropriate for deal size and complexity? Can our current teams support this motion? Does the marketing fit it? |
| **Engines** | Are engines scored against motion, market type, and advantages — or copied from habit? Is there content capacity for each? |
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
8. **Random acts of marketing** — copying channels or tactics from other companies without checking fit
9. **Ignoring marketing advantages** — planning as if the company has no tailwinds, or claiming advantages every competitor shares
10. **KPIs without projects** — setting targets with no big bets or ops work to reach them
11. **Fuel and engine out of balance** — channels with nothing to say, or content nothing distributes
12. **Hiding prices by default** — pushing sticker shock into sales calls instead of deciding pricing transparency deliberately
13. **Too many big bets** — five "big bets" means none; keep one to three

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
- Do not rebuild company-level strategy for every launch — inherit it when it exists
- Do not finalize positioning or perceptions here — draft them as working hypotheses for Define

---

## Downstream skills this feeds into

The Strategize outputs (particularly Strategy on a page, the GTM strategy doc, KPI framework, and launch plan) are read by:
- **PMM Define** — uses the working positioning hypothesis and working perceptions (to test and finalize), audience strategy, use-case prioritization, and competitive positioning to build the messaging architecture
- **PMM Get Set** — uses the launch plan, RACI, big bets, chosen growth engines, sales readiness plan, and enablement brief to execute
- **PMM Grow** — uses KPIs, big bet success criteria, revenue lever ranking, and success criteria to measure post-launch performance and prioritize optimization

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

**Secondary (philosophical lens and operating practices):**
- MKT1 / Emily Kramer — audience-first strategy; packaging around ICP needs not feature bundles; specifically:
  - Random acts of marketing, fuel and engine, marketing advantages, three drivers of strategy, four revenue levers, KPO goals, decision dashboard (MKT1 Field Guide to B2B Startup Marketing, Part 1)
  - Growth engines and channel selection (Field Guide, Part 2; MKT1 Guide to Channel <> Startup fit)
  - Marketing advantages exercise, GTM motion alignment (Marketing strategy exercises to kick off your annual planning process; Find & accelerate your marketing advantages)
  - Strategy file structure: ICP priorities, perceptions, positioning, revenue levers, big bets (How to build your marketing strategy in Claude)
  - Plans and pricing pages (Why all B2B startups need plans & pricing pages); usage-based pricing trend (State of B2B Marketing Report 2026, Part 2)
  - Templates: Rank the 4 revenue levers, Marketing advantages checklist & exercise, Market prioritization/segmentation (playbook by tier), Channel <> strategy fit, Select marketing tactics that fit your strategy, Marketing goals tracker, Marketing decision dashboard, Marketing budget & efficiency metrics, Exercise to balance fuel & engine
  - MKT1 MCP tools, when connected: `mkt1_revenue_levers`, `mkt1_marketing_advantages`, `mkt1_big_bets`, `mkt1_kpo_goals`, `mkt1_channel_strategy`
- SVPG / Martina Lauchengco (Loved) — GTM as equal partner to product discovery
