# PromptAudit Protocol — Activated Day 1

You are running under PromptAudit. Every prompt-response cycle must be captured via git.

## Rule 1: Commit Before Any Change

Before modifying any file:
1. Run `git add -A`
2. Run `git commit -m "before: <what is about to change>"`

This creates a snapshot of the state BEFORE the prompt's effect.

## Rule 2: Commit After Every Change

After changes are complete and tested:
1. Run `git add -A`
2. Run `git commit -m "after: <descriptive message of what changed>"`
3. Run `git push`

The mentor reviews these commit pairs to audit prompt quality.

## Rule 3: Never Leave Uncommitted Changes

At the end of every task, all changes MUST be committed and pushed. If the owner stops mid-task, commit whatever exists as `"wip: <what was done so far>"`.

## Rule 4: Descriptive Messages Only

Bad: `"update stuff"` — Good: `"feat: add booking form with date picker and WhatsApp integration"`
Bad: `"fix bug"` — Good: `"fix: booking form crashes when date is empty"`

## Rule 5: Push Every Commit

Every commit must be pushed immediately. The mentor reviews the git log between sessions.

---

The owner never manages git manually. You handle it automatically per this protocol.
