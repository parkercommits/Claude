---
name: brain-dump
description: "This skill should be used when the user wants to empty their head or has a jumble of thoughts, tasks or worries, for example \"brain dump\", \"let me get this out of my head\", \"I have a million things\", \"can't stop thinking about stuff\", \"here's my list\", a long rambling voice message, or a photo of a paper list or sticky notes. It sorts the dump into tasks with next actions, calendar items, ideas, worries to park and notes, proposes do / delegate / defer / delete for each task, removes duplicates against the master list, offers to add items to the user's task app with consent, and ends with a single next action."
metadata:
  version: "0.2.0"
  author: "Parker Lyons"
---

# Brain dump — Empty your head, keep one thing

Working memory is the bottleneck. A brain dump moves everything out of the head and into one trusted place, then hands back exactly one thing to do. The user does the dumping; the coach does the sorting.

**Read first:** `skills/onboarding/references/coaching-principles.md`, then the **Manual of Me**: §1 priorities, §4 where the master list lives, §8 values.

## Step 1 — Invite the dump

If the user hasn't dumped yet: "Go ahead and dump it all, in any order. Talking is fastest: tap the microphone. A photo of a paper list works too." Don't interrupt or ask questions until they say they're done.

Accept anything: voice transcripts, messy text, photos of paper lists, notebooks or sticky notes (read the image), or pasted notes.

## Step 2 — Sort it

Pull every item out and put each into one bucket:

| Bucket | What goes here | What happens |
|---|---|---|
| **Tasks** | Anything that needs doing | Rewritten as a next action starting with a verb ("Email Dana about…") |
| **Calendar** | Anything tied to a date or time | Proposed as an event or reminder |
| **Ideas** | Possibilities, "what ifs", projects for someday | A parking lot, so they're safe but not on today's list |
| **Worries** | Things that are bugging them | Parked with a time to revisit, or turned into a task if there's an action |
| **Notes** | Information to keep | Filed with the notes |

Then for each task, propose one of **do, delegate, defer, delete**, briefly. Group them; don't make the user rule on each item one by one. Example: "I'd delete these two (they don't serve your current goals), defer these four to next week, and do these three. OK?"

Check against the master list and drop duplicates.

## Step 3 — Play it back short

Summarize in counts plus the few that matter, not the full list:

> 23 things out of your head. 9 tasks (3 for this week), 2 calendar items, 6 ideas parked, 4 worries parked, 2 notes. Two tasks I'd delete. One idea that seems exciting to you: the newsletter.

Ask: "Anything I got wrong?"

## Step 4 — Put it somewhere trusted

With an explicit yes, add tasks and dates to the user's master list and calendar (§4: Apple Reminders through the Claude desktop app, Trello, Notion, Google Calendar…). If nothing is connected, give a clean, copyable list grouped by bucket. Never write to the user's tools without consent.

## Step 5 — Hand back ONE thing

Finish with a single next action using the `what-next` format: the task, why, a five-minute first step. If it's late at night or the dump was mostly worries, the one thing can be **rest**: "Everything's parked. Nothing needs you until the morning standup."

## Variations

- **Evening dump** (worries keeping them up): park every worry with a specific time tomorrow to look at it, and keep the tone calm and brief.
- **Consolidation dump** (several lists in several places): collect them all, merge into the one master list agreed in onboarding, and note in §4 that consolidation is done.
