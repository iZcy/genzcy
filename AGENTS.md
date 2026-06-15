# PromptAudit Protocol — Activated Day 1

Every prompt must produce a before/after commit pair. The owner runs all git commands manually. This protocol ensures consistency.

## Rule 1: Before Every Prompt

Tell the owner to run:
```
git add -A
git commit -m "before: <what they're about to do>"
```

This snapshots the state before the prompt's effect.

## Rule 2: After Every Prompt

After changes are done and tested, tell the owner to run:
```
git add -A
git commit -m "after: <descriptive message of what changed>"
git push
```

## Rule 3: Never Leave Uncommitted Work

If the owner stops mid-task, they must commit whatever exists as `"wip: <what was done so far>"` and push.

## Rule 4: Descriptive Messages Only

Bad: `"update stuff"` — Good: `"feat: add booking form with date picker and WhatsApp integration"`
Bad: `"fix bug"` — Good: `"fix: booking form crashes when date is empty"`

## Rule 5: Push Every Commit

Every commit must be pushed to GitHub immediately. The mentor reviews the git log between sessions.

---

The owner manages git. You enforce the protocol by reminding them before and after every prompt.
