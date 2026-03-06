# Review Focus

When reviewing code, design, or operational changes in this repository, prioritize the following areas.

## Highest Priority
1. correctness
2. operational safety
3. maintainability
4. observability
5. security
6. performance

## Specific Review Focus Areas

### Correctness
Check for:
- logical errors
- broken edge cases
- invalid assumptions
- bad state handling
- missing validation

### Operational Safety
Check for:
- unsafe deployment behavior
- weak rollback story
- partial failure risk
- poor timeout/retry handling
- hidden operational complexity

### Maintainability
Check for:
- confusing structure
- poor naming
- duplicated logic
- brittle code paths
- hard-coded assumptions

### Observability
Check for:
- missing logs
- poor error context
- lack of metrics or health visibility
- hard-to-debug failures

### Security
Check for:
- unsafe input handling
- secret leakage
- bad auth/authz assumptions
- excessive trust of external systems

### Performance
Check for:
- repeated expensive calls
- poor query patterns
- unnecessary loops or parsing
- scale risks

## Review Style
Claude should:
- be direct
- call out real risk over style trivia
- distinguish must-fix from should-fix
- prefer concrete recommendations