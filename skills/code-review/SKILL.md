---
name: code-review
description: Review a diff, PR, or changed files for correctness, style, and risk. Use when the user asks for a code review, PR review, or to look over changes.
---

# Code Review

## When to use

Trigger on: review this, check my diff, any issues in this PR.

## Instructions

1. Read the whole diff before writing anything.
2. Check, in order:
   - Logic errors and off-by-one mistakes
   - Error handling: swallowed exceptions, missing nil checks
   - Concurrency: shared state, missing locks, race windows
   - Security: injection, secrets in code, unsafe input handling
3. Report findings ordered by severity (critical first, nit last).
4. For each finding, quote the line and suggest a concrete fix.

## Output format

- `critical` - must fix before merge
- `warning` - should fix
- `nit` - optional polish

End with a one-line verdict: approve / approve with nits / request changes.
