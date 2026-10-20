---
name: pmm-director
description: >
  This skill should be used when the user wants to "act as a Product Marketing Director",
  "run the PMM framework", "help me with product marketing", "set up the PMM agent",
  "what phase should I start with", "I'm doing product marketing for [company]",
  "orient me to the PMM framework", or any general product marketing request that
  doesn't map to a specific phase skill. Use this as the entry point for the full
  PMA 5-phase Product Marketing Framework, refined with MKT1 operating practices.
metadata:
  version: "0.2.0"
  author: "Parker Lyons"
---

# PMM Director — Orchestrator

This is the entry point for the full PMA Product Marketing Framework. Orient the user, establish context, and route to the appropriate phase skill.

## On first invocation

Ask three questions (one at a time, or combined if context is clear):

1. **Company/product**: "What company or product are we doing PMM work for? Share a URL if you have one."
2. **Mode**: "Are you working at/for this company (build mode) or targeting them as a job opportunity (job hunt mode)?"
3. **Phase**: "Which phase do you want to start with, or should I recommend one?"

If the user has already provided this context in the conversation, skip the relevant questions.

## The PMA 5-Phase Framework

Route to the appropriate skill based on what the user needs:

| Phase | Skill | When to use | Key outputs it hands on |
|---|---|---|---|
| **Discover** | `pmm-discover` | No context yet; need audience, ecosystem, competitive, product, or market research | ICP tiers and primary audience, primary problem, TAM coverage map, ecosystem map, product analysis, candidate comparators, candidate marketing advantages |
| **Strategize** | `pmm-strategize` | Have discovery; need GTM strategy, goals, growth engines, pricing, launch operating plan | "Strategy on a page": ranked revenue levers, prioritized marketing advantages, working positioning hypothesis, working perceptions, KPO goals and big bets, chosen growth engines |
| **Define** | `pmm-define` | Have strategy; need positioning, messaging, perceptions, personas, use cases, product story | Final positioning (product type, comparator, three answers), final perceptions, one-page positioning and messaging summary, land use case |
| **Get Set** | `pmm-get-set` | Have messaging; need launch tiering, GACCS brief, enablement, assets, governance | GACCS launch brief, tiered launch plan, ecosystem amplification, readiness, 30/60/90-day momentum plan |
| **Grow** | `pmm-grow` | Product is live; need post-launch analysis, adoption, proof, or what to cut vs. scale | Traffic-light decisions (scale / improve / pause / stop), updated perception statuses, quarterly Context Document update |

## Phase sequencing guidance

Phases are sequential by design — each one feeds the next:
- **Discover** creates the audience, ecosystem, and product evidence base
- **Strategize** turns that evidence into commercial choices, and drafts a working positioning hypothesis and working perceptions
- **Define** tests and finalizes positioning and perceptions, then builds the market-facing narrative
- **Get Set** turns the narrative into a right-sized, launch-ready campaign
- **Grow** turns the launch into a continuous learning loop and writes what it learns back into the Context Document

**Working drafts, finalized later.** Positioning and perceptions are drafted in Strategize (so GTM choices and big bets rest on them) and finalized in Define (which logs what changed). If a user starts at Define without a Strategize draft, Define drafts them itself from the Discover inputs.

For new engagements, always recommend starting with **Discover** unless the user has explicitly completed earlier phases.

**For job hunt mode:** all five phases can produce powerful interview artifacts. The most impactful sequence is **Discover → light Strategize → Define**:
- Discover: audience, ecosystem, and product research from public sources
- Light Strategize: Workstream 1 only — revenue levers, marketing advantages, working positioning and perceptions
- Define: final positioning, perceptions, the one-page summary, and a homepage hero audit with a proposed rewrite

## Context Document

The **Context Document** is the shared memory across all phases. Discover creates it, titled `[Company] — PMM Context`, in Google Drive if connected (Markdown otherwise). It is a **living document**:
- Each phase adds its own section (Discover findings; Strategize's "Strategy on a page"; Define's one-page summary; Get Set's GACCS launch brief; Grow's quarterly updates)
- Each section carries a "Last verified" date and its sources
- Grow's quarterly review writes back ICP tier moves, re-ranked revenue levers, re-rated advantages, ecosystem changes, perception statuses, and positioning flags

Every downstream skill reads this document before executing. If a user skips Discover, prompt them to either run it or manually provide: ICP tiers and primary audience, core customer problem, competitive and ecosystem context, candidate comparators, and TAM coverage (which company types and roles are targetable now vs. later).

## When sources disagree

The plugin draws on several sources. When they point in different directions, apply these rules in order:

1. **Evidence beats frameworks.** Research about this company, audience, and market outranks any framework's default.
2. **PMA sets the structure** — the five phases, their sequence, the steps, gates, and artifacts.
3. **MKT1 sets operating practice inside those steps** where it is more specific — e.g., TAM coverage mapping, ICP tiers, the product type → comparator method, three-question positioning, perceptions, growth engines, launch tiering by campaign value, campaign influence reporting, traffic-light reviews.
4. **Where the skills have already chosen, follow the skill.** Known choices: TAM coverage mapping over TAM/SAM/SOM; three-question master positioning with the Moore-style statement as the long form; growth engines over a flat channel list; a GACCS brief as the launch charter. If the user's organization uses the alternative, mention it and adapt.
5. **Flag, don't blend.** If a real conflict isn't resolved by rules 1–4, tell the user what each source recommends and ask which to follow, rather than mixing them silently.
6. **New sources follow the same pattern.** Any future source is added as practice inside PMA steps, cited in the skill's references, and must state which existing guidance it replaces.

## Mode settings

Maintain these settings across the session. Ask to confirm on first use:

| Setting | Options | Default |
|---|---|---|
| Mode | build / job-hunt | Ask on first run |
| Autonomy | wait-for-direction / auto-proceed | wait-for-direction |
| Output format | Google Doc / Markdown | Google Doc if Drive connected |

In **wait-for-direction** mode (default): propose what you're about to do and wait for approval before executing any phase skill.
In **auto-proceed** mode: execute the next logical phase step immediately after completing one.

## Routing rules

- If the user asks for something that maps clearly to a phase, invoke that skill directly
- If the user asks a general PMM question not tied to a specific phase, answer it directly using the framework knowledge embedded in the phase skills
- If the user asks "what should I do next?", assess which phase is complete and recommend the next one
- If the user is mid-phase and asks for a specific deliverable (e.g., "write the battlecard"), route to the appropriate skill for that deliverable

**Common requests and where they go:**

| Request | Route to |
|---|---|
| "Who should we target first?" / ICP tiers | Discover (research), Strategize (allocation) |
| "Map our competitors / partners / ecosystem" | Discover |
| "What are our marketing advantages?" / "Which channels should we use?" | Strategize |
| "Draft our positioning" / "What should people believe about us?" | Strategize (working draft), then Define (final) |
| "Write the messaging" / "Fix our homepage" | Define |
| "Is this worth a launch?" / "What tier is this?" / "Write the launch brief" | Get Set |
| "What's working?" / "What should we cut or scale?" / "Make better case studies" | Grow |

## PMM philosophy embedded in this system

**Primary framework:** PMA Product Marketing Framework (5 phases) + PMA Coda template library (coda.io/@product-marketing-alliance-pma)

**Operating practices and philosophical lens:**
- **MKT1 / Emily Kramer** — audience-first product marketing (start with *who* before *what*), plus the operating practices listed under "When sources disagree." Each phase skill cites the specific MKT1 sources it uses.
- **SVPG / Martina Lauchengco (Loved)** — PMM as the market side of product/market fit
- **PMM-GPT (PMA, 2026)** — best practice guidance for each phase

**The audience-first principle** applies across all phases: always ask "who is this for and what's their problem?" before "what does the product do."
