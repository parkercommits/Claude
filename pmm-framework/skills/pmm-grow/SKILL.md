---
name: pmm-grow
description: "This skill should be used when the user wants to \"analyze the post-launch performance\", \"run the Grow phase\", \"help me understand what's driving adoption\", \"build the post-launch review\", \"what's working / not working since launch\", \"diagnose our funnel performance\", \"collect and synthesize customer feedback\", \"refresh our enablement based on what we've learned\", \"identify new segments or expansion opportunities\", or \"run the 30/60/90-day review\". Executes the PMA Grow phase: 12 steps covering learning agenda, KPI measurement, adoption analysis, VOC synthesis, message-market fit, funnel diagnosis, onboarding optimization, segment expansion, product feedback, proof collection, enablement refresh, and post-launch reviews with traffic-light decisions and quarterly updates to the Context Document.\n"
metadata:
  version: "0.4.0"
  author: "Parker Lyons"
---

# PMM Grow Skill

## Trigger conditions
Invoke this skill when the user says any of the following (or close variants):
- "Analyze the post-launch performance for [product]"
- "Run the Grow phase"
- "Help me understand what's driving adoption"
- "Build the post-launch review"
- "What's working / not working since launch?"
- "Diagnose our funnel performance"
- "Collect and synthesize customer feedback"
- "Refresh our enablement based on what we've learned"
- "Identify new segments or expansion opportunities"
- "Help me run the 30/60/90-day review"
- "Build the voice-of-customer synthesis"
- Any request to measure, analyze, optimize, or learn from a product that is already in market

**Prerequisite:** The product, feature, or offer should be live in market with some measurable activity. The Grow phase requires: KPO goals, big bets, and ranked revenue levers from Strategize ("Strategy on a page"); messaging and perceptions from Define; and the launch baseline, GACCS brief, and 30/60/90-day momentum plan from Get Set. If post-launch measurement wasn't configured, start by establishing what data is available and what the learning agenda should be.

---

## Framework & philosophy

This skill executes the **Grow phase of the PMA Product Marketing Framework.**

**The goal of Grow is to turn a launch into a repeatable, optimizable growth engine.**

- Strategize decides where to play and how to win
- Define creates the market story
- Get Set makes the business launch-ready
- Grow answers: What happened once the product hit the market? What's driving adoption, conversion, retention, and expansion? What should we optimize, fix, double down on, or stop? How do we turn launch learning into sustained commercial momentum?

**This is not a "post-launch clean-up" phase. It is a continuous operating loop of analysis, optimization, feedback, and iteration.**

**A strong Grow phase does five things well:**
1. Measures impact against the goals set earlier
2. Surfaces insight from quantitative and qualitative signals
3. Improves adoption and revenue performance through targeted optimization
4. Closes the loop with product, marketing, sales, and CS
5. Builds the evidence base for stronger future launches, messaging, and expansion motions

**The core test for Grow maturity:** Can the PMM team clearly explain which customer behaviors lead to value, which GTM motions drive adoption and revenue, and what three changes would most improve growth in the next quarter? If no — Grow is not mature yet.

**Make the call (MKT1).** Grow exists to decide what to **scale, improve, pause, or stop** — not to report. Every review ends in those calls, using the traffic-light review in Step 12.

---

## Engagement modes

- **Build mode** — Working at or for this company. All 12 steps apply. Access to product analytics, CRM data, call recordings, customer interviews, and CS feedback.
- **Job hunt mode** — Targeting this company as a prospective employer. Build a hypothetical Grow analysis using public signals: product reviews, G2/Capterra feedback themes, public case studies, competitor comparisons, community discussions. Demonstrate what you'd measure, what you'd hypothesize, and what optimizations you'd investigate. Flag all as hypotheses ⚠️ **Job Hunt Mode**. This is especially powerful for senior PMM roles.

---

## Inputs and connections

Start from the **Engagement setup**, the Get Set section (GACCS brief, momentum plan, baseline), and earlier sections of the Context Document. Re-check which tools are connected (see `skills/pmm-director/references/connections.md`). If MKT1 tools (`mkt1_*`) are connected, use them for the steps that name one, following `skills/pmm-director/references/mkt1-tools.md`. Grow depends on data more than any other phase — say plainly which analyses can't be done without a connection.

**MKT1 tools in Grow:** `mkt1_aeo_audit` checks how AI answer engines find and describe the company (Step 5); `mkt1_incognito_competitive_research` repeats the outside view from Discover; `mkt1_linkedin_posts_analysis_beta` analyzes a LinkedIn account's own analytics export (Step 11). Grow doesn't hand a whole step to a tool — it uses these as inputs.

### Company profile and existing work (build mode)

If the team has a company profile (created by `pmm-setup`), read sections 0 (Health check summary), 7 (GTM plan — goals and big bets), 8 (Teams, tools, and processes — feedback loops), and 9 (Customer voice) before starting, and skip any question they already answer. If section 8 lists frameworks or experts the team has adopted for this kind of work, use their structure and vocabulary, mapped onto this phase's steps (see "When sources disagree" in the Director).

**Audit before you build.** If the team already has existing dashboards, VOC reports, win/loss programs, and earlier post-launch reviews, start from them. Build on the team's existing reports and cadence rather than creating a parallel one, and compare against the goals in section 7.

**Propose profile updates; don't make them silently.** When this phase produces something durable — customer voice themes, ICP tier moves, perception statuses, and a re-scored health check (see Step 12) — show the proposed change to the section owner and add a change-log line once they agree. If there's no profile, suggest `pmm-setup` once, then continue without it.

### Where each input comes from

| Input | Job hunt mode — where it comes from | Build mode — where it comes from |
|---|---|---|
| Pipeline, win rate, campaign influence | — (hypothesize what you'd measure) | **CRM** — lifecycle stages, campaign influence, closed-won/lost since launch |
| Adoption, activation, retention | Public usage claims, reviews mentioning onboarding | **Product analytics** — activation, feature adoption, retention cohorts |
| Customer feedback themes | Review sites, community threads since launch | **Support and feedback** — ticket and survey themes; **call recordings** — post-launch calls |
| Message and perception pull-through | Reviews, social posts, analyst commentary | **Call recordings** — language prospects repeat back; **web analytics** — page conversion |
| Content performance | Visible engagement on public content | **Web and marketing analytics** — traffic, conversion, influenced pipeline by asset |
| Product feedback | Feature requests in reviews and communities | **Roadmap and issues** — customer-requested issues and their status |

Pull the review period's data only (e.g., the 30, 60, or 90 days since launch), compare against the Get Set baseline, and cite the tool and date range. Ask before creating issues or posting findings anywhere. Follow the guardrails in `skills/pmm-director/references/connections.md`.

---

## The 12 Grow steps

### Step 1 — Establish a post-launch learning agenda

The biggest Grow mistake is entering post-launch without clarity on what you're trying to learn. Analysis without a learning agenda produces data, not decisions.

**Define the questions that matter most across four categories:**
- Business outcome questions (is revenue/adoption/retention performing?)
- Market understanding questions (are the right customers buying? are segments behaving as expected?)
- Product experience questions (are customers using it as intended? where do they stall?)
- Commercial execution questions (are messages landing? are sales plays working?)

**Start from the plan, not a blank page.** Pull the questions from what earlier phases committed to:
- Each **big bet's** success criteria (Strategize)
- The **project and ops goals**, not just the KPIs
- The **revenue lever** the launch was meant to move
- The **GACCS launch brief** goal and the **30/60/90-day momentum plan** (Get Set) — did the momentum plan actually run?
- The **perceptions** the launch was meant to support (Define)

**Strong learning question examples:**
- Are we attracting the ICP we expected?
- Which perception is taking hold, and which is lagging?
- Which ecosystem partners, creators, or customers actually drove pipeline?
- Which use cases convert fastest?
- Where in onboarding do users stall?
- Which persona responds best to the value prop?
- Which objections are increasing in late-stage deals?
- Are customers using the product the way we positioned it?
- Are there unexpected segments showing strong pull?

**Templates:** Post-launch learning agenda, Hypothesis tracker, Growth phase goals brief, Questions-to-answer worksheet.

**Key outputs:** Post-launch learning agenda, Growth hypotheses list, Priority analysis questions.

**Good:** PMM is explicit about what the business wants to learn; analysis tied to decisions; team knows which insights would trigger action.
**Weak:** Post-launch analysis unfocused; lots of metrics, few important questions answered; no link between insight and optimization.

---

### Step 2 — Measure performance against success metrics

Don't just report performance — interpret it. Explain what is happening, why it may be happening, what it implies, and what should happen next.

**Leading indicators** (tell you whether momentum is building):
Traffic, CTR, demo requests, activation, trial starts, onboarding completion, feature engagement, enablement participation.

**Lagging indicators** (reflect commercial outcomes):
Revenue, pipeline, win rate, retention, expansion, churn, NRR, customer lifetime value.

**Always segment results by:** persona, segment, industry, region, acquisition source, lifecycle stage, sales motion, cohort, use case, plan/package. Aggregate data masks segment-level truth.

**Interpretation principle:** A launch with strong awareness but poor activation has a different problem than one with weak awareness but strong downstream conversion. PMM should identify which part of the funnel the issue lives in.

**Measure for learning, not credit (MKT1).** Attribution exists to show what works, not to decide which team gets credit. Common startup mistakes: too little reporting, fighting over credit, judging channels in isolation, and over-relying on first-touch ("original source") attribution — which in account-based GTM often just reflects list building. Instead:
- **Lifecycle stages for contacts and accounts** — track volume (or value) at each stage, conversion between stages, and time between stages
- **Capture the last touch before a meeting or opportunity** — what moved the deal forward matters more than how the record entered the system
- **Campaign influence reporting** — every campaign a contact or account engaged with before or during the sales process, and the pipeline and revenue it influenced. Campaigns span channels, and one deal is often influenced by several.
- **Blended CAC** — total acquisition spend across marketing, sales, and partnerships divided by new customers, rather than per-channel CAC
- **Report inbound and outbound separately** — they move through the funnel differently
- **Don't label pipeline "marketing-sourced" vs. "sales-sourced"** — use neutral stage names and focus on what moves deals
- Use several views (first touch, last touch before qualification, campaign influence); a complex multi-touch model is usually overkill at early stages
- **Account-stage progression for events and partner campaigns** — these are rarely the first or last touch, so measure whether target accounts moved (unaware → engaged → evaluating → in pipeline), not just sourced pipeline
- **Conversion by source at every stage** — a funnel that leaks between stages wastes the top of it; track conversion goals by source from first touch to closed-won

**Efficiency metrics** — when the launch targeted the efficiency lever, track the three MKT1 efficiency metrics: **CAC ratio, payback period, LTV:CAC**. Agree on standard definitions with finance first.

**Report to sales in their terms:** pipeline, meetings, win rate, deal velocity — not impressions or MQLs.

**Templates:** Growth KPI dashboard, Campaign influence report, Lifecycle stage report, Account-stage progression report, Full-funnel conversion calculator, Blended CAC and efficiency metrics sheet (MKT1's Marketing budget & efficiency metrics), Bottom-up forecast (by accounts or leads), Marketing ops checklist (the tracking needed for full-funnel reporting), Post-launch scorecard, Cohort analysis template, Funnel performance tracker, Segment performance review deck.

**Key outputs:** Performance dashboard, Post-launch metrics review, Leading/lagging indicator analysis, Segment and cohort insights.

**Good:** Metrics reported in a decision-oriented way; trends segmented; data interpreted through the lens of GTM, messaging, product, and customer behavior.
**Weak:** Metrics shared without interpretation; vanity metrics dominate; no baseline or targets; performance reviewed only in aggregate.

---

### Step 3 — Analyze product adoption and usage behavior

This is where PMM becomes a bridge between market promise and customer reality — learning whether customers are using the product as expected, where they drop off, and which behaviors correlate with long-term value.

**Adoption maturity model — segment customers into stages:**
Aware but inactive → Activated → Early adopter → Habitual user → Power user → Expansion-ready → At-risk.

**Activation framework — define:**
- The moment a user first experiences meaningful value
- Behaviors that indicate successful onboarding
- The gap between sign-up/purchase and first value realization

**Adoption funnel breakdown — map drop-off at each stage:**
Acquired → Onboarded → Activated → Repeat usage → Value realized → Retained → Expanded.

**Partner with:** product, analytics, lifecycle, and CS to answer: Who is adopting and who is not? What features/workflows are used most? What actions indicate activation? What behaviors correlate with retention or expansion? Where is friction highest?

**Templates:** Adoption analysis template, Activation funnel map, Usage cohort tracker, Time-to-value analysis worksheet, Feature adoption report.

**Key outputs:** Adoption analysis, Activation definition and metrics, Feature/use-case usage insights, Retention driver hypotheses, Friction point summary.

**Good:** PMM understands what usage actually drives value; adoption goes beyond "logins"; product and GTM teams align on activation definition; PMM can identify where growth is blocked.
**Weak:** Adoption measured only by account count; no agreed definition of "activated"; PMM can't connect messaging promises to actual product behavior.

---

### Step 4 — Gather and synthesize qualitative customer feedback

Quantitative data shows what is happening. Qualitative feedback explains why. Build a deliberate feedback engine — not just random Slack anecdotes.

**Feedback sources to tap:**
Customer interviews, onboarding conversations, support tickets, implementation reviews, CSMs and account managers, sales call recordings, win/loss insights, NPS open-text, customer advisory boards, community discussions.

**Theme coding model — tag feedback by:**
Desired outcome, implementation friction, onboarding confusion, missing capability, competitive comparison, value realization, pricing/packaging confusion, messaging confusion, feature request, delight moment.

**Focus on understanding:**
- What customers expected vs. what they actually experienced
- Where confusion emerged
- What nearly prevented adoption
- Which value moments mattered most
- What language customers use once they understand the product
- Where perception and reality differ

**Templates:** Customer interview guide, Post-launch feedback synthesis template, Voice-of-customer tracker, Feedback tagging framework, Support/theme analysis worksheet, PMA Customer Case Study Questions (coda.io/@product-marketing-alliance-pma), PMA Win/Loss Email Templates.

**Key outputs:** Voice-of-customer synthesis, Thematic feedback report, Top friction themes, Customer language updates, Insight recommendations for GTM and product.

**Good:** PMM synthesizes patterns not isolated quotes; feedback organized into themes that drive action; customer voice influences messaging, onboarding, and roadmap; PMM distinguishes isolated complaints from repeated structural issues.
**Weak:** Customer feedback anecdotal and unstructured; loudest internal opinions outweigh actual patterns; insights collected but not turned into action.

---

### Step 5 — Evaluate message-market fit and narrative performance

A product launch doesn't mean the messaging is working. Grow is where PMM assesses whether buyers understand the value prop, the right messages are resonating, claims are believable, and differentiation is landing.

**Assess messaging performance across:**
Website conversion, campaign engagement, sales call language, objection frequency, win/loss feedback, demo response, customer interviews, field feedback, copy tests, persona-specific conversion patterns.

**Message resonance testing — evaluate messages against:**
Clarity, relevance, distinctiveness, credibility, motivation.

**Sales call review analysis — identify:**
Where prospects lean in, what they ask about, what they misunderstand, what language reps actually use successfully.

**Track perceptions (MKT1).** Define set 3–4 perceptions with a status (not yet driven / emerging / strong). Check each one:
- Are prospects, customers, analysts, and partners repeating it back — in calls, reviews, social posts, community threads?
- Is its status moving (not yet driven → emerging → strong)? Update the status with evidence.
- Which perception is lagging, and what content or campaign would move it?
- Is content still laddering up to the perceptions, or drifting?

**Check what AI answer engines say.** More buyers now ask an AI assistant before they visit a website. Ask the major assistants the questions the primary audience asks ("best tools for…", "[company] vs [competitor]") and note whether the company appears, how it's described, and which outside pages the answers draw on. Check basics that hide a site from AI crawlers: hero copy that only appears after JavaScript runs, missing structured data, and crawler blocks. Re-check after every significant web change. **With MKT1 tools:** run `mkt1_aeo_audit` for the full technical pass and a prioritized fix list.

**Key questions:**
- Are customers repeating our language back to us?
- Are they repeating our perceptions back to us?
- Which message pillars are resonating?
- Which messages create confusion or skepticism?
- Is the category framing working?
- Are we overleading with features or under-explaining outcomes?

**Templates:** Message performance scorecard, AI answer-engine check, Messaging test plan, Objection frequency tracker, Sales call messaging analysis sheet, Website/campaign copy test brief.

**Key outputs:** Messaging effectiveness review, Message optimization recommendations, Updated pillars/proof/audience angles, Narrative risk areas.

**Good:** PMM identifies which messages drive response vs. which don't; messaging evolves based on evidence; sales and marketing get clearer talk tracks; PMM closes the gap between strategic messaging and market reality.
**Weak:** Messaging treated as fixed after launch; no one tests whether the narrative lands; copy changes happen randomly; reps improvise because the official story doesn't work.

---

### Step 6 — Diagnose funnel friction and commercial blockers

Growth problems often sit outside the product. Diagnose where the GTM motion is underperforming: poor lead quality, low conversion, long sales cycles, pricing confusion, weak champion development, poor onboarding continuity.

**Full funnel to analyze:**
Awareness → engagement → demo/trial → activation → opportunity → close → onboarded → retained → expanded.

Use the lifecycle stage and campaign influence reports from Step 2 to locate leaks — and keep inbound and outbound funnels separate, or conversion rates will mislead.

**Win/loss classification:**
Competitor win, no decision, missing capability, budget, poor fit, value not proven, implementation concern, internal priority shift.

**Funnel leak analysis — at each stage ask:**
Who is progressing? Who is not? What is the biggest reason? What might improve progression?

**Templates:** Funnel diagnosis worksheet, Sales friction tracker, Objection analysis framework, Trial-to-paid analysis sheet, Expansion blocker review, PMA Win/Loss Email Templates (coda.io/@product-marketing-alliance-pma), PMA Sales Confidence Survey Questions.

**Key outputs:** Funnel friction analysis, Commercial blocker summary, Win/loss insight report, Optimization priorities by funnel stage.

**Good:** PMM identifies where growth is breaking and why; recommendations tied to specific funnel stages; no-decision and status-quo losses analyzed.
**Weak:** Funnel issues described vaguely; no distinction between traffic, conversion, qualification, and adoption problems; commercial friction blamed on "market conditions."

---

### Step 7 — Optimize onboarding, activation, and time-to-value

Many launches underperform not because the product lacks value, but because customers don't reach that value fast enough. This is one of the most impactful Grow responsibilities.

**Time-to-value map — track stages:**
Purchase/start → Setup → First key action → First value moment → Repeat value → Habit formation/team adoption.

**Lifecycle messaging framework — define what customers should hear at:**
Purchase, onboarding, activation, adoption maturity, expansion readiness.

**Partner with:** product, lifecycle, onboarding, and CS to improve expectation-setting, first-run experience, implementation guidance, milestone communication, customer education, adoption nudges, expansion readiness.

**Templates:** Onboarding journey map, Time-to-value analysis worksheet, Activation messaging plan, Lifecycle comms framework, Customer milestone map, PMA Customer Onboarding Template (coda.io/@product-marketing-alliance-pma).

**Key outputs:** Onboarding optimization recommendations, Time-to-value improvement plan, Activation messaging updates, Customer milestone communication map.

**Good:** PMM helps align pre-sale promise with post-sale experience; friction points in onboarding identified and improved; teams know which moments matter most for activation.
**Weak:** PMM stops at acquisition; onboarding treated as an ops function only; no visibility into time-to-value; customer expectation gaps create churn risk.

---

### Step 8 — Identify new segments, use cases, and expansion opportunities

Market reality often reveals opportunities the original strategy didn't fully anticipate. Use post-launch insight to discover: unexpected user groups, stronger-than-expected use cases, new industries or regions, expansion triggers, packaging opportunities, cross-sell/upsell motions.

**Signals to look for:**
Unusual adoption concentration, customer-led use-case innovation, high-retention cohorts, sales pull from adjacent segments, expansion behavior by account type, customer language suggesting broader needs, partners or communities driving unexpected demand.

**Express findings as ICP tier moves.** A strong new segment is a candidate to move from Testing → Scaling (or Scaling → Core); a weak one may drop to "Not a priority today." Recommend the tier change explicitly so Strategize can reallocate effort.

**Ecosystem performance.** Review which partners, creators, communities, and customers drove influenced pipeline or adoption. A few strong partners usually beat many transactional ones — recommend where to deepen and where to stop.

**Opportunity prioritization lens:**
Demand signal, strategic fit, ICP overlap, monetization potential, implementation complexity, differentiation potential, enablement complexity.

**Templates:** Segment opportunity assessment, New use-case evaluation worksheet, Expansion motion brief, Opportunity scoring framework.

**Key outputs:** New segment/use-case opportunity list, Expansion recommendations, Adjacent market hypothesis, Follow-on GTM opportunities.

**Good:** PMM spots growth opportunities early; new opportunities evaluated not chased impulsively; expansion recommendations backed by data; product and GTM teams can intentionally decide where to deepen focus.
**Weak:** Emerging usage patterns ignored; every unexpected use case treated as equally important; expansion ideas anecdotal and unprioritized.

---

### Step 9 — Feed insights back into product strategy and roadmap discussions

Grow is where PMM proves strategic value beyond launch execution — bringing disciplined market insight back to product so roadmap decisions are informed by adoption behavior, customer friction, objection patterns, retention drivers, expansion signals, and competitive pressure.

**Opportunity solution framing — for each issue articulate:**
- Customer problem
- Affected segment
- Commercial impact
- Current workaround
- Evidence frequency
- Expected business upside if fixed

**Insight prioritization — rank by:**
Volume/frequency, segment importance, revenue impact, strategic alignment, urgency, workaround severity.

**Templates:** Market insights brief for product, Opportunity-impact framework, Feedback prioritization matrix, Product recommendation memo, Customer friction log.

**Key outputs:** Product feedback synthesis, Roadmap recommendation brief, Commercial impact framing, Prioritized customer problem list.

**Good:** PMM provides structured, commercially informed insight; product receives clear patterns not unfiltered requests; feedback prioritized by impact; PMM influences roadmap through evidence and market context.
**Weak:** PMM forwards random feature requests without synthesis; product sees PMM as anecdotal; commercial implications of friction not quantified.

---

### Step 10 — Collect proof points, customer stories, and case studies

Grow is where the market gives you evidence you didn't have in Define. Continuously strengthen the proof base.

**Rethink the case study (MKT1).** Small edits won't fix the traditional problem → solution → "how we helped" case study. Use customers throughout marketing instead:
- **Build a searchable customer library** — quotes, stats, mini-stories, tagged so sales can answer a prospect's question without waiting for a full case study
- **"Case study, plus"** — from one interview, produce a short write-up for sales requests *and* a video per customer and cross-customer montages
- **Interview first, then pick the format** (video, quote, one-pager, interactive page) based on the story
- **When sales asks for a case study, ask what problem they're solving** — the right asset may be different
- **Bring customers in early** — build them into campaigns and launches, not as a quote added at the end
- **The share test:** would the customer share this with their own audience? A standard case study usually fails it.
- **Amplify customers' own posts** — e.g., boost them as LinkedIn thought-leader ads

**Capture and organize by:** segment, persona, use case, industry, funnel stage, objection type, message pillar, perception supported.

**Types of evidence to collect:**
Customer wins, outcome metrics, implementation success stories, adoption milestones, workflow improvements, ROI evidence, before/after narratives, customer quotes, expansion stories.

**Templates:** Customer library (searchable proof), Case study intake form, Customer proof tracker, Win story template, ROI story worksheet, Referenceability tracker, PMA Customer Case Study Questions (coda.io/@product-marketing-alliance-pma).

**Key outputs:** Proof point library, Case study pipeline, Customer story repository, Reference customer list, Claims strengthening recommendations.

**Good:** PMM continuously upgrades the evidence base; sales and marketing gain real examples; customer stories mapped to strategic use cases and audiences; proof strengthens future messaging.
**Weak:** Customer evidence collected ad hoc; strong stories lost because no system exists; sales asks for case studies PMM hasn't prepared; same generic quote reused everywhere.

---

### Step 11 — Refresh enablement, sales plays, and lifecycle motions based on what's working

Grow is not just analysis — it produces improvements in the field. Once PMM identifies what messages, objections, use cases, and proof points are working, push those learnings back into enablement and execution.

**Update based on Grow findings:**
- Battlecards (new objections, updated competitive intel)
- Talk tracks (what language is actually resonating)
- Demo narratives (which use cases convert best)
- Discovery prompts (better qualification questions)
- Objection handling (new patterns emerging from deals)
- Qualification guidance (ICP refinements)
- Segment and expansion plays
- Customer marketing messaging
- Onboarding and lifecycle communications

**Start field updates with the rep partners.** The one or two reps who helped build the launch enablement are the fastest source of honest feedback on what's working in calls.

**Double down on content that works (MKT1):**
- **Find the hits** — which launch and follow-up assets drove engagement, influenced pipeline, or got shared
- **Repurpose each hit** into more formats (a report → blog posts, social threads, a webinar, a template), each with its **own distribution plan**
- **Make more of what works** before inventing something new
- **Reinforce the perceptions** — keep reusing the core perceptions, frameworks, and concepts across formats. Repetition strengthens the story, even when it feels like a broken record.
- **Plan content against the perceptions** — a content calendar that lists the perceptions and content pillars, then themes by quarter, makes it easy to see which perception is under-served (MKT1's Content strategy & annual planning calendar and Content roadmap). For LinkedIn, use the account's own analytics export to see which hooks, formats, and topics work (`mkt1_linkedin_posts_analysis_beta` when connected).

**Templates:** Enablement update brief, Sales play refresh template, Lifecycle optimization plan, Updated FAQ and objection tracker, Demo narrative revision template, PMA Sales Confidence Survey Questions (to measure impact of updates).

**Key outputs:** Updated field guidance, Revised sales plays, Expansion and retention messaging, Lifecycle communications refinements.

**Good:** Field-facing materials evolve with real-world learning; PMM helps the org get smarter after launch; sales becomes more effective because the story and proof improve.
**Weak:** Enablement materials frozen after launch; teams keep using outdated assumptions; PMM identifies insights but doesn't operationalize them; sales and CS create their own shadow updates.

---

### Step 12 — Run structured post-launch reviews and institutionalize learning

A mature Grow phase always includes a formal learning loop. Without it, the same mistakes repeat across launches.

**Review cadence:**
- 30-day review: early signal check, onboarding friction, quick wins
- 60-day review: adoption patterns, messaging performance, field feedback
- 90-day review: full performance assessment, funnel diagnosis, optimization priorities
- Quarterly: strategic iteration, expansion opportunities, future launch recommendations, **Context Document update** (below)

**Traffic-light review (MKT1)** — the decision step in every review. Rate each item red / yellow / green: campaigns, growth engines and channels, content series, sales plays, segments, ecosystem partners, big bets.

| Light | Meaning | Where time goes | Typical call |
|---|---|---|---|
| 🟢 Green | Working | A lot — scale it, find *why* it works, apply the pattern elsewhere | **Scale** |
| 🟡 Yellow | Close to working | The most — this is where effort moves results | **Improve** |
| 🔴 Red | Not working | The least — reds rarely turn green | **Pause** or **stop** |

The common mistake is spending most energy trying to fix the reds. For the list itself, a stop / start / continue sheet with fields for owner, effort, and impact works well (MKT1's Prioritization list & stop/start/continue exercise). Every item leaves the review with one call — scale, improve, pause, or stop — and an owner.

**Strong review structure:**
1. Launch objective recap (GACCS goal, revenue lever, big bet success criteria)
2. KPI performance vs. targets, plus project and ops goal status
3. Did the 30/60/90-day momentum plan run?
4. Adoption analysis
5. Segment and use-case findings (including recommended ICP tier moves)
6. Messaging, perception, and enablement effectiveness
7. Customer feedback themes
8. Product friction and issues
9. Traffic-light review: scale / improve / pause / stop, with owners and deadlines
10. Implications for future launches

**Quarterly Context Document update (MKT1 strategy review).** Write what Grow learned back into the shared Context Document, each change dated "last verified":
- **ICPs BY MATURITY** — move ICPs between Core / Scaling / Testing / Not a priority; update time allocation today
- **REVENUE LEVERS** — re-rank if priorities shifted
- **MARKETING ADVANTAGES** — re-rate strength today and maturity; add or drop advantages
- **CHANNEL STRATEGY** — re-score engines the traffic-light review moved
- **Ecosystem** — new competitors, complements, or frenemies; partner performance
- **PERCEPTIONS** — update each status with evidence
- **POSITIONING STATEMENT** — flag whether it needs revisiting (e.g., the comparator shifts from the old way to named competitors as the market matures)

These updates are what Discover, Strategize, and Define read on the next cycle. With MKT1 tools connected, re-run the matching tool for any section that changed a lot, rather than editing it by hand.

**If the team has a company profile**, also propose the matching profile updates to each section owner (sections 2, 3, 6, 7, and 9 most often), and re-run the health check from `pmm-setup` so section 0 shows whether the PMM function is improving. Offer to schedule this quarterly review if it isn't already.

**Templates:** Post-launch review template, Traffic-light review sheet, Lessons learned worksheet, 30/60/90-day review deck, Action log, Decision register, Context Document update log, Company profile change log.

**Key outputs:** Post-launch review, Traffic-light decisions (scale / improve / pause / stop), Lessons learned repository, Optimization action plan, Future launch recommendations, Updated Context Document, Proposed company profile updates and re-scored health check.

**Good:** Review is honest, specific, and action-oriented; learnings documented and reused; teams leave with decisions; PMM improves launch quality over time through organizational memory.
**Weak:** Postmortems skipped or become blame sessions; no action log maintained; same launch mistakes repeat; learnings discussed once then forgotten.

---

## Grow phase checklist

**Learning and measurement:**
- [ ] Defined what we need to learn post-launch, starting from big bets, KPO goals, and the GACCS brief?
- [ ] Tracking both leading and lagging indicators?
- [ ] Results segmented by audience, use case, and channel?
- [ ] Campaign influence and lifecycle stage reporting in place; inbound and outbound reported separately?

**Adoption and lifecycle:**
- [ ] Activation defined and measured?
- [ ] Drop-off points identified in onboarding funnel?
- [ ] Time-to-value understood?

**Customer insight:**
- [ ] Qualitative feedback collected systematically?
- [ ] Feedback synthesized into themes?
- [ ] Customer expectations vs. real experiences assessed?

**Messaging and GTM performance:**
- [ ] Know which messages resonate and which don't?
- [ ] Perception statuses updated with evidence?
- [ ] Objections and conversion blockers tracked?
- [ ] Win/loss insights shaping field guidance?

**Growth opportunities:**
- [ ] Emerging segments or use cases identified?
- [ ] Expansion and retention opportunities visible?
- [ ] Optimization ideas prioritized by impact?

**Product and organizational learning:**
- [ ] Structured insights fed back to product?
- [ ] Customer library of proof maintained, and stories pass the share test?
- [ ] Enablement, lifecycle, and sales plays updated based on learnings?
- [ ] Content hits repurposed and doubled down on?
- [ ] Traffic-light review done, with a scale / improve / pause / stop call and owner for every item?
- [ ] Context Document updated (ICP tiers, levers, advantages, ecosystem, perceptions, positioning flag)?

---

## Core Grow document structure

| Section | Contents |
|---|---|
| 1. Executive summary | What launched, review period, top performance outcomes, top growth priorities |
| 2. Objective recap | Original goals, revenue lever, KPO goals, big bet success criteria, hypotheses |
| 3. Performance analysis | Leading/lagging indicators, lifecycle stages, campaign influence, efficiency metrics, segment/cohort insights |
| 4. Adoption and usage | Activation definition, adoption trends, time-to-value, usage depth, retention signals |
| 5. Customer insight | Top feedback themes, onboarding friction, unmet needs, customer language updates |
| 6. Messaging and GTM effectiveness | Message resonance, perception status, objection themes, sales feedback, campaign and ecosystem performance, competitive patterns |
| 7. Growth opportunities | New segments and recommended ICP tier moves, expansion use cases, retention improvements, pricing/packaging implications |
| 8. Product implications | Roadmap feedback, feature gaps, commercially important friction points |
| 9. Proof and enablement updates | Customer library additions, proof points, content hits to repurpose, enablement changes, lifecycle optimization |
| 10. Traffic-light decisions | Every item rated red / yellow / green with a scale / improve / pause / stop call, owner, timeline, expected impact |
| 11. Context Document updates | ICP tiers, revenue levers, advantages, ecosystem, perceptions, positioning flag — dated |

---

## What good vs. weak Grow looks like

**Good Grow work is:**
- Analytical but not purely descriptive
- Action-oriented, not dashboard-oriented
- Cross-functional, not trapped within marketing
- Customer-informed, not assumption-led
- Segmented, not overly aggregated
- Continuous, not one-and-done
- Tied to adoption and revenue outcomes
- Designed to improve both current and future performance

**Weak Grow work tends to be:**
- Limited to vanity metric reporting
- Disconnected from product and customer reality
- Anecdotal rather than systematic
- Reactive instead of prioritized
- Shallow on adoption and retention
- Weak at turning insight into action
- Forgotten after one review cycle
- Focused only on acquisition, not lifecycle growth

---

## Common mistakes to avoid

1. Treating Grow as just reporting metrics
2. Measuring activity but not value realization
3. Looking only at aggregate data
4. Ignoring activation and onboarding friction
5. Collecting feedback with no synthesis method
6. Failing to test whether messaging actually worked
7. Not connecting product usage to GTM and revenue outcomes
8. Letting customer evidence go uncaptured
9. Running postmortems without action plans
10. Not feeding insights back into product, sales, and lifecycle teams
11. Optimizing acquisition while neglecting retention and expansion
12. Moving on to the next launch before extracting real learning
13. Spending most energy trying to fix the reds instead of scaling the greens and moving the yellows
14. Fighting over attribution credit instead of learning what works
15. Relying on first-touch / original-source attribution alone
16. Producing long, generic case studies no customer would share
17. Leaving the Context Document stale after the market has moved

---

## Template toolkit

**Essential:**
- Post-launch learning agenda
- Growth KPI dashboard
- Campaign influence, lifecycle stage, and account-stage progression reports
- Full-funnel conversion calculator and marketing ops checklist
- AI answer-engine check
- Traffic-light review sheet (stop / start / continue)
- Customer library (searchable proof)
- Context Document update log
- Post-launch scorecard
- Cohort analysis template
- Adoption and activation analysis worksheet
- Voice-of-customer tracker
- Customer interview guide
- Support and feedback theme analysis template
- Messaging performance scorecard
- Funnel friction diagnosis worksheet
- PMA Win/Loss Email Templates (coda.io/@product-marketing-alliance-pma)
- Onboarding journey map
- Time-to-value analysis template
- Segment opportunity assessment
- Product feedback synthesis brief
- PMA Customer Case Study Questions
- Proof point library
- Post-launch review template
- Lessons learned log
- Optimization action tracker

**Optional but valuable:**
- Expansion play brief
- Customer health and risk signals tracker
- Persona-by-stage performance map
- Lifecycle messaging optimization brief
- Reference customer pipeline
- Revenue impact scoring framework
- Market signal tracker for adjacent segments
- Content calendar mapped to perceptions
- Bottom-up forecast

---

## Downstream connections

The Grow phase feeds back into all upstream phases — it is a continuous loop. The quarterly Context Document update (Step 12) is how:
- **Back to Discover** — new customer insights, ICP tier moves, and ecosystem changes update the Context Document
- **Back to Strategize** — re-ranked revenue levers, re-rated marketing advantages, and traffic-light calls on engines and big bets reshape the next plan
- **Back to Define** — perception statuses and messaging learnings refresh positioning, value pillars, and proof; a flag if the comparator should change
- **Back to Get Set** — enablement, content hits to repurpose, and the customer library feed the next launch

---

## Reference frameworks

**Primary (structural backbone):**
- PMA Product Marketing Framework — Grow phase
- PMA Win/Loss Email Templates (coda.io/@product-marketing-alliance-pma)
- PMA Customer Case Study Questions
- PMA Sales Confidence Survey Questions
- PMA S.M.A.R.T. Template
- PMA OKR Toolkit
- PMM-GPT best practice guidance (PMA, 2026)

**Secondary (philosophical lens and operating practices):**
- MKT1 / Emily Kramer — customer feedback as the foundation of audience understanding; win/loss as core PMM intelligence; specifically:
  - Traffic lights and KPO goals (Dear Marketers, Episode 9)
  - Campaign influence reporting, lifecycle stages, blended CAC, neutral pipeline labels, rethinking case studies (Dear Marketers, Episode 12)
  - Basic tracking and attribution views; inbound vs. outbound (How to measure what marketing activities are actually driving revenue)
  - Attribution for learning, not credit (Dear Marketers, Episode 6)
  - Efficiency metrics: CAC ratio, payback period, LTV:CAC (How to calculate your marketing budget)
  - Repurpose and reinforce (MKT1 Field Guide to B2B Startup Marketing, Part 2)
  - Strategy review cadence (Marketing strategy exercises to kick off your annual planning process)
  - Making the cut-vs-scale call (I analyzed 1,100+ marketing job posts)
  - Templates: Full-funnel conversion calculator, Marketing ops checklist, Bottom-up forecasting sheet, Marketing budget & efficiency metrics, Prioritization list & stop/start/continue, Content strategy & annual planning calendar, Content roadmap
  - MKT1 MCP tools, when connected: `mkt1_aeo_audit`, `mkt1_incognito_competitive_research`, `mkt1_linkedin_posts_analysis_beta`
- SVPG / Martina Lauchengco (Loved) — post-launch learning as a shared PM/PMM responsibility for reaching sustained product/market fit
