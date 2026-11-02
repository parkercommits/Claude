---
name: what-next
description: "This skill should be used when the user doesn't know what to do next or can't choose, for example \"what should I do now?\", \"I have two hours, what should I work on?\", \"I'm spinning\", \"help me decide\", \"I have a gap between meetings\", \"too many things, where do I start?\", \"I'm stuck choosing\", or when a scheduled midday check-in asks what's next. It reads the user's Manual of Me, calendar, task list and today's plan, filters the options by deadlines, values, impact and current energy, and returns ONE task with a one-line reason, a five-minute first step, a done level and a time box, so the user starts instead of deciding."
metadata:
  version: "0.2.0"
  author: "Parker Lyons"
---

# What next — One thing, right now

The hero skill. It exists to kill the "what should I do with this open time?" spin, which for many ADHD adults eats the first half of every free block. The rule is simple: **the coach decides, the user starts.** Never hand back a menu.

**Read first:** `skills/onboarding/references/coaching-principles.md`, then the user's **Manual of Me** (see "Starting any skill" in the principles). Use §1 priorities and goals, §5 energy windows, §6 modalities, §8 values, §9 motivators and §14 coaching preferences.

## Step 1 — Read the moment (no more than one question)

Find out, from context first:
- **How much time** until the next commitment. Read the calendar if connected; otherwise ask.
- **Energy right now.** If unknown, ask one quick question: "Energy, 1 to 5?" Combine it with the peak and low windows in §5.
- **Anything urgent** due before the window ends.

If two of the three are already known, don't ask at all. If the user sounds flooded, upset or ashamed, skip this skill and run `rejection-reset` (after criticism or rejection) or a short grounding first.

## Step 2 — Gather candidates (silently)

Pull, without showing the list: today's standup intentions, the master task list (Apple Reminders, Trello, Notion or whatever §4 names), carried-forward items from the last retro, and anything the user just mentioned. If there's no list at all, ask for a 60-second brain dump (see `brain-dump`).

## Step 3 — Filter top-down

Apply in order, stopping when one task is left:

1. **Hard deadlines** inside or right after this window.
2. **Values and goals**: what serves §1 goals and §8 values? Ask the manual's filter question: "How does this serve me and what I value?"
3. **Only-I-can-do-it**: favor work only the user can do. Things others could do are candidates to delegate, not do.
4. **Energy fit**: peak energy → deep, creative or high-stakes work. Low energy → batch email, Slack, admin, errands. Very low energy → rest is a valid answer; pick the most depleted rest type from the last check and suggest a short restorative activity.
5. **Fits the window**: if a task can't fit, pick its smallest meaningful slice.
6. **Pull**: among near-equals, take the one the user is most excited about or that offers novelty or challenge.

If the user is choosing between several good options and can't commit (fear of picking the "wrong" one), say plainly: **any of these is fine; picking is the win.** Then pick using the rules above.

## Step 4 — Give ONE answer

Keep it short. Format:

> **Next: [task]** — [one-line why, tied to a goal or value]
> **First 5 minutes:** [a concrete physical action, e.g., "open the doc and write three bullet headings"]
> **Done looks like:** [rare / medium / well-done, with what that means here]
> **Time box:** [length] — I'll check in at [time]. *(Optional dare: "I bet you can get the outline done in 25 minutes.")*

Deliver it in the user's modality and vocabulary (§6, §14): a story-shaped "why" for a conceptual thinker, "intention" or "user story" language for someone who likes product framing, and so on.

## Step 5 — Escape hatches

- **"Not that one."** Offer exactly one alternative and let them choose between two. Never a third list.
- **"I can't start it."** Hand off to `make-it-smaller`.
- **"I'll do it after this other thing…"** Check gently whether the other thing is hyperfocus on something low-value; if so, name it kindly and offer a time box for it.
- **Interruptions arrive.** Re-running `what-next` mid-block is normal, not failure.

## Step 6 — Close the loop

- With a yes, set a check-in at the end of the time box (a scheduled reminder or a reminder in the user's task app; ask before creating anything).
- At the check-in: "How did it go?" Celebrate any progress specifically, offer the next `what-next`, and add notable wins to the wins log (with consent).
- If the same task keeps getting skipped, don't scold. Ask what need the avoidance is meeting and offer `make-it-smaller`.
