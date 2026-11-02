# Coaching State template

The structure of the user's private Coaching State. `kickoff` creates it; every skill reads and updates it. Keep the section names exactly as below so later sessions can find things. Where it lives: `saving-the-state.md`.

```markdown
# Coaching State — [Name]
Last updated: [date]

## Profile
- Target role(s):
- Seniority band:
- Track: Quick Prep / Full System
- Feedback directness: [1-5]
- Interview timeline: [date or "ongoing"]
- Time-aware coaching mode: [triage / focused / full]
- Interview history: [first-time / active but not advancing / experienced but rusty]
- Biggest concern:
- Coaching State location: [Google Doc / Claude Project / local folder — see saving-the-state.md]
- Known interview formats: [e.g., "behavioral screen, system design (verbal walkthrough)" — updated by Format Discovery Protocol during prep/mock]

## Resume Analysis
- Positioning strengths: [the 2-3 signals a hiring manager sees in 30 seconds]
- Likely interviewer concerns: [flagged from resume — gaps, short tenures, domain switches, seniority mismatches]
- Career narrative gaps: [transitions that need a story ready]
- Story seeds: [resume bullets with likely rich stories behind them]

## Storybank
| ID | Title | Primary Skill | Earned Secret | Strength | Last Used |
|----|-------|---------------|---------------|----------|-----------|
[rows — compact index. Full column spec in `skills/interview-coach/references/storybank-guide.md` — the guide adds Secondary Skill, Impact, Domain, Risk/Stakes, and Notes. Add extra columns as stories are enriched.]

### Story Details
#### S001 — [Title]
- Situation:
- Task:
- Action:
- Result:
- Earned Secret:
- Deploy for: [one-line use case — e.g., "leadership under ambiguity questions"]
- Version history: [date — what changed]

[repeat for each story]

## Score History
### Historical Summary (when table exceeds 15 rows, summarize older entries here)
[Narrated trend summary of older sessions — direction per dimension, inflection points, what caused shifts]

### Recent Scores
| Date | Type | Context | Sub | Str | Rel | Cred | Diff | Hire Signal | Self-Δ |
|------|------|---------|-----|-----|-----|------|------|-------------|--------|
[rows — Type: interview/practice/mock. Sub=Substance, Str=Structure, Rel=Relevance, Cred=Credibility, Diff=Differentiation — each 1-5 numeric. Hire Signal: Strong Hire/Hire/Mixed/No Hire (from analyze/mock only — leave blank for practice). Self-Δ: over/under/accurate (>0.5 delta from coach scores = over or under; within 0.5 = accurate). Keep most recent 10-15 rows.]

## Outcome Log
| Date | Company | Role | Round | Result | Notes |
|------|---------|------|-------|--------|-------|
[rows — Result: advanced/rejected/pending/offer]

## Drill Progression
- Current stage: [1-8]
- Gates passed: [list]
- Revisit queue: [weaknesses to resurface]

## Interview Loops (active)
### [Company Name]
- Status: [Researched / Applied / Interviewing / Offer / Closed]
- Rounds completed: [list with dates]
- Round formats:
  - Round 1: [format, duration, interviewer type — e.g., "Behavioral screen, 45min, recruiter"]
  - Round 2: [format, duration, interviewer type]
- Stories used: [S### per round]
- Concerns surfaced: [ranked list from `concerns` — severity + counter strategy, or from analyze/rejection feedback]
- Interviewer intel: [LinkedIn URLs + key insights, linked to rounds]
- Prepared questions: [top 3 from `questions` if run]
- Next round: [date, format if known]
- Fit assessment: [from `research` if run — strong / moderate / weak]
- Key signals: [from `research` — 1-2 lines]
- Date researched: [date, if `research` was run]

## Active Coaching Strategy
- Primary bottleneck: [dimension]
- Current approach: [what we're working on and how]
- Rationale: [why this approach — links to decision tree / data]
- Pivot if: [conditions that would trigger a strategy change]
- Root causes detected: [list]
- Self-assessment tendency: [over-rater / under-rater / well-calibrated]
- Previous approaches: [list of abandoned strategies with brief reason — e.g., "Structure drills — ceiling at 3.5, diminishing returns"]

## Meta-Check Log
| Session | Candidate Feedback | Adjustment Made |
|---------|-------------------|-----------------|
[rows — record every meta-check response and any coaching adjustment]

## Session Log
### Historical Summary (when log exceeds 15 rows, summarize older entries here)
[Brief narrative of earlier sessions]

### Recent Sessions
| Date | Commands Run | Key Outcomes |
|------|-------------|--------------|
[rows — brief, 1-line per session]

## Coaching Notes
[Freeform observations that don't fit structured fields — things the coach should remember between sessions]
- [date]: [observation — e.g., "candidate freezes in panel formats," "gets defensive about short tenure at X," "prefers morning interviews," "mentioned they interview better after coffee"]
```
