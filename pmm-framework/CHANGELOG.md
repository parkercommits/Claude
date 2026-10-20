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

## [0.1.0] — 2026-06-04

Initial release: `pmm-director`, `pmm-discover`, `pmm-strategize`, `pmm-define`, `pmm-get-set`, `pmm-grow`.
