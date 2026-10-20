# PMM Framework Plugin

A full-stack Product Marketing Director agent built on the PMA 5-phase framework. Grounded in PMA best practices, MKT1 audience-first methodology, PMM-GPT guidance, and SVPG/Loved.

## Overview

This plugin gives you a Product Marketing Director agent capable of executing end-to-end PMM strategy — from initial market discovery through post-launch growth optimization. It runs in two modes:

- **Build mode** — Active PMM work at or for a company
- **Job hunt mode** — Proactively developing PMM strategy for companies you're targeting in interviews

## Skills

| Skill | Trigger | Phase |
|---|---|---|
| `pmm-director` | "Help me with product marketing for [company]" | Orchestrator |
| `pmm-discover` | "Run discovery on [company]" | Phase 1 — Discover |
| `pmm-strategize` | "Build the GTM strategy for [company]" | Phase 2 — Strategize |
| `pmm-define` | "Build the positioning for [product]" | Phase 3 — Define |
| `pmm-get-set` | "Build the launch plan" | Phase 4 — Get Set |
| `pmm-grow` | "Analyze post-launch performance" | Phase 5 — Grow |

## Usage

**Start here for any new engagement:**
> "Help me with product marketing for [company URL]"

The `pmm-director` skill will orient you, confirm the mode (build vs job hunt), and route you to the right phase.

**Jump directly to a phase:**
> "Run discovery on [company]"
> "Build the positioning for [product]"
> "Write the battlecard for [competitor]"

## Phase sequence

```
Discover → Strategize → Define → Get Set → Grow → (loops back to Discover)
```

Each phase produces a output document. The **Context Document** created in Discover (`[Company] — PMM Context | Discover Phase`) is shared memory across all phases — every downstream skill reads it before executing.

## Frameworks embedded

- **PMA Product Marketing Framework** — 5-phase structural backbone
- **PMA Coda template library** — 35+ templates mapped to each phase (coda.io/@product-marketing-alliance-pma)
- **PMM-GPT best practices** — Phase-by-phase guidance from PMA's AI (2026)
- **MKT1 / Emily Kramer** — Audience-first methodology and positioning framework
- **SVPG / Martina Lauchengco (Loved)** — PMM as the market side of product/market fit

## Tools used

Requires Google Drive MCP to be connected for saving Context Documents as Google Docs. Falls back to Markdown files if Drive is unavailable. Web search is used during Discover for company research.

## Setup

No environment variables required. Ensure the following are connected in Cowork:
- Google Drive (for saving Context Documents)
- Web search (for company research in Discover phase)
