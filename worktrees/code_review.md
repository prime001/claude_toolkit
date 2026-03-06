# Code Review Workflow

## Goal
Assess whether code is safe, maintainable, and ready for production.

## Step 1 — Review
Use:
- `.claude/prompts/review.md`
- `.claude/templates/code_review_template.md`

Skills:
- `staff_code_reviewer`
- `security_auditor`
- `performance_optimizer`

Expected output:
- summary
- critical issues
- maintainability concerns
- security concerns
- performance concerns
- verdict

## Step 2 — Prioritize
Classify findings as:
- must fix before merge
- should fix soon
- optional improvements

## Step 3 — Suggest Fixes
Skills:
- `full_stack_engineer`
- `debugging_specialist`

Expected output:
- specific fix recommendations
- safer patterns
- refactor examples when useful

## Rules
- prioritize correctness over style
- do not invent issues
- be direct and concrete