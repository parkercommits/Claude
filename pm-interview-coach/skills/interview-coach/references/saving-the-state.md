# Saving the Coaching State

The Coaching State must be somewhere every future chat can read it, and it must stay private to the user. Offer the options below, recommend one, and walk through it one step at a time, waiting for the user to confirm each step. Interface labels change, so describe what to look for rather than insisting on exact button names.

Record the chosen location in the state's Profile (`Coaching State location`) so later sessions know where to look.

## Option A: Google Doc (recommended when Google Drive is connected)

Best for frequent updates, because the coach can read and save the doc itself.

1. Ask before creating anything. Then create a Google Doc named **"Interview Coach — Coaching State"** in the folder the user chooses, filled from `coaching-state-template.md`.
2. At the start of each session, read the doc. After each major workflow, update the affected sections in place. Don't rewrite sections that didn't change.
3. If Drive is disconnected mid-search, fall back to Option B for that session and tell the user which changes to bring back into the doc.

## Option B: A private Claude Project

Best when the user doesn't want to connect Google Drive.

1. **Give the user the Coaching State** as a Markdown file.
2. **Create a project** in Claude named "Interview Coach". Keep it private.
3. **Add project instructions.** Paste:

   ```
   This is my interview coaching space. The PM Interview Coach plugin is installed.
   - Before any coaching, read the "Coaching State" file in this project.
   - At the end of each session, give me the updated Coaching State file to replace the old one.
   ```

4. **Upload the Coaching State** to the project's files, plus the user's résumé and any job descriptions they're working from.
5. **Use the project** for coaching chats. The coach can't overwrite project files, so at the end of each session (or after a big workflow) it hands back the updated file, and the user replaces the old one.

## Option C: A folder on the user's computer

If the Claude desktop app links this chat to the user's computer and they prefer local files:

1. Ask which folder to use (e.g., `Documents/Interview Coach`), and request access to it.
2. Save `coaching_state.md` there, and update it after each major workflow.

## No storage yet

If the user wants to start coaching before choosing, coach from what's in the conversation. At the end, give them the state as a file and recommend Option A or B. If they come back without it, ask them to paste or upload it.

## Privacy

- The Coaching State holds the user's stories, scores, interview notes and job-search details. Never put it in the plugin or any shared location.
- Keep interviewer notes to public professional information. Don't record speculation about anyone's personal life.
- Before the user shares any prep document with a company, remind them to remove private notes (for example, details from earlier interviews or other offers).
