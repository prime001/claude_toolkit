# Feature Development Workflow

Goal:
Implement a new feature in a safe, maintainable way.

## Step 1 — Design

Use:
.claude/prompts/build.md

Skills:
- network_architect
- cisco_nso_expert

Task:
Design the feature before implementing.

Produce:
- architecture
- data flow
- component changes
- risks

---

## Step 2 — Implementation

Use:
.claude/prompts/task.md

Skills:
- full_stack_engineer
- devops_engineer

Task:
Implement the feature.

Produce:
- code changes
- files modified
- explanation of implementation

---

## Step 3 — Review

Use:
.claude/prompts/review.md

Skills:
- staff_code_reviewer
- security_auditor
- performance_optimizer

Task:
Review the implementation.

Produce:
- critical issues
- security concerns
- maintainability issues

---

## Step 4 — Fix

Use:
.claude/prompts/fix.md

Skills:
- debugging_specialist
- full_stack_engineer

Task:
Fix issues discovered during review.

---

## Step 5 — Summary

Use:
.claude/prompts/summary.md

Skills:
- technical_writer

Produce:
- final explanation
- implementation notes
- follow-up improvements