---
name: pmm-get-set
description: >
  This skill should be used when the user wants to "help me plan the launch for [product/feature]",
  "build the launch plan", "run the Get Set phase", "create the sales enablement for [launch]",
  "build launch readiness", "write the battlecard / objection handling / sales deck",
  "what do we need before we can launch", "set up the go/no-go process", or
  "operationalize the launch". Executes the PMA Get Set phase: 12 steps covering launch
  tiering, planning, asset briefs, sales enablement, CS readiness, commercial mechanics,
  internal comms, governance, QA, measurement setup, readiness review, and launch handoff.
metadata:
  version: "0.1.0"
  author: "Parker Lyons"
---

# PMM Get Set Skill

## Trigger conditions
Invoke this skill when the user says any of the following (or close variants):
- "Help me plan the launch for [product/feature]"
- "Build the launch plan"
- "Run the Get Set phase"
- "Create the sales enablement for [launch]"
- "Build launch readiness for [product]"
- "Write the battlecard / objection handling / sales deck"
- "What do we need before we can launch?"
- "Set up the go/no-go process"
- "Build the launch QA checklist"
- "Help me operationalize the launch"
- Any request to execute a launch or prepare teams after positioning and strategy are defined

**Prerequisite:** The Define phase should be complete — specifically: approved positioning statement, messaging framework, value pillars, proof points, persona guidance, and use-case narratives. The Strategize phase should also be complete — GTM motion, target segment, pricing/packaging direction, KPIs, and launch tier. If these don't exist, ask the user to provide them or run the relevant phases first.

---

## Framework & philosophy

This skill executes the **Get Set phase of the PMA Product Marketing Framework.**

**The goal of Get Set is to turn positioning and strategy into launch-ready execution.**

- Strategize decides what the business will do and why
- Define decides how the market should understand it
- Get Set answers: What exactly needs to be built before launch? Who needs to be ready, trained, and aligned? Which assets, approvals, and handoffs must be complete? How do we know we're actually ready — not just busy?

**A strong Get Set phase does four things well:**
1. Operationalizes the strategy into assets, workflows, and deliverables
2. Builds commercial readiness so the field can actually sell and support the offer
3. Creates launch discipline through milestones, approvals, and stage gates
4. Improves launch quality by ensuring handoffs are complete and usable

**The PMM's role:** operator, orchestrator, and quality bar owner. Not content factory, not project manager for every function. The job is to ensure the organization can tell, sell, deliver, and measure the launch.

**The core test for Get Set completion:** If the PMM disappeared for 72 hours before launch, could the business still launch cleanly because the plan, assets, owners, approvals, and escalation paths are all clear? If no — Get Set is not done.

**The best PMMs treat Get Set as a readiness system, not a content production scramble.**

---

## Engagement modes

- **Build mode** — Working at or for this company. All 12 steps apply. Access to internal teams, CRM, pricing systems, and field feedback.
- **Job hunt mode** — Targeting this company as a prospective employer. Build a hypothetical launch readiness plan: identify what assets a launch would need, what enablement gaps likely exist, what the governance model should look like, based on public information about their product, sales model, and customer base. Flag all assumptions ⚠️ **Job Hunt Mode**. This demonstrates operational PMM maturity to interviewers.

---

## The 12 Get Set steps

### Step 1 — Establish launch scope, tier, and readiness criteria

Before building anything, confirm the scale of the launch and define what "ready" actually means. Not every release deserves the same effort level — if everything is treated as Tier 1, the team burns out and quality falls.

**Launch tier model:**
- **Tier 1 — Major launch:** High revenue or strategic impact. Full campaign, executive alignment, PR, broad field enablement, robust measurement.
- **Tier 2 — Important launch:** Focused GTM motion, selective enablement, key assets, moderate campaign support.
- **Tier 3 — Maintenance / low-impact release:** Lightweight updates, self-service documentation, minimal coordinated launch motion.

**Readiness categories to define for the chosen tier:**
- Product readiness
- Messaging readiness
- Commercial readiness
- Field readiness
- Customer readiness
- Measurement readiness

**Templates:** Launch tiering framework, Launch brief/charter, Readiness criteria checklist, Stage-gate framework, PMA Launch Tiers (coda.io/@product-marketing-alliance-pma).

**Key outputs:** Launch tier recommendation, Launch brief/charter, Readiness definition, Stage-gate criteria.

**Good:** Company knows what kind of launch this is; effort matches strategic importance; minimum launch bar is shared; everyone knows what must be done before greenlighting.
**Weak:** Every launch treated as urgent and critical; no shared readiness bar; launch date fixed before quality is assessed; teams confuse activity with readiness.

---

### Step 2 — Turn strategy into a detailed launch plan

Translate strategy and messaging into a concrete execution plan with owners, milestones, dependencies, and deliverables.

**Workstreams to plan across:**
Product, web/content, demand gen, sales enablement, CS/support, lifecycle/customer comms, partner/channel, legal/compliance, operations/analytics.

**Explicit milestone categories:**
- Strategy frozen
- Messaging approved
- Asset build complete
- Field enablement complete
- Launch QA complete
- Go/no-go checkpoint

**Workback sequencing from launch date:** asset deadlines → review cycles → training date → QA/compliance signoff → web deployment date → pricing/SKU readiness → CRM/reporting configuration.

**Templates:** Launch project plan, Workback schedule, Cross-functional launch tracker, Dependency tracker, RACI/DACI, Decision log, PMA Launch Checklist (coda.io/@product-marketing-alliance-pma), PMA Internal Roadmap Template.

**Key outputs:** Integrated launch plan, Workback timeline, Cross-functional ownership map, Dependency and escalation tracker.

**Good:** Actionable plan, not just presentational; owners and due dates clear; dependencies visible early; PMM proactively managing blockers.
**Weak:** Launch deck exists but no operational plan; tasks vague or ownerless; teams find out about deadlines too late; PMM becomes reactive traffic manager.

---

### Step 3 — Translate positioning into asset requirements and content briefs

Positioning doesn't automatically become usable assets — teams need structured briefs and clear translation guidance, not "here's the messaging doc, go build."

**For each asset, define:**
- Primary audience
- Use case it serves
- Message pillar it supports
- Proof point it demonstrates
- CTA
- Channel/placement
- Owner and deadline

**Typical assets to scope by tier:**

*Digital/web:* website pages, landing pages, in-app messaging, product tour.
*Campaign:* launch blog post, product announcement copy, email sequences, ad/social copy, webinar messaging.
*Sales:* pitch deck/narrative slides, demo talk track, one-pager, battlecard.
*Customer-facing:* customer FAQs, release notes, customer communications, onboarding materials.
*Internal:* internal FAQ, executive talking points, PR/analyst brief (if relevant).

**Templates:** Content brief template, Message-to-asset mapping worksheet, Asset prioritization list, Web page brief, Campaign brief, Customer communications brief, Executive narrative brief.

**Key outputs:** Prioritized asset list, Content and creative briefs, Message-to-asset map, Copy guidance and source language.

**Good:** Every key asset has a clear purpose and brief; content teams know what message to lead with; assets align to audience and funnel stage; PMM reduces rewrites by being precise upfront.
**Weak:** Teams build from their own interpretation; messaging consistency breaks immediately; too many low-priority assets created; asset creation starts without briefs.

---

### Step 4 — Build sales readiness and field enablement

A launch is not ready because a deck exists. It is ready when the field can confidently pitch, qualify, demo, position, handle objections, and progress deals.

**Sales readiness rubric — can reps:**
- Explain the problem?
- Identify the right ICP?
- Connect messaging to business value?
- Handle likely objections?
- Articulate packaging/pricing clearly?
- Recognize when *not* to pitch it?

**Readiness milestone model (stronger than "training delivered"):**
1. Enablement content created
2. Training session delivered
3. Key teams attended
4. Field knowledge checked
5. Managers reinforced in pipeline review or role-play
6. Adoption monitored in calls/deals

**Enablement deliverables by type:**

*Core:* Sales narrative / talk track, pitch deck or storyline slides, battlecard, objection handling guide, discovery questions, qualification criteria.
*Supporting:* Use-case cheat sheet, competitive comparison guidance, pricing/packaging explanation, demo flow guidance, internal FAQ.

**Templates:** Sales enablement plan, Readiness checklist, Sales play template, PMA Battlecard Template (coda.io/@product-marketing-alliance-pma), Objection handling framework (PMA Objection Handling Script), Demo talk track template, Discovery question guide, FAQ template, Certification/knowledge-check template, PMA Sales Playbook Template, PMA Sales One-Pager.

**Key outputs:** Field enablement plan, Sales readiness assets, Training sessions, Readiness completion status, FAQ/objection handling set.

**Good:** Sales agrees the offer is pitchable; reps know when and how to use the story; enablement tied to actual sales moments; PMM measures readiness not just attendance.
**Weak:** Enablement is a one-time presentation; assets generic and too polished to be practical; reps unclear on qualification, pricing, or objections; PMM assumes "shared = adopted."

---

### Step 5 — Prepare customer success, support, and post-sale teams

Many launches fail after the sale because post-sale teams were informed, but not equipped.

**What CS, onboarding, support, and account teams need:**
- What's changing and who gets access
- Expected customer questions and known limitations
- Launch caveats and escalation paths
- Adoption talking points and renewal/expansion messaging guidance

**Useful deliverables:**
- Customer rollout email copy
- Support macros
- Adoption talking points
- Implementation notes
- Customer-facing FAQ
- Known limitations list
- "What changed" explainer
- Renewal/expansion messaging guidance

**Templates:** CS enablement brief, Support FAQ, Onboarding guide, Release communication plan, Internal support readiness checklist, Customer issue escalation framework, PMA Customer Onboarding Template (coda.io/@product-marketing-alliance-pma).

**Key outputs:** CS and support readiness package, Customer communication plan, Adoption guidance, Issue escalation and support notes.

**Good:** CS/support can explain the release simply; post-sale teams know how to set expectations; adoption and retention risks anticipated; customers get a smoother experience.
**Weak:** Support sees the release at the same time as customers; CS gets vague messaging with no practical guidance; teams unprepared for objections; launch treated as pre-sale only.

---

### Step 6 — Finalize offer, packaging, pricing, and commercial mechanics

Get Set is where commercial complexity must be resolved, not deferred. Strong messaging and demand gen will fail if commercial details are unclear.

**Key questions to resolve:**
- Can the product actually be sold in systems today?
- Are quote-to-cash workflows ready?
- Can field teams explain packaging simply?
- Are contractual/legal issues resolved?
- Is there clarity on grandfathering, migration, bundling, or entitlements?

**Partner with:** product, finance, rev ops, and sales leadership to confirm: pricing, package names, plan inclusions/exclusions, SKUs/billing setup, discount guidance, contract/legal language, sales process implications, internal ordering and quoting mechanics.

**Templates:** Commercial readiness checklist, Offer mechanics brief, Pricing/packaging FAQ, SKU readiness tracker, Sales process update brief, PMA Guide to Pricing Models (coda.io/@product-marketing-alliance-pma).

**Key outputs:** Commercial readiness signoff, Pricing and packaging FAQ, Internal offer mechanics guide, SKU/system readiness confirmation.

**Good:** Pricing and packaging final before launch; sales ops and field know how to transact; PMM can explain the offer in customer language; no surprise commercial blockers at launch.
**Weak:** GTM starts before billing/logistics are ready; price guidance changes late; packaging confusing internally and externally; reps cannot confidently quote or position.

---

### Step 7 — Build the internal communications plan

A high-quality launch requires internal clarity before external activity.

**Tailor communications by audience:**
- Execs: strategic rationale, business goals, what to watch for
- Sales: what's new, how to pitch it, what changed in the process
- CS/support: what customers will experience, how to handle questions
- Marketing: campaign timing, channel coordination, what's live when
- Product: what's shipping, known limitations, feedback loops
- Regional teams/partners: what applies to them, timing differences

**Complete handoff principles — a handoff is not complete just because a deck was shared, a file exists, or a meeting happened. A complete handoff answers:**
- Is this final or still changing?
- What is approved vs. under review?
- What changed from the last version?
- What assumptions should the next team work from?
- Who owns follow-up if new issues emerge?

**Templates:** Internal communications plan, Stakeholder map, Launch announcement template, Change log, Single source of truth doc, Handoff checklist.

**Key outputs:** Internal comms plan, Single source of truth, Stakeholder updates, Structured handoff package, Change log/decision log.

**Good:** Stakeholders aligned and not surprised; receiving teams know exactly what to do next; version control clear; PMM reduces back-and-forth by making handoffs complete.
**Weak:** Context lives in one person's head; teams ask the same questions repeatedly; different regions work from different versions.

---

### Step 8 — Operationalize launch governance and stage gates

Strong PMM functions separate themselves from ad hoc launch culture by moving through explicit gates, not vibes.

**Recommended 5-gate model:**

| Gate | Name | What's confirmed |
|---|---|---|
| Gate 1 | Strategy sync | Validated customer pain, target audience agreed, GTM rationale aligned |
| Gate 2 | Messaging approval | Positioning approved, core messages finalized, sales says it is pitchable |
| Gate 3 | Commercial readiness | Pricing, SKU, legal, packaging finalized; systems updated; support processes in place |
| Gate 4 | Launch readiness / go-no-go | Core assets built, web/email/comms ready, field enabled, metrics/tracking live, top risks mitigated |
| Gate 5 | Post-launch review | 30/60-day impact review, adoption/revenue/pipeline assessment, lessons learned |

**Templates:** Governance model doc, Stage-gate checklist, Go/no-go decision memo, Launch review agenda, Launch risk review template.

**Key outputs:** Launch governance model, Stage-gate checklist, Go/no-go recommendation, Approval record.

**Good:** Readiness is explicit and auditable; PMM can confidently recommend go/no-go; stakeholders know what approval means; launches become less chaotic over time.
**Weak:** No one knows who can delay launch; checkpoints are status meetings with no decisions; risks raised but not resolved; launches happen because the date arrived.

---

### Step 9 — QA messaging, assets, and customer experience

PMM acts as the final quality-control layer across message consistency and customer experience before launch. Not about reviewing every comma — about ensuring the launch feels coherent.

**QA inspection areas:**
- Does homepage story match sales talk track?
- Does in-product language reflect approved terminology?
- Are customer emails clear on timing, access, limitations?
- Do support docs match the launch announcement?
- Are we overclaiming vs. actual product readiness?
- Is naming consistent across all channels?
- Are CTAs appropriate for the audience?
- Is proof claimed accurate and supportable?

**Templates:** Launch QA checklist, Messaging consistency checklist, Web/campaign review rubric, Customer experience walkthrough checklist, Claim verification worksheet.

**Key outputs:** QA findings log, Final launch corrections, Message consistency signoff, Customer experience review summary.

**Good:** Launch feels integrated across touchpoints; claims accurate; customer experience smooth from announcement through onboarding; PMM catches drift before it reaches the market.
**Weak:** Every channel tells a slightly different story; terminology inconsistent; launch copy overpromises; customer confusion predictable but unaddressed.

---

### Step 10 — Set up measurement, tracking, and feedback loops

A launch is not ready if you cannot measure whether it worked. Measurement setup belongs in Get Set, not after launch.

**Metrics to operationalize (select by launch type):**
Influenced pipeline, sourced pipeline, win rate, feature adoption, activation, usage depth, retention/expansion, traffic and conversion, trial/demo volume, enablement completion and adoption, support ticket themes, customer sentiment.

**Feedback loops to configure:**
- Sales feedback form (quick post-call input on message resonance, objections encountered, prospect questions)
- CS feedback channel (post-onboarding experience signals)
- Qualitative review cadence (weekly for first 30 days, then monthly)

**Templates:** Launch measurement plan, KPI scorecard, Dashboard requirements doc, Sales feedback form, Post-launch insights tracker.

**Key outputs:** Measurement plan, Dashboard/reporting requirements, Baseline + targets, Feedback collection mechanism.

**Good:** PMM knows what will be measured and how; reporting ready on day one; leading and lagging indicators separated; sales and CS have a quick way to submit real-world feedback.
**Weak:** Team decides metrics after launch; no one owns reporting; activity metrics dominate; feedback comes through anecdotes only.

---

### Step 11 — Run launch readiness reviews and close gaps

PMM synthesizes everything and makes the call: are we genuinely ready?

**Readiness scorecard — assess red/yellow/green for each dimension:**
- Product readiness
- Message readiness
- Field readiness
- Commercial readiness
- Support readiness
- Campaign/web readiness
- Measurement readiness

**When issues are found, make trade-off recommendations:**
- Delay a specific asset
- Reduce launch scope
- Sequence rollout by audience or region
- Gate access for certain customer tiers
- Soften a specific claim
- Accept known risk with explicit sign-off

**Templates:** Launch readiness scorecard, RYG status tracker, Go/no-go checklist, Issue log, Launch blocker escalation form.

**Key outputs:** Readiness review, RYG scorecard, Go/no-go recommendation, Final issue resolution plan.

**Good:** Readiness reviewed holistically; PMM can articulate launch risk clearly; scope decisions made intentionally; teams enter launch with fewer surprises.
**Weak:** Readiness reviews performative; teams hide risk to avoid delays; no one makes hard trade-offs; launch proceeds with unresolved fundamentals.

---

### Step 12 — Prepare the final handoff into launch execution

Get Set ends when execution teams can move quickly without reopening foundational questions.

**Launch-day command structure must define:**
- Who owns issues in real time during launch week
- Response paths for: customer confusion, field escalation, content changes, system issues
- Who can authorize scope changes or delays
- Single source of truth for launch-day assets

**Templates:** Launch handoff package, Launch day run-of-show, Command center doc, Issue escalation matrix, Final approvals checklist.

**Key outputs:** Final handoff package, Launch day runbook, Owner list/escalation paths, Execution-ready source of truth.

**Good:** Launch-week execution smoother because ambiguity is low; teams know who owns issues in real time; handoff enables action without repeated clarification.
**Weak:** Launch-day questions expose unfinished decisions; teams scramble for final files and approvals; ownership unclear; PMM answering preventable questions all week.

---

## Get Set readiness checklist

**Launch design:**
- [ ] Right launch tier assigned?
- [ ] Launch scope clear?
- [ ] Readiness definition shared with all teams?

**Planning:**
- [ ] Integrated launch plan with owners and deadlines?
- [ ] Dependencies visible?
- [ ] Critical path and escalation path defined?

**Asset creation:**
- [ ] Right assets prioritized?
- [ ] Every major asset has a clear brief?
- [ ] Messages consistent across channels?

**Sales readiness:**
- [ ] Talk track, proof, and objection guidance ready?
- [ ] Enablement delivered?
- [ ] Actual field readiness validated (not just attendance)?

**Customer readiness:**
- [ ] CS, onboarding, and support prepared?
- [ ] Customer communications ready?
- [ ] Expected questions, limitations, and escalation paths documented?

**Commercial readiness:**
- [ ] Pricing, packaging, SKUs, legal terms, and systems finalized?
- [ ] Field can actually transact?
- [ ] Offer easy to explain?

**Governance:**
- [ ] Stage gates and go/no-go criteria defined?
- [ ] One source of truth exists?
- [ ] Handoffs complete and documented?

**QA and measurement:**
- [ ] All core touchpoints checked for consistency and accuracy?
- [ ] Measurement configured before launch?
- [ ] Plan to gather field and customer feedback quickly?

**Launch handoff:**
- [ ] Execution teams know what happens on launch day?
- [ ] Ownership clear during launch week?
- [ ] Final unresolved issues addressed or formally accepted?

---

## Core Get Set document structure

| Section | Contents |
|---|---|
| 1. Executive summary | What is launching, why it matters, launch tier, launch date/scope |
| 2. Objectives and success criteria | Launch goals, key metrics, readiness definition |
| 3. Audience and message summary | Target segments, core messaging, key use cases, message guardrails |
| 4. Workstreams and deliverables | Content/web, sales enablement, CS/support, customer comms, campaign/channel, ops/analytics, legal/commercial |
| 5. Asset plan | Required assets, owners, due dates, approval status |
| 6. Readiness plan | Training plan, stakeholder communication, support readiness, internal launch comms |
| 7. Commercial readiness | Pricing, packaging, SKUs, systems/process updates |
| 8. Dependencies and risks | Blockers, assumptions, mitigation plans, escalation path |
| 9. Governance | Stage gates, checkpoint meetings, go/no-go criteria, decision owners |
| 10. Measurement and feedback | KPI tracking, dashboard setup, feedback loop design, review cadence |
| 11. Launch-day plan | Run-of-show, owner matrix, escalation contacts, contingency actions |

---

## What good vs. weak Get Set looks like

**Good Get Set work is:**
- Operationally rigorous, not ad hoc
- Cross-functional, not PMM-only
- Milestone-driven, not just deadline-driven
- Quality-controlled, not content-chaotic
- Enablement-led, not asset-led
- Readiness-based, not optimism-based
- Explicit about handoffs, owners, and approvals
- Realistic about constraints and trade-offs

**Weak Get Set work tends to be:**
- A flurry of asset requests with no prioritization
- Over-dependent on heroic last-minute effort
- Vague on ownership
- Weak on commercial and support readiness
- Focused on launch day, not launch readiness
- Based on deck-sharing rather than capability-building
- Inconsistent across channels and teams
- Missing governance, measurement setup, and QA discipline

---

## Common mistakes to avoid

1. Treating Get Set as asset creation only
2. Starting execution before readiness criteria are defined
3. Overproducing low-value assets
4. Underinvesting in sales and CS readiness
5. Confusing enablement with a single training session
6. Allowing incomplete handoffs between teams
7. Leaving pricing/SKU/legal mechanics unresolved too late
8. Skipping launch QA
9. Not setting up measurement before launch
10. Running status meetings with no real decisions
11. Letting launch date pressure override launch quality
12. Failing to define what is "must-have before launch" vs. "can follow post-launch"

---

## Template toolkit

**Essential:**
- Launch brief/charter, Launch tiering framework, PMA Launch Tiers
- Workback plan / integrated project plan
- Cross-functional RACI or DACI
- Dependency tracker
- Content brief template, Message-to-asset mapping worksheet
- Sales enablement plan
- PMA Battlecard Template, Objection Handling Script, Sales Playbook Template, Sales One-Pager
- FAQ template
- Customer communications brief
- Internal communications plan
- Commercial readiness checklist
- Launch QA checklist
- Launch readiness scorecard
- Go/no-go checklist
- Measurement plan
- Handoff checklist
- PMA Launch Checklist (coda.io/@product-marketing-alliance-pma)
- Launch day runbook

**Optional but valuable:**
- Certification quiz/knowledge check
- Demo narrative template
- Support macro guide
- Executive briefing doc
- Regional localization checklist
- Partner launch kit
- Issue escalation matrix
- Post-launch review template

---

## Downstream skills this feeds into

Get Set outputs directly enable:
- **PMM Grow** — uses the KPI framework, measurement plan, feedback loops, and launch baseline to track post-launch performance, adoption, and optimization opportunities

---

## Reference frameworks

**Primary (structural backbone):**
- PMA Product Marketing Framework — Get Set phase
- PMA Launch Checklist (coda.io/@product-marketing-alliance-pma)
- PMA Launch Tiers
- PMA Internal Roadmap Template
- PMA Battlecard Template
- PMA Sales Playbook Template
- PMA Objection Handling Script
- PMA Sales One-Pager
- PMA New Product Project Planner
- PMA Customer Onboarding Template
- PMM-GPT best practice guidance (PMA, 2026)

**Secondary (philosophical lens):**
- MKT1 / Emily Kramer — enablement as "showing how the product fits into the audience's full workflow," not just explaining features
- SVPG / Martina Lauchengco (Loved) — launch readiness as a shared PMM/PM accountability, not a handoff
