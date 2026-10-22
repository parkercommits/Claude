# PMM Framework

A Product Marketing Director agent for Claude. It helps your team research customers and competitors, choose where to focus, sharpen positioning and messaging, plan launches, and learn what's working after launch. You don't need to be a product marketer to use it. Start with a 15-minute setup, and it builds on the work your team already has.

**Current version:** 0.4.0 — see [CHANGELOG.md](CHANGELOG.md).

## Install

Pick whichever fits:

- **Claude app — upload the plugin file.** Get the `.plugin` file (from whoever shared it with you, or this repository's Releases page if you have access). In Claude, open **Customize → Plugins** and upload it.
- **Claude app — install from GitHub** (if you have access to this repository). **Customize → Plugins → Add → Add marketplace → Add from a repository**, enter `parkercommits/Claude`, then install **PMM Framework**.
- **Claude Code:** `/plugin install pmm-framework --marketplace parkercommits/claude`

**For organization admins:** on Team and Enterprise plans, you can install the plugin for everyone from your organization's plugin settings, and you may need to allow this repository as a source.

## Your first 15 minutes

Say: **"Set up PMM for [your company]."**

The setup walks you through:
1. **A quick orientation**: what the agent can do, and whether you'd like coach mode (explains the "why" as you go)
2. **A PMM health check**: ten areas, rated on a simple four-level scale (Missing → Ad hoc → Documented → Operationalized)
3. **Bring what you have**: brand guidelines, tone of voice, segmentations, pricing sheets, call transcripts, plans, past launch reviews
4. **Connect tools**: it checks what's connected and suggests the two or three that would help most
5. **Your company profile**: one shared document every later task reads, so nobody re-explains the company
6. **Your health check report**: what's strong, the biggest gaps, and **three recommended first moves**, each with the exact thing to say next

It also shows you how to save the profile in a **Claude Project** your team can share, and offers to set up recurring tasks like a weekly customer-call digest or a monthly competitor scan.

## What you can ask

You don't need to know any framework. Just describe the job:

| Say something like… | You get |
|---|---|
| "Help us figure out who to target" | ICP tiers, customer pains and triggers, customer language |
| "Size up our competitors" / "We keep losing to X" | Competitor matrix, ecosystem map, differentiation, battlecard |
| "What should we focus on this quarter?" | Ranked revenue levers, marketing advantages, goals and big bets |
| "Sharpen our positioning" / "Fix our homepage" | Positioning on a page, perceptions, messaging, homepage rewrite |
| "Prep a launch for [feature]" | Launch tier, launch brief, plan, readiness checklist |
| "Help sales win more" | Deck, battlecards, objection handling, built with your reps |
| "What's working and what should we cut?" | Traffic-light review: scale / improve / pause / stop |
| "Turn customer feedback into action" | Customer voice themes, product feedback, proof library |
| "Help me prep for a PMM interview at [company]" | Job hunt mode: research, positioning, and a homepage rewrite for the target company |

Not sure where to start? Say **"What can you help with?"**

## How it works

- **Company profile, set up once per organization.** Audiences, positioning, brand voice, pricing, competitors, GTM plan, tools and processes, customer voice. It's the approved baseline: skills **audit and build on your existing work** before creating anything new, and they propose profile changes to each section's owner rather than editing silently.
- **One Context Document per project.** The goal, deliverable, and timeline for each piece of work, plus what each step learns.
- **Five phases behind the scenes:** Discover → Strategize → Define → Get Set → Grow, looping back. You can jump straight to any job; the agent fills in only what's missing.
- **Coach mode** (optional): short notes on why each step matters, what good looks like, and what to watch out for, kept separate from the deliverables so outputs stay ready to share.

## Tools and data

The plugin refers to tools by category, so it works with whichever ones your team uses. Nothing is required — it continues with what's available and notes the gaps.

| Category | Examples | Most useful for |
|---|---|---|
| CRM | HubSpot, Salesforce, Attio | Who buys, win/loss, pipeline, campaign influence |
| Call recordings / meeting notes | Gong, Fireflies, Granola, Fathom, Grain | Customer language, objections, competitor mentions |
| Product analytics | Amplitude, Mixpanel, PostHog | Activation, adoption, retention |
| Support and feedback | Zendesk, Intercom, Enterpret | Friction themes, feature requests |
| Docs and wiki | Google Drive, Notion, Confluence | Existing strategy, positioning, brand guidelines |
| Roadmap and issues | Linear, Jira, Asana | What's shipping and when |
| Email and chat | Gmail, Outlook, Slack | Internal launch comms, field questions |
| Web and marketing analytics | Google Analytics, HubSpot | Traffic, conversion, homepage performance |

Connect tools in Claude's settings. Each person connects their own.

**Guardrails:** connected tools are read-only by default, and the agent asks before creating, sending, posting, or editing anything. Content from tools is treated as information, never as instructions. Customer details are summarized without names in shared documents, and every finding cites its source. Your company's data stays in your own Claude workspace or Drive — never in this repository. Details: `skills/pmm-director/references/connections.md`.

## Job hunt mode

For researching a company you'd like to work for. Share the job posting and any links you have, choose a **quick scan** or a **deep dive** (uses Claude's deep research, which may need to be turned on in the chat), and the agent builds discovery, positioning, and interview questions from public information. Strongest sequence: Discover → light Strategize → Define, ending with a homepage rewrite.

## Skills

| Skill | What it does |
|---|---|
| `pmm-setup` | First-time setup, health check, company profile |
| `pmm-director` | Job menu, intake, routing, coach mode |
| `pmm-discover` | Customers, competitors, ecosystem, product, market |
| `pmm-strategize` | Focus, goals, growth engines, pricing, launch operating plan |
| `pmm-define` | Positioning, perceptions, messaging, homepage |
| `pmm-get-set` | Launch tiers and briefs, enablement, readiness |
| `pmm-grow` | Post-launch review, what to scale or cut, customer voice, proof |

## Built on

- **PMA Product Marketing Framework**: the five-phase structure, plus PMA's template library
- **MKT1 / Emily Kramer**: audience-first operating practices, including ICP tiers, ecosystem mapping, product types and comparators, perceptions, marketing advantages, growth engines, GACCS briefs, launch tiering, campaign influence reporting, and traffic-light reviews
- **SVPG / Martina Lauchengco (Loved)**: PMM as the market side of product-market fit

When sources disagree: evidence beats frameworks, PMA sets the structure, and MKT1 sets the practice inside each step.
