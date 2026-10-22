---
name: pmm-setup
description: "This skill should be used when a team or person is starting with the PMM Framework for the first time, or wants to \"set up the PMM agent for [company]\", \"get started\", \"onboard our team\", \"what can this do\", \"run a PMM health check\", \"assess our product marketing\", \"rate our PMM maturity\", \"build our company profile\", or \"update our company profile\". Runs a guided setup of about 15 minutes: orientation, a 10-area PMM health check, gathering existing work (brand guidelines, segmentation, pricing, call transcripts, plans), connecting tools, building a reusable company profile, and a health check report with three recommended first moves."
metadata:
  version: "0.4.0"
  author: "Parker Lyons"
---

# PMM Setup — Guided onboarding and health check

Use this the first time a team (or person) uses the PMM Framework at a real company. It sets up once what every later task needs, so nobody has to re-explain the company, and it gives the user something useful in the first session: a health check report with three clear first moves.

**For job hunt mode** (researching a company you want to work for), the Director's intake is the better fit. This skill can still run a health check from public information if asked — mark every rating as an outside-in estimate.

## Principles

- **Make it easy.** About 15 minutes. Small rounds of questions, multiple choice wherever possible, skips always fine. The user can stop at any step and pick up later.
- **Research first, then confirm.** Draft what you can from the company's website and the files they share, and ask the user to correct it — don't make them type what you can find.
- **Their work is the baseline.** Existing brand guidelines, segmentations, pricing, and plans are the starting point. Later skills audit and build on them rather than starting over.
- **Plain language.** No framework jargon until the user needs it. Talk about jobs ("prep a launch"), not phases ("Get Set").
- **Value before paperwork.** End with a report and a next step, not just a filled-in form.

## Before starting

Check for an existing company profile — in this project's files, the conversation, or a connected Drive. If one exists, offer: **update the profile**, **re-run the health check**, or **skip to work**. Don't redo setup.

## Step 1 — Orient (1 minute)

Tell the user, briefly:
- What the agent does: helps research customers and competitors, set GTM strategy, write positioning and messaging, plan launches, and learn what's working after launch.
- How setup works: a few questions, a health check, share what you already have, and you'll get a short report with three recommended first moves.
- That they can skip anything.

Then ask (one round, multiple choice where possible):
1. **Company** — name and website (if not already known)
2. **Your role** — dedicated PMM / marketing leader / founder or executive / product manager / sales or CS / other
3. **Who does product marketing today** — a dedicated PMM team / one PMM / spread across other roles / nobody yet
4. **What you most want help with first** — show the job menu from the Director (e.g., prep a launch, sharpen positioning, help sales win more, figure out what to focus on)
5. **Coach mode** — "Want me to explain the why behind each step as we go?" Default to **on** when there's no dedicated PMM, or the user is new to PMM; off otherwise.

## Step 2 — Company snapshot (research, then confirm)

Research the company's public footprint (homepage, pricing, product pages, customers, recent news). Present a short draft: what they do, who they sell to, business model and sales motion, stage. Ask: "What's wrong or missing?"

## Step 3 — Health check (5 minutes)

Run the 10-area health check in `references/health-check.md`: three rounds (4 + 3 + 3 areas), one multiple-choice question per area with the area-specific level descriptions as options. After each round, ask once for any documents or systems behind the answers.

## Step 4 — How you work today (a few open questions)

Ask only what the snapshot, health check, and shared files haven't answered. Group into at most two rounds:

- **Pricing and packaging** — how is pricing set today, and what's in each plan?
- **GTM strategy and calendar** — what are this period's goals, upcoming launches or campaigns, and the roadmap themes GTM should know?
- **Feedback loops** — how does what customers say reach marketing, sales, and product? On what rhythm, through which tools?
- **Systems and processes** — which tools do you use for CRM, call recordings, analytics, docs, roadmap, and chat?
- **How teams communicate** — where are decisions written down, which channels and meetings matter, and where should PMM outputs go?
- **Boundaries** — anything I shouldn't read or copy into shared documents?

## Step 5 — Bring what you have

Show this checklist and ask the user to share whatever exists — links, uploads, or "it's in this Drive folder." Explain what each improves so the ask feels worth it:

| Asset | What it sharpens |
|---|---|
| Brand guidelines, tone-of-voice guide | Every customer-facing draft sounds like your brand |
| Current positioning or messaging docs | Positioning work starts from your story, not from scratch |
| Segmentation, ICP, or persona work | Targeting and messaging match your real priorities |
| Call transcripts or a call recording tool | Messaging uses customers' own words; objections are real |
| Pricing sheet and packaging | Pricing advice and sales materials are accurate |
| Marketing or GTM plan, calendar, roadmap | Recommendations fit what's already planned |
| Competitive analysis, battlecards, win/loss notes | Competitive work builds on what sales already knows |
| Past launch plans and post-launch reviews | Launches reuse what worked and avoid repeats |
| Sales deck, case studies, website copy | Audits show where the story drifts |

Read what they share. Summarize it into the profile; don't paste whole documents. Note where each source lives.

## Step 6 — Connect tools

Run the connection check in `skills/pmm-director/references/connections.md`: say what's already connected, and suggest only the two or three missing tool categories that would add the most given their answers. Never block on a connection.

## Step 7 — Build the company profile

Fill in `references/company-profile-template.md` from everything gathered. Mark unconfirmed items ❓ and missing ones "Not yet defined." Show the user a short summary of what's in it and what's missing, and ask them to name an owner for the profile (a role is fine).

## Step 8 — Health check report

Produce a one-page report, following the scoring guidance in `references/health-check.md`:
- **Scorecard** — the ten areas, each with its level, whether evidence backs it, and a one-line note
- **What's strong** — two or three things to protect
- **Biggest gaps** — the ones that matter most for their stated goal
- **Three first moves** — each with why now, what they'll get, rough time, and the exact thing to say to start it
- **Offered next:** recurring tasks (Step 9) and saving the profile for the team (Step 10)

Deliver the report the way the team works (section 8 of the profile): a document, or as an artifact or doc if that's the norm in this environment.

## Step 9 — Offer recurring tasks (optional)

If the environment can schedule tasks, offer a few that match their feedback loops and tools. Suggest at most three; create one only after the user agrees to it.

| Task | Cadence | Needs |
|---|---|---|
| Customer voice digest: themes, objections, and quotes from recent calls | Weekly | Call recording or meeting notes tool |
| Competitor and ecosystem scan: launches, pricing changes, news | Monthly | Web search |
| GTM calendar check: upcoming launches, and whether each has a brief and a tier | Monthly | Docs or roadmap tool |
| Health check and quarterly review: re-score, Grow review, profile updates | Quarterly | Profile and connected tools |

Each scheduled run starts fresh, so write its instructions to name the company, the profile's location, and what to deliver where. Scheduled runs follow the same guardrails: read-only, and ask before changing anything.

## Step 10 — Save the profile for the team

Walk the user through `references/project-setup.md`: a Claude Project in their own workspace (recommended), or a shared Drive folder. Make it step by step and confirm each step.

## Finish

Close with: where the profile and report live, the three first moves, and the single best next prompt to try. Hand off to the Director (or the phase skill for the first move).

## Updating later

When asked to update the profile, show the current sections with their last-updated dates, ask which to change, and add a change-log line. Propose changes to sections other people own rather than overwriting them. Suggest re-running the health check quarterly.
