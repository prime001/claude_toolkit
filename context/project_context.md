# Project Context

## Purpose
This repository contains the source code, configuration, automation, and supporting assets for this project.

The goal of this repository is to provide a maintainable, production-safe implementation that is easy for engineers to understand, modify, test, and operate.

## Primary Goals
- keep the system reliable and maintainable
- reduce manual operational effort
- support safe deployment and troubleshooting
- prefer clear architecture over clever implementation
- keep the codebase practical and production-oriented

## Intended Users
Primary users of this repository are:
- engineers maintaining and extending the system
- operators supporting the system in runtime environments
- reviewers validating correctness, safety, and maintainability

## Repository Priorities
When making recommendations or changes, prioritize in this order:

1. correctness
2. operational safety
3. maintainability
4. clarity
5. performance
6. speed of implementation

## Important Expectations
- assume code may run in production
- assume another engineer will inherit this code later
- prefer explicit behavior over hidden magic
- call out assumptions clearly
- recommend minimal, practical changes when possible

## Important Areas
Important parts of this repo may include:
- source code directories
- tests
- deployment/configuration files
- infrastructure definitions
- scripts and automation tools
- documentation

Update this section with real paths for the repo, for example:
- `src/`
- `tests/`
- `docker/`
- `scripts/`
- `docs/`

## How Claude Should Help
Claude should:
- use repo-specific context before giving generic advice
- preserve existing architecture unless there is a strong reason to change it
- be direct about risks and tradeoffs
- avoid unnecessary abstraction
- prefer implementation-ready outputs