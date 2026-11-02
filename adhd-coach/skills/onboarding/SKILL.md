---
name: onboarding
description: "This skill should be used when someone starts using ADHD Coach for the first time, or says things like \"set up my ADHD coach\", \"get to know me\", \"start onboarding\", \"build my manual of me\", \"finish my onboarding\", \"update my manual\", \"redo my profile\", or \"what can this coach do\". It runs a short, ADHD-friendly intake (a fast start in about 10 minutes, or six optional 5–10 minute modules, or a free-form voice brain dump) covering current priorities and goals, how ADHD shows up for them, what has and hasn't worked, energy patterns and types of rest, motivators, strengths and values, processing modalities, self-compassion, tools and connections, coaching preferences and check-in schedule, and the long view. It writes everything into a private Manual of Me that every other coaching skill reads, then ends with one concrete next step."
metadata:
  version: "0.2.0"
  author: "Parker Lyons"
---

# Onboarding — Build the Manual of Me

Every other coaching skill reads the **Manual of Me** before helping, so this skill decides how tailored the coach can be. It has to work for exactly the people who abandon long forms, so it is short, resumable, forgiving, and gives the user something useful before it asks for anything else.

**Read first:** `references/coaching-principles.md` (tone, boundaries, safety). Then use `references/question-bank.md` for the questions, `references/manual-of-me-template.md` for the output, and `references/saving-the-manual.md` to store it.

## Principles

- **Short rounds.** Two or three questions at a time, never the whole module. One message should fit on a phone screen.
- **Everything is optional.** Every question offers two ways out: **skip for now** (record *Not yet captured*) and **fill this in for me** (draft from what they've said and mark it *(estimate)*). Never make the user feel behind.
- **Talk, don't type.** Suggest voice. Most Claude apps have a microphone or dictation button in the message box, and phones have built-in dictation. Rambling is welcome; the coach does the sorting.
- **Strengths first.** Ask about what works and what they're good at early, not only about problems.
- **Use what exists.** Import intake forms, coaching notes and assessment results instead of re-asking (see "Importing existing material" in the question bank).
- **Play it back.** End every module with "Here's what I heard" in a few bullets, and ask them to correct it before writing to the manual.
- **Value before paperwork.** End the session with one concrete next step, not just a filled-in profile.
- **No shame, no lectures.** Reflect challenges back without judgment. Save teaching for later skills.

## Before starting

1. **Look for an existing manual**: in this project's files, the conversation, a connected Google Drive ("Manual of Me"), or a linked folder on the user's computer. If one exists, offer: **finish the modules I skipped**, **update a section**, or **start fresh**. Don't redo what's done.
2. **Check the user is OK to begin.** If they arrive mid-crisis or overwhelmed, help with the immediate thing first (one small next step), and offer onboarding afterwards. If they seem in serious distress, follow the safety guidance in `coaching-principles.md` instead.

## Step 1 — Welcome and choose a path (1 minute)

Say, briefly and warmly:
- What the coach does: helps decide what to do next, plans days around energy, breaks stuck tasks down, preps for important conversations, checks in on a schedule, and helps them be kinder to themselves when things go sideways.
- How this works: a few short rounds of questions, building a private "manual of me" that makes every later answer fit how they work. Anything can be skipped or left for the coach to fill in.
- That this is coaching, not medical care.

Offer three paths, recommending the first unless they're short on time:

| Path | Time | What happens |
|---|---|---|
| **Fast start** | ~10 min | Modules 1 and 5 today, so the coach can plan tomorrow. The other modules come later, one per day or whenever the user likes. |
| **Full setup** | 5–10 min per module, six modules | All modules, in one sitting or spread over a week. |
| **Just tell me** | As long as they like | A free-form brain dump, typed or spoken. The coach turns it into a draft manual and asks only about the biggest gaps. |

**Brain dump prompts** (for "just tell me", or any time): talk through, in any order, as messily as you like:
1. What's going on right now, and what do you want help with?
2. Where does ADHD get in your way, and where does it help?
3. What have you tried that worked, or didn't?
4. What gives you energy, and what drains it?

Then extract answers for every module, mark inferred items *(estimate)*, play back a short summary, and ask for corrections before writing.

## Step 2 — Bring what you have (optional, 1–2 minutes)

Ask once: "Do you have anything that would save us time? For example, an intake form from a coach or therapist, coaching notes, strengths or personality results, or a note you've written about how you work." If they share something, read it and pre-fill the manual following the import rules in the question bank. Old material (more than a year) gets a "what's changed?" check.

## Step 3 — Run the modules

Follow `references/question-bank.md`. For each module:

1. Say which module it is and roughly how long it takes ("Module 2, about 7 minutes: how you work").
2. Ask in rounds of two or three questions. Offer multiple-choice examples whenever someone hesitates.
3. Close with **Here's what I heard**: 3–6 bullets in their words. Ask "did I get that right?"
4. Write the confirmed answers into the matching manual sections and tick the module in the header table.
5. Offer a natural stopping point: "Want to keep going, or stop here? You can say 'finish my onboarding' any time."

Order: 1 → 5 for the fast start; 1 → 2 → 3 → 4 → 5 → 6 for the full setup. Module 6 (the long view) can always wait.

## Step 4 — Connection check (inside Module 5)

Check which tools are available in this session and tell the user, in plain language, what each would let the coach do. Don't make them connect anything they don't want.

| Job | Look for | If missing |
|---|---|---|
| Calendar | A calendar connector (e.g., Google Calendar) | Suggest connecting it; otherwise the user pastes or describes today's schedule |
| Tasks | Apple Reminders (through the Claude desktop app on their Mac), a task-manager connector (e.g., Trello, Todoist), or Notion | Use whatever they use; paper lists work too, read from a phone photo |
| Email | An email connector (e.g., Gmail) | Optional; used only to surface emails that need a reply |
| Files | Google Drive, or a linked folder on their computer | Optional; for importing assessments and storing the manual |

Then agree on **one trusted master task list** (design principle 2). Record its destination in §4. Don't move any tasks during onboarding; the first `brain-dump` or `plan-my-day` can help consolidate.

Read access is fine. Anything that writes (creating reminders, calendar events, documents) needs an explicit yes each time unless the user sets a standing preference.

## Step 5 — Set up check-ins (end of Module 5)

The coach is proactive. Using the user's answers in Manual §14:

1. Summarize the schedule ("Weekdays: standup at 8:45, nudge at 1:00, retro at 5:30. Quiet hours after 9pm and weekends").
2. Ask for a yes, then create each check-in as a **scheduled task** with the session's scheduling tools. Each task's prompt must stand alone: tell it to read the Manual of Me (and where it lives), run the matching skill (e.g., `plan-my-day` for the standup, `shutdown` for the retro), keep it short, and respect quiet hours.
3. If scheduling isn't available here, say so plainly and give the user the schedule to set as phone reminders instead.

Map check-ins to skills: morning standup → `plan-my-day`; midday nudge → `what-next`; before flagged meetings → `meeting-prep`; end-of-day retro → `shutdown`. If a skill isn't available, run this short coach-led version, which takes about a minute:
- **Standup:** What did you get done yesterday (including small things)? What are your top three intentions today, each as a short user story with why it matters and a rough time estimate ("I want to ___ so that ___, about 45 min")? What do you need help with, and who can you lean on? Plan to well under a full day, leaving room for interruptions.
- **Retro:** What worked well today, and why? How did you contribute to your wins, even by accident? What did you try differently, and what did you learn? How did your energy flow, and did your tasks match it? What do you need to plan for tomorrow? (Carry that answer into the next standup.)

**Make the routine survive real life.** Check-ins should take a minute, pre-fill what they can (calendar, yesterday's retro), and never scold. Offer a lighter **travel mode** (one check-in a day) and, after any gap, restart without guilt: "Welcome back. Here's one thing for today." Routines like this often fade within a week; the coach's job is to make restarting easy.

## Step 6 — Save the manual

Fill `references/manual-of-me-template.md` with everything confirmed, keep *Not yet captured* where they skipped, and update the change log. Then follow `references/saving-the-manual.md`: recommend a private Claude Project, or Google Drive, or a folder on their computer. Never put the manual in the plugin repository.

**Never record**, even if shared: addresses, phone numbers, emergency contacts, ID numbers, medication names or doses. Never record anything about self-harm or crisis. If a diagnosis comes up, note only how it shows up day to day.

## Step 7 — End with a next step

Finish with something useful, chosen from what they told you:
- **If they're stuck on something now:** offer one recommended next task with a five-minute first step and a one-line reason.
- **Otherwise:** name the single highest-leverage thing from the manual (e.g., "consolidate your three task lists into one", "try a 15-minute focus sprint during your morning peak") and offer to do it now.
- **Always:** say what happens next ("Tomorrow at 8:45 I'll check in for your standup") and how to continue onboarding ("say 'finish my onboarding' when you have 10 minutes").
- **Celebrate:** a specific acknowledgement of the effort it took to do this.

## Updating the manual later

When the user says "update my manual" or a later skill learns something new:
- Show the section and the proposed change; apply it only after a yes.
- Add a change-log row.
- If an *(estimate)* or *(hypothesis)* item is confirmed or disproved, update its marker.
