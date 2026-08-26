---
name: commit-message
description: Write a conventional commit message from a git diff. Use when the user asks to commit, write a commit message, or summarize staged changes.
---

# Commit Message

## Instructions

1. Run `git diff --staged` or read the provided diff.
2. Pick the type: feat / fix / docs / refactor / test / chore.
3. Subject line: imperative mood, 72 chars max, no trailing period.
4. Add a body only when the why is not obvious from the diff.

## Examples

- `feat: add retry with exponential backoff to http client`
- `fix: prevent duplicate rows when import runs twice`
- `docs: document the --dry-run flag`
