# Saving the company profile for the team

Recommend **a Claude Project in the team's own Claude workspace** by default: the profile and source files sit next to every PMM chat, and on Team or Enterprise plans the project can be shared with colleagues. Offer a **shared Google Drive folder** if the team prefers Drive or the user's plan doesn't support project sharing. Either way, the data stays in the company's own accounts — never in the public plugin repository.

Walk the user through it one step at a time, in plain language, and wait for them to confirm each step. Interface labels change over time; describe what to look for rather than insisting on exact button names.

## Option A — Claude Project (recommended)

1. **Download the profile.** Give the user the finished company profile as a file (Markdown or Word, their choice), plus the health check report.
2. **Create the project.** In Claude, open Projects and create a new project named "[Company] PMM".
3. **Add the project instructions.** Paste this into the project's instructions:

   ```
   This is [Company]'s product marketing workspace. The PMM Framework plugin is installed.
   - Before any PMM task, read the "[Company] — PMM Company Profile" file in this project and
     treat it as the approved baseline.
   - Audit and build on existing work in this project before creating anything new.
   - Follow section 4 (Brand voice and copy rules) for anything customer-facing.
   - Propose changes to the profile rather than editing it silently; note the section owner.
   - Deliver outputs where section 8 says they should go.
   - Coach mode: [on / off]. When on, briefly explain why each step matters.
   ```

4. **Upload files to the project's knowledge.** The company profile first, then the most useful source documents: brand or tone-of-voice guidelines, current positioning or messaging docs, segmentation or persona work, the pricing sheet, the GTM calendar or plan, recent launch reviews. For call transcripts, upload a small representative sample (e.g., 10–15 recent calls across segments) or, better, connect the call recording tool so skills can pull fresh calls.
5. **Share it with the team** (Team and Enterprise plans). Use the project's Share option to add colleagues; give "Can edit" to people who will maintain the profile and "Can view" to everyone else.
6. **Each teammate installs the plugin and connects their own tools.** Connections are per person. An organization admin may be able to install the plugin for everyone and may need to allow the plugin's source; point them to the plugin README.

## Option B — Shared Google Drive folder

1. Create a folder such as "PMM / Company profile" in the team's shared drive.
2. If Google Drive is connected, offer to create the profile there as a Google Doc; otherwise give the user the file to upload.
3. Add the same source documents to the folder.
4. Share the folder with the team using Drive's normal permissions.
5. Note the folder in profile section 8, and remind users to connect Google Drive in Claude so skills can read it.

## Keeping it current

- Section owners update their sections; the change log records it.
- Grow's quarterly review proposes profile updates for owners to approve.
- Re-run the health check quarterly (or offer to schedule it) and update section 0.
