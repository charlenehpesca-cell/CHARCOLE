# Skill: Checkpoint

Save state so work can resume cleanly in another chat, on another device, or after a context switch.

## When
- Switching client, task or device
- The conversation is long and context may be lost
- Charlene says "checkpoint", "save progress" or "pause here"

## Steps
1. `git pull`.
2. Write a short entry under **Latest checkpoint** in `MEMORY.md` (replace the previous one):
   ```
   - YYYY-MM-DD HH:mm — <task> (<client or personal>)
     - Done: <what's finished>
     - Next: <the very next action>
     - Files: <paths touched>
     - Open question: <if any>
   ```
3. If the work is client-specific, also add the "Next" line to that client's `MEMORY.md` under Active projects. Never put client details in root MEMORY.md beyond the task name.
4. Add any unfinished item that will outlive this session to `governance/remaining-todos.md`.
5. Commit `Checkpoint: <task>` and push.
6. Tell Charlene in one line what was saved and what the next action is.
