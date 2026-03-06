# Bug Fix Workflow

Goal:
Identify root cause and implement a safe fix.

## Step 1 — Debugging

Use skills:

- debugging_specialist
- cisco_nso_expert
- network_architect

Analyze:

- logs
- metrics
- system behavior

Determine root cause.

---

## Step 2 — Fix

Use:
.claude/prompts/fix.md

Skills:
- debugging_specialist
- full_stack_engineer

Implement minimal fix.

---

## Step 3 — Review

Use:
.claude/prompts/review.md

Ensure fix does not introduce:

- regressions
- security issues
- performance problems

---

## Step 4 — Documentation

Use:
.claude/prompts/summary.md

Explain:

- root cause
- fix
- prevention steps