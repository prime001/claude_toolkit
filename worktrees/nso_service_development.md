# NSO Service Development Workflow

## Goal
Design and implement Cisco NSO service logic that is correct, idempotent, maintainable, and safe in production.

## Step 1 — Service Design
Use:
- `.claude/prompts/build.md`

Skills:
- `cisco_nso_expert`
- `systems_architect`
- 'network_architect'

Expected output:
- service purpose
- YANG model approach
- Python vs template split
- lifecycle considerations
- FASTMAP and ownership considerations
- reconciliation impact
- risks

## Step 2 — Implementation
Use:
- `.claude/prompts/task.md`

Skills:
- `cisco_nso_expert`

Expected output:
- YANG model
- Python service logic
- template structure
- helper functions
- assumptions
- performance notes

## Step 3 — Review
Use:
- `.claude/prompts/review.md`

Skills:
- `cisco_nso_expert`
- `staff_code_reviewer`

Expected output:
- idempotency concerns
- FASTMAP concerns
- ownership/reconcile risks
- MAAPI efficiency concerns
- maintainability issues
- operational risks

## Step 4 — Fix
Use:
- `.claude/prompts/fix.md`

Skills:
- `cisco_nso_expert`
- `debugging_specialist`

Expected output:
- corrected code/model/template
- explanation of fixes
- remaining risks

## Step 5 — Summary
Skills:
- `technical_writer`

Expected output:
- service design summary
- files changed
- important behavior notes
- follow-up work

## Rules
- prefer clear service boundaries
- prioritize idempotency and operational clarity
- minimize unnecessary MAAPI tree walks
- treat brownfield assumptions as risky