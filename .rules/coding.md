# Coding & Content Conventions

CHARCOLE is mostly Markdown for Obsidian. These conventions keep notes consistent and linkable.

## Files and folders
- Notes are `.md`. Note titles use Title Case with spaces (`Second Brain Setup.md`), matching how Obsidian shows them.
- Client folders use lowercase-hyphen slugs (`clients/hl-accelerator/`). Never rename one without following `.rules/safety.md`.
- Daily notes are `Daily/YYYY-MM-DD.md`.
- Zettelkasten titles are a full-sentence idea (`Clients buy outcomes, not hours.md`).
- Images and files go in `Attachments/` only.

## Note structure
- Start with YAML frontmatter when a template defines it. Common keys: `type` (daily, project, area, resource, zettel, inbox, moc), `status`, `created`, `source`.
- One `# H1` per note, matching the filename.
- Create new notes from `Templates/` when a template exists for that type.

## Links
- Link between notes with `[[wikilinks]]`, not Markdown paths.
- Every new Zettelkasten or Resource note links to at least one existing note.
- Don't link from personal or PARA notes to a specific client's details; link to the client folder name at most.

## Writing
- Charlene's own messages follow `00_Resources/voice-principles.md`. Client-facing copy follows that client's `brand/`.
- Short paragraphs; bullets only when the content is list-shaped.
- Dates are ISO (`2026-10-29`). Timezone is Asia/Manila.

## Config
- `.obsidian/` settings are shared across devices. Change only the specific key needed; never rewrite the folder.
- `.obsidian/workspace*.json` stays ignored.

## Code and automations
- TODO: conventions for GHL (GoHighLevel) workflows, scripts or automation exports for client builds (e.g. THREVI), once any are stored here.
- Scripts, if added, live in `playbooks/scripts/` with a comment header: what it does, inputs, who it's for.
