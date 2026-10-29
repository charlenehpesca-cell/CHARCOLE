# MEMORY.md — Cross-Session Index

Read this after AGENT.md and CLAUDE.md. Keep it under 200 lines: it points to detail, it doesn't hold it. Rules belong in CLAUDE.md or `.rules/`. Client facts belong in that client's own MEMORY.md.

## Memory files

| File | What's in it | Read it when |
| --- | --- | --- |
| `memory/user.md` | Charlene's role, setup and preferences | Every session (short) |
| `memory/feedback.md` | Corrections she has given | Before repeating a kind of task |
| `memory/project.md` | State of CHARCOLE and key decisions | Changing structure, settings or sync |
| `memory/reference.md` | URLs, paths, IDs, versions | Needing a link, path or tool detail |

## Clients

Details live in each folder; load only the one the task needs.

- THREVI: GHL CRM build, `clients/threvi/`
- HL Accelerator: `clients/hl-accelerator/`
- OneSource: `clients/onesource/`
- Pau Parreno: `clients/pau-parreno/`
- Ivy Woolfturk: `clients/ivy-woolfturk/`

## Active work

- Second brain setup, see `10 - Projects/Second Brain Setup.md`
- Open TODOs across sessions are in `governance/remaining-todos.md`

## Latest checkpoint

_None yet. `.skills/checkpoint.md` writes the most recent one here (one entry, overwrite each time)._

## Key contacts

_TODO: people not tied to one client._
