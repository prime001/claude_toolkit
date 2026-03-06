# Architecture

## High-Level Overview
This project is composed of a set of components that work together to deliver the system's required functionality.

Claude should reason about the system in terms of:
- clear component boundaries
- explicit data/control flow
- operational behavior
- deployment implications

## Major Components
Document the major components here.

Example structure:

### Frontend
Responsible for:
- user interface
- presentation logic
- client-side interactions

### Backend / API
Responsible for:
- business logic
- API endpoints
- validation
- orchestration

### Data Layer
Responsible for:
- persistence
- state management
- queries
- schema integrity

### Background Jobs / Workers
Responsible for:
- async processing
- scheduled tasks
- long-running actions
- integrations

### Observability
Responsible for:
- metrics
- logs
- tracing
- dashboards
- alerts

## System Boundaries
Claude should preserve clean boundaries between:
- presentation logic
- business logic
- data access
- infrastructure/deployment logic
- integration logic

Avoid mixing concerns unless there is a strong practical reason.

## Data Flow
Document the key data flow here.

Example:
1. request enters frontend or API
2. validation occurs
3. backend service processes request
4. data is read/written
5. logs/metrics are emitted
6. response is returned

## Deployment Model
Document how the system is deployed.

Example:
- local development via Docker Compose
- production via containers or VMs
- reverse proxy in front of services
- metrics collected by Prometheus
- dashboards in Grafana

## Operational Considerations
When making suggestions, Claude should consider:
- what happens if a component fails
- restart/retry behavior
- observability and debuggability
- safe upgrades and rollback
- partial failure handling

## Architecture Guidance
Prefer:
- simple component responsibilities
- clear APIs
- deterministic flows
- maintainable service boundaries

Avoid:
- hidden coupling
- duplicated responsibilities
- giant monolith functions or modules
- unnecessary architectural sprawl