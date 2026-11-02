# Changelog

All notable changes to the PM Interview Coach plugin. Versions follow [semantic versioning](https://semver.org): minor versions add or expand skills; patch versions fix wording or errors.

## [0.1.0] — 2026-11-02

First release: Noam Segal's Interview Coach (a Claude Code project) repackaged as a Claude plugin.

### Added
- **`interview-coach`**: the orchestrator. Holds the shared rules from the original `CLAUDE.md` (priority hierarchy, operating rules, five-dimension rubric, seniority calibration, evidence sourcing, coaching voice, mode detection) and routes to the command skills.
- **15 command skills**, one per original command: `kickoff`, `research`, `prep`, `analyze`, `debrief`, `practice`, `mock`, `stories`, `concerns`, `questions`, `hype`, `thankyou`, `progress`, `negotiate`, `reflect`. Workflows are carried over from the original command references, with trigger descriptions written for Claude chat.
- **Shared references** under `skills/interview-coach/references/`: cross-cutting modules, differentiation, examples, role drills, detailed rubrics, storybank guide, transcript processing and the help list.
- **`coaching-state-template.md`**: the Coaching State structure, extracted from the original `coaching_state.md` format, plus a `Coaching State location` field.
- **`saving-the-state.md`**: where the Coaching State lives in Claude chat (Google Doc, private Claude Project, or a local folder) and how each option is saved.

### Changed from the original
- The local `coaching_state.md` file becomes the **Coaching State**, a private document in the user's own space, because Claude chat can't read or write files in a project folder.
- Internal links now point to skills and to `skills/interview-coach/references/`.
- Added "Working in Claude chat" guidance: optional connectors (Drive, Gmail, Calendar, meeting recorders), LinkedIn fallbacks, and phone-friendly prep files.
