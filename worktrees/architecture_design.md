# Architecture Design Workflow

## Goal
Produce a scalable, maintainable architecture before implementation begins.

## Step 1 — Define Problem
Skills:
- `systems_architect`
- `product_strategist`

Expected output:
- problem statement
- functional requirements
- non-functional requirements
- scope and non-scope
- assumptions

## Step 2 — Design Architecture
Use:
- `.claude/templates/system_design_interview_template.md`

Skills:
- `systems_architect`
- `devops_engineer`
- `network_architect`

Expected output:
- high-level architecture
- component breakdown
- data flow
- deployment model
- reliability approach
- observability plan

## Step 3 — Evaluate Tradeoffs
Skills:
- `systems_architect`
- `security_auditor`
- `performance_optimizer`

Expected output:
- major design tradeoffs
- risks
- scaling limits
- security concerns
- operational complexity

## Step 4 — Implementation Plan
Skills:
- `technical_writer`

Expected output:
- build phases
- milestones
- dependencies
- validation and rollout plan

## Rules
- prefer simple boundaries
- design for operability
- call out unknowns explicitly