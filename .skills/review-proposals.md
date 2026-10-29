# Skill: Review Proposals

Let Charlene approve, edit or reject pending improvements.

## When
- She asks to review proposals, or more than 3 are pending.

## Steps
1. `git pull`. List every file in `governance/proposals/` with `status: pending`.
2. For each, show: title, target file, the proposed change, and why. Keep it to a few lines each.
3. Ask for a decision on each: **approve**, **edit** (she gives the wording), or **reject**.
4. **Approve / edit:** apply the change to the target file exactly as approved. Set the proposal's `status: approved` (or `approved-with-edits`) and add `decided: YYYY-MM-DD`.
5. **Reject:** set `status: rejected`, add `decided:` and a one-line reason.
6. Log every decision in `governance/learnings-log.md`:
   `| YYYY-MM-DD | <proposal> | <target file> | approved/rejected | <one-line summary> |`
7. Leave decided proposals in place as the audit trail; never delete them.
8. Commit `Review proposals: <n> approved, <n> rejected` and push.
