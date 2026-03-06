# Coding Standards

## General Principles
Code in this repository should be:
- readable
- maintainable
- explicit
- testable
- production-safe

Prefer clarity over cleverness.

## Structure
- keep modules focused
- keep functions cohesive
- avoid deeply nested control flow
- separate parsing, business logic, and rendering/integration logic where practical

## Naming
- use descriptive names
- avoid vague abbreviations unless they are standard in this repo/domain
- prefer names that reflect intent and behavior

## Error Handling
- fail clearly
- avoid swallowing exceptions silently
- include useful context in logs and errors
- use specific exception handling where possible

## Logging
- log meaningful operational events
- include enough context for debugging
- avoid noisy or redundant logs
- never log secrets

## Testing
- prefer deterministic tests
- test critical paths and failure paths
- avoid overly brittle tests
- test behavior, not implementation trivia

## Maintainability
- avoid duplication when it meaningfully improves maintainability
- do not over-abstract too early
- prefer straightforward code over clever patterns

## Review Expectations
Changes should be reviewed for:
- correctness
- readability
- safety
- maintainability
- performance where relevant

## Guidance for Claude
When generating code:
- align with existing repo patterns
- keep code concise but readable
- include comments only where they add real value
- favor implementation that another engineer can safely maintain