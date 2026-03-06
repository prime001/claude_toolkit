# NSO Reconcile Review Workflow

## Goal
Evaluate reconciliation or brownfield onboarding logic for safety, correctness, and explainability.

## Step 1 — Understand Identification Logic
Skills:
- `cisco_nso_expert`
- `debugging_specialist`

Expected output:
- how services are identified
- what evidence is used
- confidence level of matching logic
- risk areas

## Step 2 — Review Matching Heuristics
Use:
- `.claude/prompts/review.md`

Skills:
- `cisco_nso_expert`

Expected output:
- false positive risks
- false negative risks
- brittle parsing concerns
- grouping/ownership concerns
- maintainability issues

## Step 3 — Evaluate Operational Safety
Skills:
- `incident_responder`
- `staff_code_reviewer`

Expected output:
- rollback risks
- partial state risks
- logging/observability gaps
- operator explainability issues

## Step 4 — Recommend Fixes
Skills:
- `cisco_nso_expert`

Expected output:
- safer match criteria
- fallback behavior when confidence is low
- improved logs or evidence collection
- performance improvements

## Rules
- treat ownership inference as high risk
- do not assume brownfield data is clean
- prefer evidence-based matching over clever heuristics