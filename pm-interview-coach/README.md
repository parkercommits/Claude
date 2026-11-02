# PM Interview Coach

An adaptive interview coach for Claude. It preps you for specific interviews, scores your answers (real transcripts and practice) on five dimensions, finds the root cause behind weak spots, builds a storybank you can recall under pressure, and remembers your progress across chats.

**Current version:** 0.1.0. See [CHANGELOG.md](CHANGELOG.md).

Adapted from [Interview Coach](https://github.com/noamseg/interview-coach-skill) by Noam Segal (MIT), repackaged as a Claude plugin so it works in Claude chat on desktop, web and phone, not only in Claude Code.

## Install

- **Claude app — install from GitHub:** **Customize → Plugins → Add → Add marketplace → Add from a repository**, enter `parkercommits/Claude`, then install **PM Interview Coach**.
- **Claude app — upload the plugin file:** get the `.plugin` file from this repository's Releases page, then upload it under **Customize → Plugins**.
- **Claude Code:** `/plugin install pm-interview-coach --marketplace parkercommits/claude`

## Your first 10 minutes

Say **"kickoff"** (or "set up my interview coach") and share your résumé. The coach reviews it for positioning strengths, likely interviewer concerns and story seeds, asks about your target role and timeline, and creates your **Coaching State**.

## Where your progress lives: the Coaching State

One private document holds your profile, storybank, scores, interview loops and coaching notes. Every skill reads it first and updates it after major work. Kickoff helps you pick where it lives:

- **A Google Doc** (recommended if Google Drive is connected): the coach reads and saves it itself.
- **A private Claude Project**: the coach hands you the updated file at the end of each session to replace the old one.
- **A folder on your computer**, if the desktop app is linked to it.

It never goes in this repository.

## What you can say

| Say | What happens |
|---|---|
| "kickoff" | Set up your profile and Coaching State |
| "research [company]" | Quick company snapshot and fit check |
| "prep [company]" + the job description | Prep brief: format, interviewers, likely questions mapped to your stories, concerns, questions to ask, day-of cheat sheet |
| "hype" | Pre-interview confidence boost and a 3x3 plan |
| "debrief" | Same-day capture right after a real interview |
| "analyze" + a transcript | Five-dimension scoring, interviewer signals, a rewrite of your weakest answer, and the one bottleneck to fix |
| "practice" / "mock [format]" | Drills (constraint ladders, pushback, pivots, panels, technical communication) or a full mock interview |
| "stories" | Build and sharpen your storybank, with earned secrets |
| "concerns" / "questions" | Likely doubts and counters; questions to ask them |
| "thankyou" | Specific thank-you notes per interviewer |
| "progress" | Score trends, self-calibration, outcomes |
| "negotiate" | Offer negotiation with exact scripts |
| "reflect" | Post-search retrospective and archive |
| "help" | The full command list |

## How it scores

Every answer gets 1–5 on **Substance**, **Structure**, **Relevance**, **Credibility** and **Differentiation**, calibrated to your seniority. Scores map to root causes (narrative hoarding, status anxiety, conflict avoidance and others) and the coach picks the next drill from your actual bottleneck instead of running everyone through the same sequence.

## Works well with

- **ADHD Coach** (in this marketplace): when its `meeting-prep` spots a job interview, it asks whether you want PM Interview Coach's full prep or its own one-minute prep card.
- **Google Drive, Gmail, Calendar, and a meeting recorder such as Fireflies**: for the Coaching State, interview logistics and transcripts. All optional.

## Privacy

Your Coaching State and prep documents stay in your own space. Interviewer research uses public professional information only, and the coach says where each insight came from.
