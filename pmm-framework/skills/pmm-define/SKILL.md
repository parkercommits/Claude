---
name: pmm-define
description: >
  This skill should be used when the user wants to "build the positioning for [company/product]",
  "write the messaging framework", "help me define the product story", "run the Define phase",
  "create a messaging house", "build the value proposition", "help me with positioning and messaging",
  "write the product narrative", "define our use cases", or "build the differentiation framework".
  Executes the PMA Define phase: 14 steps covering product type and comparator, positioning
  statement, messaging architecture, personas, use cases, differentiation, proof points,
  perceptions, product narrative, message validation, and governance.
metadata:
  version: "0.2.0"
  author: "Parker Lyons"
---

# PMM Define Skill

## Trigger conditions
Invoke this skill when the user says any of the following (or close variants):
- "Build the positioning for [company/product]"
- "Write the messaging framework for [product]"
- "Help me define the product story"
- "Run the Define phase"
- "Create a messaging house for [product]"
- "Build the value proposition for [product]"
- "Help me with positioning and messaging"
- "Write the product narrative"
- "Define our use cases"
- "Build the differentiation framework"
- Any request to create market-facing or internal messaging after strategy is complete

**Prerequisite:** The Strategize phase should be complete — specifically: agreed target segment, ICP, priority personas, business objectives, use case focus, GTM motion, pricing/packaging assumptions, and the **working positioning hypothesis and working perceptions** Strategize drafts (see "Strategy on a page" in the Context Document). Define also reads the Discover Context Document: ICP tiers and primary audience, primary problem solved today, product analysis, and candidate comparators. If these don't exist, prompt the user to complete or share them before messaging work begins. Starting positioning before segmentation is clear is one of the most common Define mistakes.

**Positioning and perceptions handoff:** Strategize drafts a working positioning hypothesis (product type, comparator, and the three positioning answers) and working perceptions, so GTM choices and big bets rest on them. Define does not start from scratch — it pressure-tests both against the evidence, then finalizes them (positioning in Steps 3–4, perceptions in Step 11) and logs what changed. If Strategize skipped either, draft it in the relevant step from the Discover inputs.

---

## Framework & philosophy

This skill executes the **Define phase of the PMA Product Marketing Framework.**

**The goal of Define is to turn strategic choices into the market-facing and internally usable foundation for execution.**

- Strategize answers: *What opportunity are we pursuing? Who are we targeting? How will we go to market?*
- Define answers: *How exactly will we describe this product? What is the positioning we want the market to remember? What messages should each audience hear? How do we translate strategy into a clear product story, proof, use cases, and sales narrative?*

**A strong Define phase does three things well:**
1. Clarifies the market story so customers immediately understand why this matters
2. Creates message discipline so every team tells the same story in the right way
3. Builds the bridge from strategy to execution so Get Set becomes faster, sharper, and more consistent

**The key test for Define completeness:** Could your demand gen lead, content lead, sales enablement lead, AEs, CSMs, and product team all use the messaging framework to create their own assets *without inventing a new story*? If no — Define is not done yet.

**Audience-first lens (MKT1):** Throughout Define, the question is always "what does this mean for the customer?" not "what does this say about our product." Define is where product truth becomes customer relevance.

**Positioning → messaging → copy (MKT1).** Keep the three layers distinct:
- **Positioning** — how the product solves the problem better than a specific alternative, for the primary audience. Short, stable, internal.
- **Messaging** — positioning adapted by audience, funnel stage, and channel. The intent and guidelines behind what you say.
- **Copy** — the exact words in a specific asset. Written from messaging, never the other way round.

Product positioning is also a subset of the company story, not the whole of it. The company story is carried by **perceptions** (Step 11); product positioning and launch messaging should support them.

**Short beats exhaustive.** Positioning should condense research, not restate it. A long positioning document tends to be both exhaustive and unfinished. Keep the positioning and core messaging to a page or two; everything else is supporting appendix.

---

## Engagement modes

- **Build mode** — Working at or for this company. All 14 steps apply. Access to internal data, existing personas, sales input, and customer research to ground messaging in reality.
- **Job hunt mode** — Targeting this company as a prospective employer. Build a hypothetical positioning and messaging framework from public sources. This is exceptionally powerful for interviews — showing up with a complete messaging house for a company's product demonstrates senior-level PMM thinking. Always include the homepage hero audit (Step 13) of the company's current site: what it says today, how it scores on who / what / why better, and a proposed rewrite. Flag all assumptions ⚠️ **Job Hunt Mode**.

---

## The 14 Define steps

### Step 1 — Reconfirm strategic inputs before writing messaging

Weak Define work happens when teams jump straight into taglines and copy without stable strategy beneath them.

**Actions:**
- Review and confirm: target segment, ICP, priority personas, business objective, use case focus, GTM motion, pricing/packaging assumptions
- Pull from the Discover Context Document: ICP tiers and the one primary audience, primary problem solved today, features → use cases → benefits map, and candidate comparators
- Pull the working positioning hypothesis and working perceptions from Strategize; note which parts are evidence-backed and which are guesses
- Identify unresolved strategic issues that would weaken positioning
- Clarify what is fixed vs. still a hypothesis
- Align on the scope of what is being defined: product / feature / solution / package / platform capability / category narrative

**Templates:** Messaging kickoff brief, Define phase intake template, Strategy-to-positioning handoff doc, Assumptions and open questions log.

**Key output:** Define Phase Brief / Messaging Kickoff Brief.

**Good:** Everyone agrees on target customer and use case before messaging starts; open questions surfaced early.
**Weak:** Team is still debating audience while messaging is underway; positioning created before segmentation is resolved.

---

### Step 2 — Distill the core customer problem and value thesis

Before writing positioning, sharply define the customer problem, the impact of that problem, the desired outcome, why current alternatives fall short, and why your offer deserves attention.

**Actions:**
- Synthesize research into a customer-centered problem statement
- Capture current state and desired future state
- Define the value hypothesis: what changes for the customer? what outcome improves? what friction is removed? what risk is reduced?
- Separate: product truth / market relevance / emotional resonance

**Useful frameworks:**
- **Jobs-to-be-Done (JTBD):** What triggers customers to look for a solution? What barriers stop them? What progress do they seek?
- **Current-state / future-state framing:** "Today you struggle with X. With this, you achieve Y."
- **Value proposition design:** Match customer pains → desired gains → product value

**Templates:** Problem statement template, Value proposition canvas, JTBD worksheet, Customer outcomes map, Pains/gains/value drivers worksheet.

**Key outputs:** Customer problem statement, Value thesis, Outcome framework, Core value proposition draft.

**Good:** Problem described in customer language; value tied to outcomes not features; message makes sense to both buyer and user.
**Weak:** Problem statement sounds like a roadmap update; value proposition is feature-heavy; no link between customer pain and business outcome.

---

### Step 3 — Choose the product type and comparator (frame of reference)

Customers understand new offers by comparing them to something they already know. Positioning is ultimately about comparison, so the most important frame-of-reference decision is **what single alternative you position against**. The fastest route there is to identify the product type (MKT1).

**The four product types and their comparators:**

| Product type | What it is | Position against |
|---|---|---|
| **Vertical solution** | A product built for a specific industry or role, where horizontal tools exist | The generic, horizontal tools the audience uses today |
| **New way** | A new approach to a problem people already solve some other way | The old way — the status quo, manual process, or legacy approach |
| **10x better** | A clearly superior version of a product type the audience already knows | The incumbent competitor(s) |
| **Buy vs. build** | A product that replaces what teams would otherwise build in-house | Building it yourself |

**Rules of thumb:**
- Pick the type with the **primary audience** in mind — the same product can be a different type to different audiences.
- If more than one type applies, draft positioning against each comparator and choose the strongest.
- Tie-breaks: torn between vertical solution and new way → choose **vertical solution**. Torn between buy vs. build and new way → choose **buy vs. build**.
- "10x better" is a high bar. If you aren't truly 10x better for everyone, narrow the audience until you are.
- **Don't create a new category by default.** Early on it is rarely worth it. Describe the new way in plain language rather than coining a category name; early competitors in the same emerging space often help establish the approach.
- Product type and comparator can, and likely will, change as the market matures.

**Actions:**
- Start from the candidate comparators in the Discover Context Document and the Strategize positioning hypothesis
- Classify the product type for the primary audience; apply the rules of thumb
- Choose one comparator; record the runners-up and why they lost
- Clarify what you are, what you are not, and how buyers describe the space — align to buyer language, not internal preference
- Map the full set of substitutes (direct competitors, status quo, manual workaround, internal build, adjacent tools) so Step 8 can address them

**Templates:** Product type and comparator worksheet, Competitive alternatives map, "What are we?" decision memo.

**Key outputs:** Product type, chosen comparator (with rationale and runners-up), Competitive alternatives map, Category language guidance.

**Good:** Buyers can quickly understand what the product is; one clear comparator; sales can explain the offer without over-educating; uses a frame customers recognize.
**Weak:** Company insists on category language no customer uses; product described in abstract invented terms; positioning against several alternatives at once; confusion about whether it competes with tools, services, or workflows.

---

### Step 4 — Create the positioning statement

The centerpiece of the Define phase. Positioning is not a slogan — it is the strategic articulation of your place in the market, for the primary audience, against the chosen comparator.

**Master positioning — the three questions (MKT1).** Lead with these; this is the version teams remember:
1. **Who is it for?** The primary audience, narrowed until the product is clearly better for them
2. **What is it?** In plain language the audience already uses
3. **Why is it better** than the chosen comparator, on the single most important difference?

**Long-form internal statement.** Once the three answers are set, expand them into the full statement below for internal alignment. It must not contradict the three answers.

**Positioning must also answer:**
- What unmet need or problem does it solve?
- Why should the market believe us?

**Long-form positioning statement structure:**
```
For [target customer / persona / segment]
Who [has a specific problem or goal]
Our [product/solution] is [category / frame of reference]
That [delivers key benefit / outcome]
Unlike [alternative / competitor / status quo]
We [differ in specific, credible ways]
Because [proof / reasons to believe]
```

**Actions:**
- Build a positioning statement covering: target audience, need/problem, product/solution definition, key value, differentiation, proof/credibility
- Test it: is it specific? Is it distinct from competitors? Is it focused on outcomes? Is it credible and supportable? Simple enough to remember, strong enough to scale?
- Compare against the Strategize positioning hypothesis: record what changed and why

**Refinements (only where needed):**
- **Segment-level positioning** for a Scaling-tier ICP whose who / why-better genuinely differs
- **Feature- or product-level positioning** for a distinct product line
- **Today vs. future positioning** — what you can credibly claim now, versus where the product is heading. Never let future positioning leak into today's copy.

**Templates:** Three-question positioning template, Positioning statement template (PMA: coda.io/@product-marketing-alliance-pma), Geoffrey Moore-style positioning framework, Internal positioning canvas.

**Key outputs:** Master positioning (three answers), Long-form internal positioning statement, Positioning change log vs. the Strategize hypothesis, Approved market-facing positioning direction.

**Good:** Specific, audience-centered, outcome-focused, distinct from competitors, credible and scalable.
**Weak:** Generic "single pane of glass / end-to-end / seamless / innovative" language; could apply to any competitor; no clear difference from status quo; too broad to be useful.

---

### Step 5 — Build the messaging architecture

Once positioning is set, create a messaging system usable across channels, personas, funnel stages, and internal teams.

**Top-level building blocks (MKT1)** — draft these first for the primary audience and get buy-in from a small cross-functional group before going further:
- **Problem** you solve
- **Solution** — what the product does about it
- **Who it's for**
- **Why it's better** than the comparator

These four blocks become the homepage hero and the first slide of the sales narrative.

**Messaging hierarchy structure:**

**1. Core message** — The one central idea the market should remember.

**2. Value pillars** — Default to **three** distinct, benefit-led reasons the product matters (e.g., faster outcomes, lower risk, better visibility). Go to four or five only if each is genuinely distinct and provable.

**3. Supporting messages** — What each pillar means in practice.

**4. Proof points** — Evidence that each claim is true.

**5. Persona adaptations** — How the message changes by buyer role, user role, or industry.

**6. Use-case adaptations** — How the story changes based on the job-to-be-done.

**7. How it works** — The product explained in about three simple steps. Essential for "new way" products and anything complex; it removes the question "but how?"

**Actions:**
- Draft the four top-level building blocks for the primary audience first; secure buy-in; then repeat for secondary audiences
- Create a messaging hierarchy with: core message, value pillars, how it works, persona-specific messages, use-case-specific messages, proof points, objection handling themes, channel adaptations, copy guidance
- Keep the core messaging guide to a page or two

**Templates:** Messaging hierarchy template, Messaging matrix, Value pillars worksheet, Persona messaging template, Message map, PMA Messaging Framework (coda.io/@product-marketing-alliance-pma), PMA Storytelling Framework.

**Key outputs:** Messaging framework / messaging house, Value pillars, Persona-based message map, Use-case messaging, Proof point library.

**Good:** Clear hierarchy; consistency with room for adaptation; value pillars differentiated and evidence-backed; messaging changes by persona without losing core narrative.
**Weak:** Disconnected list of claims; every team invents its own story; persona messaging is just the same copy with a different title.

---

### Step 6 — Define personas, buying roles, and audience-specific needs

Define is where PMM sharpens personas into messaging-ready audience profiles — knowing not just who personas are, but what language they use, what outcomes matter, what objections they have, what proof they need, and how they influence the buying decision.

**Actions:**
- Refine buyer personas and user personas
- Identify buying committee roles and map: goals, pain points, triggers, priorities, objections, decision criteria, preferred proof
- Differentiate between: champion, decision-maker, user, blocker, evaluator

**Buyer committee mapping (B2B):**
- Who feels the pain?
- Who signs the contract?
- Who validates risk?
- Who uses the product daily?

**Decision criteria mapping:**
- Functional criteria
- Economic criteria
- Technical criteria
- Emotional criteria
- Political/internal criteria

**Templates:** PMA B2B Buyer Persona Template (coda.io/@product-marketing-alliance-pma), PMA B2C Buyer Persona Example, PMA B2B User Persona Template, PMA B2B Persona Questions, Buyer committee map, Persona messaging brief, Objection and priority matrix.

**Key outputs:** Refined personas, Buyer committee map, Persona-specific priorities and messaging guidance.

**Good:** Personas influence actual messaging and asset creation; team understands buyer vs. user needs; objections and proof needs are specific by audience.
**Weak:** Personas are demographic posters with no strategic utility; internal teams cannot use them in real work; buyer/user/approver blended together.

---

### Step 7 — Define primary use cases and solution narratives

Customers often buy solutions for a specific job, not a full feature set. Use-case work ensures the product is communicated in terms of real situations where it matters most.

**Use-case prioritization criteria:**
- Pain intensity
- Market demand
- Differentiation
- Product readiness
- Monetization potential
- Sales simplicity

**Solution narrative structure (Situation-Complication-Resolution):**
- **Situation:** What's happening now
- **Complication:** Why current methods fail
- **Resolution:** How the product improves the outcome

**Lead with one "land" use case (MKT1).** Listing everything the product can do makes the message confusing. Choose a single entry-point use case — the one that best fits the primary audience's most urgent problem and is easiest to adopt — and lead with it in top-of-funnel messaging. Other use cases support expansion and appear deeper in the funnel.

**Actions:**
- Prioritize the most commercially relevant use cases
- Name the land use case; map the others to expansion or specific personas
- For each: identify trigger, workflow/problem, desired outcome, product capability involved, proof/credibility needed
- Translate the product into "how it helps in a real situation"

**Templates:** Use-case prioritization matrix, Solution narrative template, Use-case brief, Workflow-to-value mapping worksheet.

**Key outputs:** Priority use-case list, Use-case narratives, Solution story by use case, Use-case proof requirements.

**Good:** PMM identifies the few use cases most likely to win in market; sales and marketing can tell concrete stories; product becomes easier to understand and sell.
**Weak:** Every feature becomes a "use case"; narrative too broad to resonate; no prioritization between high-impact and edge-case scenarios.

---

### Step 8 — Establish differentiation and competitive messaging

Translate competitive insight into a usable, credible market stance — starting with strategic differentiation, not just battlecards.

**Differentiation hierarchy — test claims in this order:**
1. Is it true?
2. Is it relevant?
3. Is it specific?
4. Is it defensible?
5. Does the customer care?

**Alternatives-based positioning — compare against:**
- Doing nothing / status quo
- Manual process
- Incumbent solution
- Point solution
- Internal build

**Choose the competitive target by market maturity (MKT1):**
- **Early or "new way" markets:** position against the old way (status quo, manual process, legacy approach), not against other emerging players. Emerging competitors help validate the approach; attacking them confuses buyers.
- **Maturing markets:** as buyers start comparing vendors directly, shift differentiation toward named competitors.
- **Match the audience's sophistication:** for advanced buyers, explain why current approaches are hard and differentiate against the tools they use now. For less mature buyers, differentiate against the status quo and introduce far fewer new concepts.

**Actions:**
- Identify competitors and alternatives most likely to matter
- Clarify where you truly win, where to avoid direct comparison, where status quo is the main competitor
- Turn competitive insight into differentiation themes and message guidance

**Templates:** Competitive positioning matrix, Differentiation worksheet, Reasons-to-win framework, Alternative comparison brief, PMA Competitor SWOT (coda.io/@product-marketing-alliance-pma).

**Key outputs:** Differentiation framework, Competitive messaging guidance, Reasons to win / reasons to believe.

**Good:** Differentiation based on customer value; claims credible and specific; teams know when to compare directly and when to reframe.
**Weak:** "We're better because we have more features"; no distinction between parity and true differentiation; competitive messaging aggressive but not believable.

---

### Step 9 — Build proof points, evidence, and reasons to believe

Good positioning without proof is aspiration. Document the evidence that supports every major claim.

**Types of proof to gather and organize:**
- Customer quotes and testimonials
- Case studies
- Benchmark data
- Product performance metrics
- Analyst validation
- Implementation examples
- Security/compliance reassurance

**Actions:**
- Match proof to: claims, personas, funnel stage, use case
- Identify proof gaps that must be solved before launch

**Templates:** Proof point library, Claims-to-evidence map, Social proof inventory, Validation gap tracker, PMA Customer Case Study Questions (coda.io/@product-marketing-alliance-pma).

**Key outputs:** Reasons-to-believe library, Claims-to-proof matrix, Evidence gap list.

**Good:** Every major value claim has supporting proof; proof tailored to buyer concerns; PMM knows where the story is strong vs. still a hypothesis.
**Weak:** Claims broad and unsubstantiated; proof consists only of "customers love it"; no evidence strategy for risk-sensitive buyers.

---

### Step 10 — Align messaging with pricing, packaging, and offer design

Messaging cannot exist in a vacuum — how an offer is packaged shapes how it should be positioned.

**Actions:**
- Ensure positioning accurately reflects the commercial offer
- Clarify: what's included / what's premium / what's add-on / what's limited
- Pressure-test whether messaging overpromises relative to packaging
- Help make pricing/packaging understandable in customer language

**Templates:** Offer narrative template, Packaging-to-value map, Monetization messaging brief, Commercial story framework.

**Key outputs:** Offer narrative, Packaging explanation guidance, Commercial messaging notes.

**Good:** Offer structure and positioning reinforce each other; sales can explain value and package logic simply.
**Weak:** Premium positioning with unclear packaging; messages promise outcomes the package doesn't support.

---

### Step 11 — Define perceptions (the company story layer)

Product positioning covers the product. **Perceptions** cover the whole company story: the 3–5 beliefs you want your audience to hold and repeat back to you (MKT1). They sit above product positioning; the product story, launches, and most content should support at least one of them. Without them, every launch tells a separate story.

**Write 3–5 perceptions, each:**
- Written from the **audience's point of view**, as a belief they'd say out loud ("Brand is measurable," not "We measure brand")
- Tagged with a category: **company**, **audience**, **market**, or **product** insight
- Given a status: **established** (already believed), **emerging** (some evidence), or **new** (we must create it)
- Backed by supporting evidence — customer quotes, data, trends — that content can later use
- Durable for roughly 6–12 months

**Test:** No other company could credibly claim the same combination of perceptions. If a competitor could, sharpen them.

**Actions:**
- Start from Strategize's working perceptions; refine them cross-functionally (product, sales, CS, leadership), grounded in Discover research, and log what changed — big bets planned in Strategize may need updating if a perception changes
- Check that the master positioning reinforces at least one product perception
- For each perception, sketch the content, campaigns, or proof that would drive it (handed to Get Set and Grow)

**Templates:** Perceptions worksheet (perception, POV, category, status, evidence, programs that drive it).

**Key outputs:** 3–5 approved perceptions with status and supporting evidence.

**Good:** Perceptions are specific, audience-voiced, and distinctive; teams can say which perception a piece of content supports.
**Weak:** Perceptions read like company values or taglines; written in "we" voice; generic enough that any competitor could claim them.

> **In job hunt mode:** infer the perceptions the company appears to be driving today from its site, content, and executive posts, then propose a sharper set.

---

### Step 12 — Create the product story and narrative flow

Positioning and messaging are essential, but teams also need the coherent narrative that explains the market problem, urgency, solution, impact, and credibility — the backbone for launch presentations, web copy, keynote structure, sales pitches, demos, and press narrative. The product story should nest under the perceptions from Step 11, not tell a separate story.

**Master product story elements:**
- Market context (why this matters now)
- Customer struggle (the problem in their world)
- Why existing approaches fail
- What changed / why now
- What the product enables
- Why it's credible
- What outcome customers can expect

**Useful narrative methodologies:**
- **Problem-agitate-solve:** for urgency and clarity
- **StoryBrand structure:** makes customer the hero, not the company
- **Narrative design:** context → tension → solution → evidence → action

**Templates:** Story arc template, Product narrative framework, Executive narrative brief, Narrative flow outline, PMA Storytelling Framework (coda.io/@product-marketing-alliance-pma).

**Key outputs:** Master product story, Narrative deck/outline, Market-facing story framework.

**Good:** Story is memorable and easy to retell; creates urgency without hype; supports both brand-level and product-level communication.
**Weak:** Story is a feature tour; starts with the company rather than the customer; different functions retell it in incompatible ways.

---

### Step 13 — Validate messaging before full-scale rollout

PMMs should not assume the first draft is correct because internal stakeholders like it.

**Test messaging with:** customers, prospects, sales reps, CS, executives, partners.

**What to test:** clarity, relevance, differentiation, believability, emotional resonance, recall.

**Homepage hero test (MKT1):** Visitors give a homepage a few seconds. Show the hero (or a draft of it) to someone in the primary audience for about five seconds, then ask: Who is this for? What is it? Why is it better than what you use now? If they can't answer all three, the copy failed — fix messaging before writing more assets. In job hunt mode, run this audit on the company's current homepage and propose a rewrite.

**Qualitative testing:** interviews to explore what resonates, what confuses, what feels unique, what sounds generic.
**Quantitative testing:** surveys or experiments to measure preference, comprehension, perceived differentiation, and intent.

**Templates:** Message testing guide, Concept test interview script, Sales feedback form, A/B messaging experiment brief.

**Key outputs:** Messaging validation summary, Revised positioning and message recommendations, Known message risks.

**Good:** PMM uses customer and field feedback to improve the narrative; messaging gets sharper before campaign build starts; evidence that the message lands.
**Weak:** Messaging approved internally only; revision driven by HIPPOs not market response; teams learn messaging is weak after launch.

---

### Step 14 — Secure cross-functional approval and establish message governance

Define is not done when the messaging exists. It is done when the organization knows which message is official and how it should be used.

**Actions:**
- Align stakeholders on final narrative and message set
- Document: approved positioning, approved perceptions, approved pillars, approved proof points, words/phrases to use, words/phrases to avoid
- Define brand voice and tone (personality, a few do/don't examples) so copy doesn't sound generic or machine-written
- Establish governance for future edits, including when positioning gets revisited (e.g., comparator shift as the market matures)

**Copy guardrails to include in the terminology guide (MKT1):**
- Clear over clever — write the way the audience speaks; plain language beats pithy wordplay
- No generic outcome claims ("increase revenue," "boost productivity") in the hero or top third of a page — every competitor says them
- Match jargon to audience sophistication
- Specific social proof ("Used by 40 regional utilities") over vague praise ("Companies love us")

**Templates:** Messaging approval workflow, Message governance doc, Terminology guide, Brand and PMM alignment brief.

**Key outputs:** Approved messaging framework, Terminology guide, Message governance rules.

**Good:** One source of truth exists; brand, demand gen, content, product, and sales are aligned; teams know what is fixed and what can be adapted.
**Weak:** Multiple versions circulate; everyone uses different terms for the same product; PMM keeps "fixing copy" because governance was never established.

---

## Core messaging document structure

Lead with a **one-page summary** that most teams can work from on its own. Everything else is an appendix for teams that need depth.

**Page 1 — Positioning & messaging on a page:**
- Primary audience (and ICP tier)
- Product type and comparator
- Master positioning: who it's for / what it is / why it's better
- Perceptions (3–5)
- Top-level messaging blocks: problem / solution / who / why better
- Three value pillars, each with its strongest proof point
- Land use case
- How it works (three steps)

**Appendix:**

| Section | Contents |
|---|---|
| A. Audience definition | Primary segment, buyer personas, user personas, buying roles |
| B. Customer problem | Core pain, current-state friction, business impact, why now |
| C. Value proposition | Core value thesis, desired outcomes, promise to customer |
| D. Frame of reference | Product type rationale, comparator runners-up, full alternatives map |
| E. Long-form positioning | Full internal positioning statement; segment, feature, and future positioning if any |
| F. Messaging architecture | Core message, value pillars, support points, proof points |
| G. Persona & use-case adaptations | What each audience cares about, objections, tailored value emphasis |
| H. Differentiation | Why we win, where we're distinct, where to avoid weak comparisons |
| I. Story framework | Narrative flow for launch, content, and sales |
| J. Guidance | Approved terms, voice and tone, copy guardrails, phrases to avoid |
| K. Validation notes | What has been tested (incl. homepage hero test), what still needs testing, known risks |

---

## Define phase checklist

**Strategic readiness:**
- [ ] Target audience clear enough to support messaging work?
- [ ] Primary use cases agreed?
- [ ] Unresolved strategic questions documented?

**Positioning foundation:**
- [ ] Customer problem clearly articulated?
- [ ] Desired customer outcome defined?
- [ ] Product type identified and one comparator chosen?
- [ ] Strategize positioning hypothesis tested and changes logged?

**Messaging:**
- [ ] Master positioning written as three answers (who / what / why better)?
- [ ] 3–5 perceptions defined, audience-voiced, with status?
- [ ] Land use case named?
- [ ] One-page summary exists?
- [ ] Value pillars created with supporting proof?
- [ ] Clear messaging hierarchy exists?

**Audience relevance:**
- [ ] Buyer and user personas refined for messaging use?
- [ ] Objections and decision criteria mapped by persona?
- [ ] Messaging adapted by use case?

**Differentiation:**
- [ ] Differentiation is relevant and credible?
- [ ] Alternatives customers compare us against are identified?
- [ ] Claims hold up under competitive scrutiny?

**Proof:**
- [ ] Every major claim has evidence?
- [ ] Proof gaps identified?
- [ ] Proof points mapped to audience concerns?

**Validation and governance:**
- [ ] Messaging tested externally or with the field?
- [ ] Homepage hero passes the who / what / why-better test?
- [ ] One approved source of truth exists?
- [ ] Teams know what language to use and avoid?

---

## Common mistakes to avoid

1. **Confusing messaging with copywriting** — starting with taglines before positioning is clear
2. **Using internal product architecture as the message structure** — organize by customer value, not by feature hierarchy
3. **Writing to everyone** — start with the primary audience, then adapt
4. **Treating differentiation as a feature checklist** — differentiation is about customer value, not feature count
5. **Ignoring proof and reasons to believe** — claims without evidence are not credible
6. **Creating personas that aren't actionable** — every persona should influence at least one real asset
7. **Failing to prioritize use cases** — not every workflow deserves equal attention
8. **Letting every stakeholder rewrite the message** — governance must be established early
9. **Skipping message testing** — internal consensus is not market validation
10. **Building a messaging deck no team actually uses** — operationalize the framework, don't file it away
11. **Positioning against several alternatives at once** — choose one comparator
12. **Coining a category too early** — describe the new way in plain language first
13. **Writing an exhaustive positioning document** — condense to a page; put depth in the appendix
14. **Telling launch stories that don't ladder up** — every launch should support at least one perception

---

## What good vs. weak Define looks like

**Good Define work is:**
- Customer-centered, not company-centered
- Specific, not generic
- Differentiated, not interchangeable
- Outcome-led, not feature-led
- Evidence-backed, not slogan-heavy
- Consistent, not fragmented
- Usable across functions, not trapped in a strategy deck
- Tested, not assumed

**Weak Define work tends to be:**
- Filled with buzzwords and abstractions
- Too broad to guide execution
- Disconnected from actual buyer language
- Missing proof points
- Internally inconsistent across sales, product, and marketing
- Based on product architecture instead of customer value
- Not validated with the market
- Impossible to operationalize

---

## Template toolkit

**Essential templates:**
- Define phase kickoff brief
- Problem statement template
- Value proposition canvas
- Product type and comparator worksheet
- Three-question positioning template (who / what / why better)
- Positioning statement template (PMA: coda.io/@product-marketing-alliance-pma)
- Perceptions worksheet
- Positioning & messaging on a page (one-page summary)
- Messaging hierarchy / messaging house (PMA Messaging Framework)
- Value pillars worksheet
- Persona messaging template (PMA B2B Buyer Persona Template)
- Buyer committee map
- Use-case prioritization matrix
- Solution narrative template
- Differentiation framework
- Claims-to-proof matrix
- Product story / narrative outline (PMA Storytelling Framework)
- Message testing guide, including the homepage hero test
- Terminology and governance guide, including voice and tone

**Optional but valuable:**
- Category framing worksheet
- Feature-to-benefit-to-outcome map
- Message do/don't guidance
- Industry-specific message variation template
- Pricing/packaging narrative brief
- Objection handling pre-work template

---

## Downstream skills this feeds into

The Define outputs power everything in Get Set:
- **PMM Get Set** — uses the one-page summary, messaging framework, positioning statement, persona guides, land use case, use-case narratives, and product story to build: sales decks, battlecards, launch emails, demo talk tracks, onboarding copy, website copy, campaign briefs. Launch messaging must support at least one perception.
- **PMM Grow** — uses messaging as the baseline to measure adoption and message pull-through post-launch, and tracks whether perceptions are moving from new → emerging → established

Define also writes back to the Discover Context Document if positioning work changes the primary audience, primary problem, or comparator.

---

## Reference frameworks

**Primary (structural backbone):**
- PMA Product Marketing Framework — Define phase
- PMA Positioning Template (coda.io/@product-marketing-alliance-pma)
- PMA Messaging Framework
- PMA Storytelling Framework
- PMA B2B Buyer Persona Template + B2B Persona Questions
- PMA B2B User Persona Template
- PMA Customer Case Study Questions
- PMM-GPT best practice guidance (PMA, 2026)

**Secondary (philosophical lens and operating practices):**
- MKT1 / Emily Kramer — audience-first positioning; the "who is this for" question before "what does it do"; specifically:
  - Product types, comparators, three positioning questions, today vs. future positioning (MKT1 Guide to Positioning; Field Guide to B2B Startup Marketing, Part 2)
  - Market-maturity guidance, land use case, primary audience in the hero (Positioning & messaging teardown, with Anthony Pierri)
  - Messaging building blocks, messaging vs. copy (How to create a more effective homepage)
  - Perceptions (Perceptions: Our favorite marketing strategy exercise; How to build your marketing strategy in Claude)
  - Common messaging mistakes, brand personality (guest post by Allyson Letteri)
- SVPG / Martina Lauchengco (Loved) — messaging as the market side of product/market fit
