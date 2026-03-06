# Incident Response Workflow

## Goal
Restore service safely, identify root cause, and capture prevention steps.

## Step 1 — Assess Impact
Skills:
- `incident_responder`

Expected output:
- affected systems
- user impact
- severity
- suspected timeline
- recent changes

## Step 2 — Stabilize
Skills:
- `incident_responder`
- `devops_engineer`

Expected output:
- immediate mitigation options
- lowest-risk stabilization path
- rollback or containment advice

## Step 3 — Investigate Root Cause
Use:
- `.claude/templates/incident_response_template.md`

Skills:
- `incident_responder`
- `debugging_specialist`

Expected output:
- evidence
- likely cause
- confirmed root cause if available
- unresolved unknowns

## Step 4 — Recover
Expected output:
- recovery actions
- validation checks
- service restoration criteria

## Step 5 — Prevent Recurrence
Skills:
- `technical_writer`

Expected output:
- monitoring improvements
- testing gaps
- config or process changes
- postmortem summary

## Rules
- prioritize safe restoration first
- avoid risky changes during incident mitigation unless necessary