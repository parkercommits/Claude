# MKT1 tools — when connected, use them

Some teams connect the **MKT1 MCP** (tools named `mkt1_*`, from Emily Kramer's MKT1 subscription). When those tools are in the session, they are the current, most detailed version of the MKT1 practices this plugin uses. Use them for the steps listed below. When they are not connected, run the plugin's own method in that step — every phase works fully without MKT1.

## Detecting the tools

- Check at intake and at the start of each phase, with the other connections (`connections.md`).
- The tools may be deferred (loaded on demand). Search the session's tools for `mkt1_` before deciding they aren't there.
- Tell the user once, in plain words: "MKT1 tools are connected, so I'll use them for positioning, ICPs, competitive research, and a few other steps." Don't repeat it every phase.
- Never suggest that a team subscribe to MKT1. If they ask what would deepen a step, it's fine to say the step has an MKT1 version.

## Which steps use which tool

| Plugin step | MKT1 tool | Context Document section it fills |
|---|---|---|
| Setup Step 2 — company snapshot | `mkt1_company_overview` | COMPANY OVERVIEW |
| Discover 2B — ICP tiering | `mkt1_icp_prioritization` | ICPs BY MATURITY |
| Discover 2C — competitor research | `mkt1_competitive_research` | COMPETITIVE RESEARCH |
| Strategize 1A — revenue levers | `mkt1_revenue_levers` | REVENUE LEVERS |
| Strategize 1B — marketing advantages | `mkt1_marketing_advantages` | MARKETING ADVANTAGES |
| Strategize Workstream 2 — big bets | `mkt1_big_bets` | BIG BET CAMPAIGNS |
| Strategize Workstream 2 — KPO goals | `mkt1_kpo_goals` | KPO GOALS |
| Strategize 3D — growth engines | `mkt1_channel_strategy` | CHANNEL STRATEGY |
| Define Steps 3–4 — positioning | `mkt1_positioning` | POSITIONING STATEMENT |
| Define Step 11 — perceptions | `mkt1_perceptions` | PERCEPTIONS |
| Define Step 13 — homepage review | `mkt1_homepage_positioning` | HOMEPAGE REVIEW |
| Get Set Step 1 — launch brief | `mkt1_gaccs` | GACCS LAUNCH BRIEF |

Supporting tools, used where a step says so:

| Tool | Use it for |
|---|---|
| `mkt1_incognito_competitive_research` | How buyers, candidates, or AI answer engines see the company vs. competitors from the public web alone (Discover, job hunt mode) |
| `mkt1_general_research` | Any dataset across 10+ companies, or auditing a spreadsheet someone built |
| `mkt1_state_of_b2b_marketing_data`, `mkt1_vetted_b2b_startup_list` | Benchmarks and examples from fast-growing B2B companies |
| `mkt1_website_examples` | Homepage, pricing page, and social-proof patterns (Define, Get Set) |
| `mkt1_aeo_audit` | Whether AI answer engines can find and describe the company (Grow, after web changes) |
| `mkt1_templates` | The current link to any MKT1 template a step names |
| `mkt1_newsletter`, `mkt1_linkedin_search` | The source behind an MKT1 concept, when the user asks "why" |
| `mkt1_job_description_and_scorecard`, `mkt1_interview_questions` | Job hunt mode: the likely scorecard and interview questions for the target role |
| `mkt1_marketing_comp_checker`, `mkt1_salary_lookup`, `mkt1_startup_equity_evaluator` | Job hunt mode, offer stage: salary and equity against MKT1's market data |
| `mkt1_marketing_strategy_setup` | Showing MKT1's strategy progress view beside the health check |

## The pattern for a delegated step

1. **Say which tool you're using**, in one line, then call it. The tool returns instructions; follow them in this conversation.
2. **Feed it what the plugin already knows.** The tools open with a refresher offer and intake questions. Answer from the company profile and the Context Document yourself; ask the user only what neither covers. Skip the refresher unless coach mode is on.
3. **Follow the tool's own steps and rules**, including its DRAFT confirmations, its "blank, don't guess" research rules, and its output format.
4. **Write the confirmed result into the Context Document** under the section name in the table above, with a "Last verified" date and sources, replacing only that section. Do this yourself; don't hand the Context Document to the tool's save routine.
5. **Add what the plugin step asks for that the tool doesn't** — for example, the evidence log, handoffs to the next phase, or job hunt framing — then carry on with the rest of the step.
6. **Offer `marketing-strategy.md` only if the team uses it.** MKT1 tools save to a file of that name. If the team already keeps one, or asks for one, keep it in sync using MKT1's exact headings; otherwise don't create a second strategy file.

**When the tool and the plugin differ:** the tool's version of the MKT1 method wins over this plugin's description of it. Evidence about the company, the team's adopted frameworks, and the PMA phase structure still come first (see "When sources disagree" in the Director).

**When a tool fails or is missing** mid-step, say so in one line and finish the step with the plugin's own method. Never block.

## Surface limits to pass on honestly

- `mkt1_competitive_research` fills three AEO columns and writes a styled spreadsheet only where there's a terminal (Claude Code). Elsewhere it returns the same table as CSV with those columns blank. Say which you got.
- `mkt1_homepage_positioning` and the other research tools grade only what they can actually load. A login page, parked domain, or empty JavaScript shell is reported as such, not graded.
- Some MKT1 templates are Figma boards, interactive microtools, or videos that Claude can't read. Name them and let the user open them.

## Keeping this list current

MKT1 adds and renames tools. Whoever maintains this plugin should check `mkt1_changelog` monthly and update the tables above when a step should use a new tool.

## Distribution rules

This plugin is shared with teams that may not have MKT1. Keep MKT1's paid material out of it and out of anything the plugin saves for sharing:

- Refer to MKT1 tools and templates by name. Don't write template URLs into the plugin; get the current link from `mkt1_templates` in the session when the user needs it.
- Don't copy an MKT1 tool's instructions, column lists, or HTML templates into plugin files or shared documents. Their outputs — the user's own ICP map, positioning, brief — are the user's work and belong in the Context Document.
