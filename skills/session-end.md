# Skill: Session End

Wrap up a work session so the next one starts smarter.

## When
- Charlene says she's done, "wrap up", "end session", or a deliverable is finished.

## Steps
1. `git pull`.
2. **Deliverables:** update `deliverables.md` for any client worked on (status, due date).
3. **Facts:** save new facts, decisions and contacts Charlene stated or confirmed:
   - client facts → `clients/<client>/MEMORY.md`
   - project state and decisions → `memory/project.md`
   - her preferences → `memory/user.md`
   - links, paths and IDs → `memory/reference.md`
4. **Corrections:** if she corrected anything, log it in `memory/feedback.md`, and run `skills/feedback.md` if a rule should change.
5. **TODOs:** add or tick items in `governance/remaining-todos.md`.
6. **Daily note:** add a one-line log entry to today's `Daily/YYYY-MM-DD.md` (create it from `Templates/Daily Note.md` if missing). Personal summary only; no client details beyond the client name.
7. Clear **Latest checkpoint** in `MEMORY.md` if the task is fully done.
8. Commit `Session end: <summary>` and push.
9. Reply with: what was done, what's next, anything waiting on her.
