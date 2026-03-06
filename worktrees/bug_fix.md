# Bug Fix Workflow

## Goal
Find the real root cause, implement the smallest safe fix, and prevent recurrence.

## Step 1 — Triage
Skills:
- `debugging_specialist`
- `incident_responder`

Expected output:
- problem summary
- observed symptoms
- possible root causes ranked by likelihood
- affected scope

Gather evidence before suggesting fixes.

## Step 2 — Root Cause Analysis
Use:
- `.claude/templates/incident_response_template.md`

Skills:
- `debugging_specialist`
- `devops_engineer`

Expected output:
- likely root cause
- supporting evidence
- why the system allowed it
- validation checks

## Step 3 — Fix
Use:
- `.claude/prompts/fix.md`

Skills:
- `debugging_specialist`
- `full_stack_engineer`

Expected output:
- minimal fix
- explanation of why it resolves the issue
- validation steps

## Step 4 — Review
Use:
- `.claude/prompts/review.md`

Skills:
- `staff_code_reviewer`

Expected output:
- regression risks
- operational risks
- follow-up improvements

## Step 5 — Prevention
Skills:
- `technical_writer`
- `incident_responder`

Expected output:
- monitoring improvements
- logging improvements
- test additions
- config or architecture changes to prevent recurrence

## Rules
- do not confuse symptoms with root cause
- prefer minimal safe fixes
- preserve working behavior