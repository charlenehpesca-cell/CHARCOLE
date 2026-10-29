# Skill: Feedback → Proposal

Turn a correction or an improvement idea into a reviewable proposal instead of silently changing rules.

## When
- Charlene corrects the agent ("no, I'm on Windows", "rename that to THREVI")
- The agent makes a mistake a rule would have prevented
- A repeated task could be smoother with a new rule, skill or template

## Steps
1. Log the correction in `memory/feedback.md` (date, what happened, the correct behavior).
2. If it should change a rule, skill, template or AGENT.md, create
   `governance/proposals/YYYY-MM-DD-<short-slug>.md`:
   ```
   ---
   status: pending
   created: YYYY-MM-DD
   target: <file the change would edit>
   source: <correction | mistake | idea>
   ---

   # <Proposal title>

   ## Problem
   What happened or what's missing.

   ## Proposed change
   The exact text to add, change or remove in the target file.

   ## Why
   What this prevents or improves.

   ## Risk
   What could go wrong. "None" is allowed.
   ```
3. Don't apply the change. Commit `Propose: <title>` and push.
4. Tell Charlene in one line that a proposal is waiting.
