# Engagement intake — question bank

The Director runs intake once per engagement and saves the answers to the **Engagement setup** section of the Context Document. Phase skills read that section instead of asking again.

## How to ask

- **Ask in small rounds** — at most five questions at a time, most important first.
- **Offer choices** where the answer is one of a few options (use a multiple-choice question tool if the environment has one). Always allow a free-text answer.
- **Accept "don't know" and skips.** Anything skipped, research it if possible; otherwise record it as an open question.
- **Don't re-ask** what the user already said in the conversation or what a connected tool can answer.
- **Offer a fast start.** If the user wants to skip intake, collect only the Round 1 answers and go.
- **Offer "just tell me."** The user can describe the situation freely instead — typed, or spoken with their app's microphone or dictation. Extract the answers, play back "Here's what I heard," and ask only about what's still missing.
- **Offer "fill it in for me."** For any question, draft an answer from research and what's already known, mark it as an estimate, and let the user correct it.

---

## Round 1 — Every engagement

| # | Question | Why it matters |
|---|---|---|
| 1 | Which company and product? (URL if possible) | Anchors all research |
| 2 | **Mode:** build (working at or for the company) or job hunt (targeting it as an employer)? | Changes sources, depth, and outputs |
| 3 | What decision or goal should this work support? (e.g., prepare for a final-round interview, reposition for a new segment, plan a Q3 launch) | Discover starts from the decision and works backward |
| 4 | What do you want at the end? (e.g., interview presentation, positioning one-pager, launch plan, full Context Document) | Sets the stopping point and format |
| 5 | Timeline? (date of interview, launch, or review) | Sets research depth |

Then recommend a starting phase and sequence (job hunt default: Discover → light Strategize → Define).

---

## Round 2A — Job hunt mode

Ask for whatever the user has; everything else is researched from public sources.

**About the role**
- Link to the **job posting** — it often reveals the team's current problems and priorities
- Interview stage, format, and who's on the panel (roles are enough)
- Any take-home or presentation prompt, word for word

**Links to start research from** (any the user has handy)
- Homepage and pricing page
- Blog, newsroom, changelog or release notes
- Help center or product documentation
- Customer case studies or customer page
- Review-site pages (G2, Capterra, TrustRadius, app marketplaces)
- Recent news articles, funding announcements, executive interviews or podcasts
- Industry or analyst reports, white papers relevant to the category

**What the user already knows**
- Competitors and alternatives they believe matter
- Anything learned from the network, recruiters, or earlier interviews
- Their own early hypotheses about the company's positioning or challenges

**Research depth** — offer a choice:
- **Quick scan** — regular, targeted research; fast and light on usage. Enough for early conversations and screens.
- **Deep dive** — deep research for the broad landscape plus targeted research for precise details. Takes longer and uses more of the user's usage allowance. Best for final rounds, presentations, and take-homes.

If the user picks deep dive, check whether a deep research capability is available. If it needs to be turned on by the user (in the Claude app, the Research option in the chat), tell them now so it's ready when Discover starts.

**Optional connections in job hunt mode** (only the user's own data, only with permission):
- Email (e.g., Gmail) — recruiter threads, the job description, interview scheduling details
- Meeting notes or recordings (e.g., Granola, Fireflies) — notes from earlier interview conversations
- Docs (e.g., Google Drive) — the user's own prep notes, résumé, earlier research

---

## Round 2B — Build mode

**If a company profile exists, skip most of this round.** Ask only about the initiative (what, who, what's decided), and anything the profile marks ❓ or "Not yet defined" that this initiative depends on. If no profile exists and the user expects to come back or share with a team, offer `pmm-setup` first.

**About the initiative**
- What's the initiative? (new product, feature launch, repositioning, new segment, competitive response)
- Who are the key stakeholders and decision-makers? (roles are enough)
- What's already decided vs. still open?

**Existing material** — links or file names for any that exist:
- Current positioning, messaging framework, or brand guidelines
- Personas, ICP definitions, segmentation work
- Marketing strategy or annual plan
- Past launch plans and post-launch reviews
- Win/loss analyses, customer research, survey results
- Pricing and packaging documentation

**Tools and data** — which tools does the company use, by category? (See `connections.md`.) Then check which are already connected in this session and suggest the most valuable missing ones.

**Frameworks and experts** (optional)
- Any product marketing frameworks, thought leaders, or internal playbooks the team follows for this kind of work? Use them per the Director's "When sources disagree" rules.

**Access and sensitivity**
- Anything Claude should not read or should not copy into shared documents?
- Should the Context Document be private to the user or shared with the team?

---

## After intake

1. Summarize the setup back to the user in a few lines and confirm.
2. Write the **Engagement setup** section at the top of the Context Document:
   - Company, product, mode, goal/decision, deliverable, timeline
   - Research depth (job hunt) or initiative and stakeholders (build)
   - Links provided, existing material, known competitors, user hypotheses
   - Connected tools by category, and tools the user chose not to connect
   - Open questions and things the user asked not to be used
   - Date
3. Route to the first phase.
