# PMM Framework Plugin

A full-stack Product Marketing Director agent built on the PMA 5-phase framework and refined with MKT1's operating practices. Grounded in PMA best practices, MKT1 audience-first methodology, PMM-GPT guidance, and SVPG/Loved.

**Current version:** 0.2.0 — see [CHANGELOG.md](CHANGELOG.md) for what changed in each version.

## Overview

This plugin gives you a Product Marketing Director agent capable of executing end-to-end PMM strategy — from initial market discovery through post-launch growth optimization. It runs in two modes:

- **Build mode** — Active PMM work at or for a company
- **Job hunt mode** — Proactively developing PMM strategy for companies you're targeting in interviews

## Skills

| Skill | Trigger | Phase | Highlights |
|---|---|---|---|
| `pmm-director` | "Help me with product marketing for [company]" | Orchestrator | Routing, handoffs, rules for when sources disagree |
| `pmm-discover` | "Run discovery on [company]" | Phase 1 — Discover | ICP tiers, TAM coverage, ecosystem map, product analysis, research reliability rules |
| `pmm-strategize` | "Build the GTM strategy for [company]" | Phase 2 — Strategize | Revenue levers, marketing advantages, working positioning and perceptions, KPO goals, growth engines |
| `pmm-define` | "Build the positioning for [product]" | Phase 3 — Define | Product type → comparator, three-question positioning, perceptions, one-page summary |
| `pmm-get-set` | "Build the launch plan" | Phase 4 — Get Set | GACCS launch brief, right-size by tier, ecosystem amplification, 30/60/90-day momentum |
| `pmm-grow` | "Analyze post-launch performance" | Phase 5 — Grow | Traffic-light decisions, campaign influence reporting, customer library, quarterly Context Document update |

## Usage

**Start here for any new engagement:**
> "Help me with product marketing for [company URL]"

The `pmm-director` skill will orient you, confirm the mode (build vs job hunt), and route you to the right phase.

**Jump directly to a phase:**
> "Run discovery on [company]"
> "Build the positioning for [product]"
> "Write the battlecard for [competitor]"

**Job hunt mode tip:** the strongest interview sequence is Discover → light Strategize → Define, ending with positioning, perceptions, and a homepage rewrite for the company you're targeting.

## Phase sequence

```
Discover → Strategize → Define → Get Set → Grow → (loops back to Discover)
```

Positioning and perceptions are drafted in Strategize and finalized in Define.

The **Context Document** (`[Company] — PMM Context`) is the shared memory across all phases. Discover creates it; each phase adds a section; Grow updates it quarterly. Every downstream skill reads it before executing.

## Frameworks embedded

- **PMA Product Marketing Framework** — 5-phase structural backbone
- **PMA Coda template library** — 35+ templates mapped to each phase (coda.io/@product-marketing-alliance-pma)
- **PMM-GPT best practices** — Phase-by-phase guidance from PMA's AI (2026)
- **MKT1 / Emily Kramer** — Audience-first methodology and operating practices: ICP tiers, ecosystem mapping, product types and comparators, perceptions, marketing advantages, growth engines, GACCS briefs, launch tiering, campaign influence reporting, traffic-light reviews
- **SVPG / Martina Lauchengco (Loved)** — PMM as the market side of product/market fit

When sources disagree: evidence beats frameworks; PMA sets the structure; MKT1 sets the operating practice inside each step. Details are in the `pmm-director` skill.

## Tools used

Requires Google Drive MCP to be connected for saving Context Documents as Google Docs. Falls back to Markdown files if Drive is unavailable. Web search is used during Discover for company research.

## Setup

No environment variables required. Ensure the following are connected in Cowork:
- Google Drive (for saving Context Documents)
- Web search (for company research in Discover phase)
