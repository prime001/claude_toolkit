# System Design Template

Use this template when designing or evaluating a complex system.  
The goal is to produce a **clear, structured architecture explanation** that engineers can implement and operate.

---

# 1. Problem Definition

## Problem Summary
Describe the problem the system must solve.

Include:
- the primary goal of the system
- what users or systems interact with it
- expected outcomes

## Scope
Define what is **in scope** and **out of scope**.

This prevents unnecessary complexity.

## Key Use Cases
List the most important user interactions or system operations.

Example:

- create resource
- retrieve resource
- update resource
- background processing

---

# 2. Requirements

## Functional Requirements
Describe what the system must do.

Examples:

- users can upload files
- system stores and retrieves data
- system processes tasks asynchronously

## Non-Functional Requirements
Define system qualities such as:

- scalability
- reliability
- latency targets
- security expectations
- durability

Example:

- API latency < 200ms
- system supports 100k concurrent users
- uptime target 99.9%

---

# 3. High-Level Architecture

Provide a top-level architecture diagram or description.

Explain:

- major system components
- how components interact
- external dependencies

Typical components include:

- clients
- API services
- background workers
- data stores
- message queues
- monitoring systems

---

# 4. Component Design

Describe the responsibilities of each component.

Example:

## API Service
Handles:
- request validation
- business logic
- authentication

## Worker Services
Handles:
- background tasks
- scheduled jobs
- async processing

## Data Layer
Handles:
- persistence
- indexing
- querying

---

# 5. Data Model

Describe key entities and relationships.

Include:

- primary data objects
- relationships between objects
- indexing strategy

Example:

Entity:
User
Fields:
- id
- email
- created_at

---

# 6. Data Flow

Explain how data moves through the system.

Example request flow:

1. client sends request
2. request hits load balancer
3. API service validates request
4. business logic runs
5. database updated
6. response returned

Also describe background workflows if relevant.

---

# 7. Scalability Strategy

Explain how the system scales.

Consider:

- horizontal scaling
- stateless services
- load balancing
- sharding
- caching

Example techniques:

- CDN
- Redis cache
- message queues
- database replication

---

# 8. Reliability and Fault Tolerance

Describe how the system handles failures.

Include:

- retries
- timeouts
- circuit breakers
- failover strategies

Explain how the system behaves when:

- services crash
- databases fail
- external APIs are unavailable

---

# 9. Performance Optimization

Identify potential bottlenecks.

Consider:

- database queries
- network latency
- serialization overhead
- resource contention

Explain strategies such as:

- caching
- batching
- asynchronous processing

---

# 10. Observability

Explain how the system will be monitored.

Include:

## Logging
Structured logs for debugging.

## Metrics
Examples:

- request latency
- error rates
- queue backlog

## Alerts
Define when operators should be notified.

---

# 11. Security Considerations

Discuss:

- authentication
- authorization
- data encryption
- rate limiting
- input validation

Ensure sensitive data is protected.

---

# 12. Deployment Model

Explain how the system runs in production.

Include:

- containerization
- orchestration platform
- configuration management
- secrets management

Example:

- Docker containers
- Kubernetes cluster
- environment-based configuration

---

# 13. Tradeoffs

Explain important design tradeoffs.

Examples:

- consistency vs availability
- complexity vs performance
- cost vs scalability

Be explicit about why decisions were made.

---

# 14. Risks and Unknowns

Identify potential risks.

Examples:

- scaling limits
- operational complexity
- integration risks

List questions that need further validation.

---

# 15. Future Improvements

Suggest possible future enhancements.

Examples:

- caching layers
- additional data partitioning
- improved observability
- advanced traffic routing

---

# Design Principles

Always prefer:

- simplicity
- clear boundaries
- observable systems
- production safety
- maintainable architecture

Avoid unnecessary complexity or premature optimization.