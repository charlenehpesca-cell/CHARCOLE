# AGENT.md — Living Constitution

Loaded at the start of every session, before anything else. This file says **how the agent works** in CHARCOLE. `CLAUDE.md` says **what I prefer and where things go**. If they conflict, `.rules/safety.md` wins, then this file, then CLAUDE.md.

## What this repo is

CHARCOLE is Charlene's private second brain: one GitHub repo (`charlenehpesca-cell/CHARCOLE`) synced to an Obsidian vault on her Windows PC and read by Claude on every device. It holds notes, not code: client folders, personal business notes, playbooks, a PARA + Zettelkasten vault, and this governance layer.

## Load order (every session)

1. `AGENT.md` (this file)
2. `CLAUDE.md`: preferences, rules, Routing Map
3. `MEMORY.md`: cross-session index, then only the `memory/` files the task needs
4. `.rules/safety.md` always; `.rules/operations.md` before changing files; `.rules/coding.md` before writing notes, scripts or config
5. The one folder the Routing Map points to. Nothing else.

For client work, load only `clients/<client>/` plus steps 1–4. Never open another client's folder in the same task.

## Core principles

1. **Clients stay separate.** No client's information, files or decisions leak into another client's work, into `personal/`, or into the PARA folders.
2. **Nothing is lost.** Archive instead of delete. Git history is never rewritten.
3. **No secrets in the repo.** Passwords, API keys and tokens never get written here; note where they live instead.
4. **Every change syncs.** Pull before editing, commit and push after.
5. **Memory is earned.** Save facts Charlene states or confirms. Don't save guesses.
6. **Rules change through proposals.** The agent never edits AGENT.md or `.rules/` on its own initiative; it files a proposal (see below).

## Skills (procedures)

| Skill | Use when |
| --- | --- |
| `.skills/checkpoint.md` | Before switching task, client or device, or when a session is getting long |
| `.skills/session-end.md` | Charlene says she's done, or a piece of work wraps up |
| `.skills/feedback.md` | Charlene corrects the agent, or the agent spots a rule that would have prevented a mistake |
| `.skills/review-proposals.md` | Charlene asks to review proposals, or more than 3 are pending |

## Governance loop

1. A correction or idea comes up, and `feedback.md` files it in `governance/proposals/`.
2. Charlene reviews it with `review-proposals.md`: approve, reject or edit.
3. Approved changes are applied to the target file and logged in `governance/learnings-log.md`.
4. Open items across sessions live in `governance/remaining-todos.md`.

## Amending this file

Only through an approved proposal, or when Charlene directly asks for a change in chat. Every amendment gets a line in `governance/learnings-log.md`.

_Last amended: 2026-10-29 (created)._
