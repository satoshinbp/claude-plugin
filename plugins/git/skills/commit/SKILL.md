---
name: commit
allowed-tools: Bash(git add:*), Bash(git status:*), Bash(git commit:*)
description: Create git commits following the conventional commits spec.
model: sonnet
effort: medium
---

## Context

- Current git status: !`git status`
- Current git diff (staged and unstaged changes): !`git diff HEAD`
- Current branch: !`git branch --show-current`
- Recent commits: !`git log --oneline -10`

## Your task

Analyze the changes above and create commits following the conventional commits spec.

1. **Group changes by concern**
   - Single concern → one commit
   - Multiple concerns → split into multiple non-breaking commits, one per concern
2. **For each concern, execute in order**
   - Stage the relevant files with `git add <files>`
   - Create the commit with `git commit`
3. Act immediately without asking for confirmation. Output no text other than tool calls.
