# Feature Development Workflow

## Goal
Design, implement, review, and summarize a new feature in a maintainable way.

## Step 1 — Design
Use:
- `.claude/prompts/build.md`
- `.claude/templates/feature_design_template.md`

Skills:
- `systems_architect`
- `full_stack_engineer`

Expected output:
- feature overview
- architecture impact
- component changes
- data flow
- implementation plan
- risks

Do not start coding until the design is clear.

## Step 2 — Implement
Use:
- `.claude/prompts/task.md`

Skills:
- `full_stack_engineer`
- `devops_engineer`

Expected output:
- files to create or modify
- implementation code
- notes on decisions and tradeoffs
- testing considerations

Keep implementation aligned with repo constraints and coding standards.

## Step 3 — Review
Use:
- `.claude/prompts/review.md`
- `.claude/templates/code_review_template.md`

Skills:
- `staff_code_reviewer`
- `security_auditor`
- `performance_optimizer`

Expected output:
- critical issues
- maintainability issues
- security concerns
- performance concerns
- recommended fixes

## Step 4 — Fix
Use:
- `.claude/prompts/fix.md`

Skills:
- `debugging_specialist`
- `full_stack_engineer`

Expected output:
- corrected implementation
- explanation of changes
- remaining risks
- validation steps

## Step 5 — Summarize
Use:
- `.claude/prompts/summary.md`

Skills:
- `technical_writer`

Expected output:
- final feature summary
- files changed
- key design decisions
- open follow-up items

## Rules
- do not skip design
- do not make large rewrites unless justified
- prefer minimal, maintainable changes
- call out assumptions explicitly