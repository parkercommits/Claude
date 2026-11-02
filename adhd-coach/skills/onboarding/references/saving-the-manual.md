# Saving the Manual of Me

The manual must be somewhere every future chat can read it, and it must stay private to the user. Offer the options below in this order of preference, recommend one, and walk through it one step at a time, waiting for the user to confirm each step. Interface labels change; describe what to look for rather than insisting on exact button names.

## Option A — A private Claude Project (recommended)

1. **Give the user the manual** as a Markdown file (or a Word file if they prefer).
2. **Create a project** in Claude named "ADHD Coach". Keep it private; don't share it.
3. **Add project instructions.** Paste:

   ```
   This is my ADHD coaching space. The ADHD Coach plugin is installed.
   - Before any coaching, read the "Manual of Me" file in this project.
   - Coach the way section 14 of my manual describes.
   - Propose changes to my manual instead of editing it silently.
   ```

4. **Upload the manual** to the project's files, plus any assessment results the user wants the coach to see (strengths reports, Self-Compassion Test scores).
5. **Use the project** for coaching chats from now on. When the manual changes, the coach gives the user an updated file to replace the old one.

## Option B — Google Drive

1. If Google Drive is connected, offer to create the manual as a Google Doc named "Manual of Me — ADHD Coach" in a folder the user chooses (ask before creating it). Otherwise give them the file to upload.
2. Note the doc's location in the manual's §4 so later skills know where to look.
3. Remind the user to keep Google Drive connected in Claude so skills can read and update it.

## Option C — A folder on the user's computer

If the Claude desktop app links this chat to the user's computer and they prefer local files:

1. Ask which folder to use (e.g., `Documents/ADHD Coach`), and request access to it.
2. Save `manual-of-me.md` there.
3. Note the location in §4.

## Keeping it current

- Skills propose updates; the user approves; the change log records each one.
- The weekly review proposes edits based on experiments.
- Offer a fuller refresh every three months, including a Self-Compassion Test retake if the user took it.
- **Blind refresh:** for the refresh, have the user answer the Module 1 and Module 6 questions again *without* looking at their earlier answers, then compare the two side by side. What changed is often the most useful thing to talk about.
