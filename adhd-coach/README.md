# ADHD Coach

A pocket ADHD coach for Claude. It learns how you work (your challenges, strengths, values, energy and the systems you've tried), then helps you at the moment you get stuck: deciding what to do next, planning your day around your energy, breaking down tasks you've been avoiding, and being kinder to yourself when things go sideways.

**Current version:** 0.1.0, onboarding only. See [CHANGELOG.md](CHANGELOG.md) and the roadmap below.

> ADHD Coach is a coaching tool, not medical or mental-health care. It doesn't diagnose, and it doesn't give medication or treatment advice. If you're in crisis, contact someone you trust or a crisis line (in the US, call or text 988).

## Install

- **Claude app — install from GitHub:** **Customize → Plugins → Add → Add marketplace → Add from a repository**, enter `parkercommits/Claude`, then install **ADHD Coach**.
- **Claude app — upload the plugin file:** get the `.plugin` file from this repository's Releases page, then upload it under **Customize → Plugins**.
- **Claude Code:** `/plugin install adhd-coach --marketplace parkercommits/claude`

## Your first 10 minutes

Say: **"Set up my ADHD coach."**

Pick a path:
- **Fast start** (about 10 minutes): what's going on right now, plus your tools and coaching preferences. Enough for the coach to plan tomorrow.
- **Full setup**: six short modules (5–10 minutes each), in one sitting or one a day.
- **Just tell me**: tap the microphone and talk. The coach turns your brain dump into a draft for you to correct.

Anything can be skipped or left for the coach to fill in. Come back any time with **"finish my onboarding."**

## What onboarding builds: your Manual of Me

A private, readable "user manual" for your brain that every coaching skill reads first:

- What's going on now: priorities, 60-day goals, your support team
- How ADHD shows up for you, and what has and hasn't worked
- Your tools, and one trusted master task list
- Energy: peak hours, dips, and the seven types of rest
- How you process information (e.g., visual, verbal, kinesthetic) and whether you think in systems or steps
- Strengths (including VIA or CliftonStrengths results), values and motivators
- Self-compassion (optionally, your Self-Compassion Test scores)
- How you like to be coached: tone, bluntness, vocabulary, and when the coach should check in

It also sets up **proactive check-ins** (morning standup, midday nudge, before meetings you flag, end-of-day retro) on the schedule you choose.

**Privacy:** your manual stays in your own space (a private Claude Project, your Google Drive, or a folder on your computer), never in this repository. It records how you work, not identifiers or medical details.

## Roadmap

| Release | Skills |
|---|---|
| **MVP** | `onboarding` ✓, `what-next`, `plan-my-day` (standup), `brain-dump`, `make-it-smaller`, `shutdown` (retro), `meeting-prep` |
| **v1** | `pause-before-send`, `focus-sprint`, `overwhelm-reset`, `in-case-of-fire`, `leaving-checklist`, `wins-log`, `best-self`, `self-compassion`, `weekly-review` |
| **v2** | `session-prep`, `support-map`, a visual dashboard |

## Built on

Ideas from the ADHD and coaching literature, including Russell Barkley's "point of performance" model, ADHD-adapted CBT, DBT skills, the ADDCA view of processing modalities, the VIA character strengths, Kristin Neff's self-compassion research, Saundra Dalton-Smith's seven types of rest, and the Reflected Best Self exercise. ADHD Coach links to their free resources rather than reproducing them.
