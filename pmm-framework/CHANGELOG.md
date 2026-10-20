# Changelog

All notable changes to the PMM Framework plugin. Versions follow [semantic versioning](https://semver.org): minor versions add or expand skills; patch versions fix wording or errors.

## [0.2.0] — 2026-10-20

### Changed — `pmm-discover`
Refined against MKT1 product marketing research best practices.

- **Three research pillars.** Discover now explicitly covers audience, market/ecosystem/competitors, and product.
- **TAM mapping replaces TAM/SAM/SOM.** Map TAM coverage by company type and role (now vs later); a single top-down size figure is optional for the business case.
- **ICP tiering is a required output.** Core / Scaling / Testing / Not a priority today, with one primary audience named.
- **ICP composition** at company and persona level, including buyer roles.
- **Audience behavior** is now an explicit research target: information sources, communities, tool stack, content preferences, trusted voices.
- **Competitive intelligence expanded to an ecosystem map.** New complements and frenemies table; competitor matrix adds business model, stage/funding, homepage positioning, GTM motion, and content types.
- **New 2E Product analysis step.** Primary problem solved today and a features → use cases → benefits map.
- **Research reliability rules** for desktop and AI-assisted research: canonical URLs, defined attributes, blank-and-flag instead of guessing, sources on every data point, spot-checks.
- **Handoff to Define.** Synthesis lists candidate comparators (without choosing one) plus ICP tiers and the primary problem.
- **Living Context Document** with "Last verified" dates and a sources list.
- Updated synthesis themes, templates toolkit, "What NOT to do," downstream handoffs, and MKT1 references.

### Changed — `pmm-define`
Refined against MKT1 positioning and messaging best practices. Define now has 14 steps.

- **Positioning handoff from Strategize.** Strategize drafts a working positioning hypothesis; Define pressure-tests and finalizes it, logging what changed. Define also reads ICP tiers, primary problem, product analysis, and candidate comparators from the Discover Context Document.
- **Step 3 rebuilt around product type → comparator.** Four product types (vertical solution, new way, 10x better, buy vs. build), tie-break rules, one chosen comparator, and a caution against coining a new category early.
- **Master positioning uses MKT1's three questions** (who it's for / what it is / why it's better); the Moore-style statement becomes the long-form internal version. Adds segment, feature, and today-vs-future refinements.
- **Positioning → messaging → copy** layers made explicit, with a "short beats exhaustive" principle.
- **Messaging architecture** starts from four top-level building blocks (problem / solution / who / why better), defaults to three value pillars, and adds a "how it works" block.
- **Land use case**: lead top-of-funnel messaging with one entry-point use case.
- **Competitive target by market maturity** and audience sophistication.
- **New Step 11 — Perceptions**: 3–5 audience-voiced beliefs with category, status, and evidence; the product story nests under them.
- **Homepage hero test** added to validation (and a homepage audit in job hunt mode).
- **Governance** adds voice and tone plus MKT1 copy guardrails.
- **One-page summary** now leads the core messaging document; the rest moves to an appendix.
- Updated checklist, common mistakes, templates, downstream handoffs, and MKT1 references.
- Step 11 now starts from Strategize's working perceptions and finalizes them.

### Changed — `pmm-strategize`
Refined against MKT1 marketing strategy best practices.

- **Inherit or build.** Inherit an existing company-level marketing strategy; draft a light version only when none exists (always in job hunt mode).
- **Three drivers of strategy** — research, business model / GTM motion, marketing advantages — framed up front, with "random acts of marketing" as the anti-pattern.
- **Workstream 1 adds:** ranked four revenue levers (1A), the marketing advantages exercise (1B), and a working positioning hypothesis plus working perceptions (1C) for Define to finalize.
- **KPO goals:** KPIs plus 1–3 big bets (the launch is one), ops goals, and explicit non-goals.
- **Audience strategy uses Discover's ICP tiers**, with effort allocation by tier.
- **Growth engines replace the flat channel list:** inbound, outbound, product virality, events, ecosystem, lifecycle — chosen from audience behavior, motion, and advantages. Adds a check that marketing fits the GTM motion.
- **Plans and pricing page guidance:** have one, show some prices, avoid fake gating, keep it simple, test transparency.
- **Fuel vs. engine balance** check in resourcing.
- **"Strategy on a page"** leads the artifact stack and is written into the Context Document.
- Updated week-by-week model, decision framework, common mistakes, downstream handoffs, and MKT1 references.

### Changed — `pmm-get-set`
Refined against MKT1 launch and campaign best practices.

- **A launch is a campaign**, with one DRI and momentum beyond launch day; checklists are a starting point, not the strategy.
- **Right-size by tier** table: which of the 12 steps apply at Tier 1, 2, and 3.
- **Step 1:** decide whether it deserves a launch at all (roadmap ≠ marketing calendar); tier by comparing against other campaigns; tier frequencies; bundle releases and decouple ship and announce dates; **GACCS launch brief** replaces the generic launch charter.
- **Step 2:** new ecosystem amplification workstream (early access and amplification kits for creators, customers, partners, community); pair launches with data reports, events, and other moments.
- **Step 3:** every asset brief names the perception it supports and its distribution plan.
- **Step 4:** co-build enablement with one or two reps, capture what buyers say, speak in pipeline terms, set rules of engagement for launch leads.
- **Step 9:** QA checks perceptions, the homepage hero test, and the pricing page.
- **Step 10:** launch metrics tied to the revenue lever the launch moves.
- **Step 12:** 30/60/90-day post-launch momentum plan and Grow handoff.
- Prerequisites read Strategy on a page and Define's one-page summary; updated checklist, document structure, mistakes, templates, and MKT1 references.

### Changed — `pmm-grow`
Refined against MKT1 measurement, customer marketing, and review practices.

- **Make the call:** every review ends with scale / improve / pause / stop decisions.
- **Step 1:** learning agenda starts from big bets, KPO goals, the revenue lever, the GACCS brief, the momentum plan, and perceptions.
- **Step 2:** measure for learning, not credit — lifecycle stages for contacts and accounts, last touch before meeting/opportunity, campaign influence reporting, blended CAC, inbound and outbound reported separately, neutral pipeline labels; efficiency metrics (CAC ratio, payback, LTV:CAC); report to sales in pipeline terms.
- **Step 5:** track perceptions and update their status with evidence.
- **Step 8:** express segment findings as ICP tier moves; review ecosystem partner performance.
- **Step 10:** rethink the case study — searchable customer library, "case study, plus," interview first, the share test, amplify customer posts.
- **Step 11:** start field updates with the rep partners; find content hits, repurpose them, and reinforce perceptions.
- **Step 12:** traffic-light review (red / yellow / green) as the decision step; big bet and momentum-plan review; quarterly Context Document update (ICP tiers, levers, advantages, ecosystem, perceptions, positioning flag).
- Updated checklist, document structure, mistakes, templates, upstream connections, and MKT1 references.

### Changed — `pmm-director`, README, and plugin manifest
Consistency pass so the orchestrator matches the refined phases.

- **Phase table** lists the key outputs each phase hands on.
- **Working drafts, finalized later:** positioning and perceptions are drafted in Strategize and finalized in Define.
- **Job hunt sequence** is now Discover → light Strategize (Workstream 1) → Define, ending with a homepage hero audit.
- **Living Context Document**, retitled `[Company] — PMM Context`: each phase adds a section with "Last verified" dates; Grow writes back quarterly.
- **New "When sources disagree" rules:** evidence beats frameworks; PMA sets the structure; MKT1 sets operating practice inside each step; follow choices the skills have already made; flag unresolved conflicts rather than blending; future sources follow the same pattern.
- **Common requests routing** table.
- README and plugin description updated to reflect the MKT1 refinements and current version.

## [0.1.0] — 2026-06-04

Initial release: `pmm-director`, `pmm-discover`, `pmm-strategize`, `pmm-define`, `pmm-get-set`, `pmm-grow`.
