# Senior Software Engineer System Design Roadmap

## Goal

Transition from:

```text
Feature Developer
        ↓
Senior Engineer
        ↓
System Designer
        ↓
Architect
```

Focus on:

- Scalability
- Distributed Systems
- Cloud Architecture
- Reliability
- Event-Driven Systems
- Production Engineering

---

# Phase 1: System Design Fundamentals

## Duration

2-3 Weeks

## Topics

### Scalability

- Vertical Scaling
- Horizontal Scaling
- Tradeoffs

### Networking

- DNS
- TCP/IP
- HTTP/HTTPS
- TLS
- Reverse Proxy

### Load Balancing

- Layer 4
- Layer 7
- Round Robin
- Least Connections

### Caching

- Browser Cache
- CDN Cache
- Application Cache
- Database Cache

### Databases

- SQL
- NoSQL
- ACID
- BASE

### Distributed Systems

- CAP Theorem
- Consistency
- Availability
- Partition Tolerance

### Reliability

- Replication
- Failover
- High Availability

## Deliverables

Create notes for:

```text
system-design-notes/
├── scaling.md
├── load-balancer.md
├── caching.md
├── databases.md
├── cap-theorem.md
├── replication.md
```

---

# Phase 2: Production Ready Monolith

## Duration

3-4 Weeks

## Project

Rent Management System

## Features

### Authentication

- JWT
- Refresh Tokens
- RBAC

### Database

- PostgreSQL
- Indexing
- Pagination

### Infrastructure

- Docker
- Docker Compose

### Storage

- S3

### Caching

- Redis

### Monitoring

- Logs
- Metrics
- Health Checks

### CI/CD

- GitHub Actions
- Jenkins

## Learn

### Database Optimization

- Query Plans
- Indexing
- N+1 Problems

### Performance

- Caching
- Connection Pooling

## Deliverable

Production-grade monolith.

---

# Phase 3: Authentication Service

## Duration

2-3 Weeks

## Project

Standalone Auth Service

## Features

### User Management

- Signup
- Login
- Forgot Password
- Reset Password

### Security

- JWT
- Refresh Tokens
- MFA

### Authorization

- RBAC
- Permissions
- Roles

### Sessions

- Device Tracking
- Session Management

### Security Controls

- Rate Limiting
- Account Locking
- Token Revocation

## Database

```text
users
roles
permissions
user_roles
sessions
refresh_tokens
audit_logs
```

## Learn

- Authentication Architecture
- Authorization Models
- Security Design

---

# Phase 4: Event Driven Architecture

## Duration

3-4 Weeks

## Project

Banking Subscription Platform

## Services

```text
Customer Service
Subscription Service
Asset Service
Notification Service
Audit Service
```

## Communication

### Synchronous

```text
REST APIs
```

### Asynchronous

```text
Kafka
```

## Events

```text
CustomerCreated
SubscriptionCreated
AssetCreated
UserInvited
RoleAssigned
```

## Learn

### Kafka

- Topics
- Partitions
- Consumer Groups

### Reliability

- Retries
- Dead Letter Queues
- Idempotency

### Consistency

- Eventual Consistency
- Distributed Transactions

## Deliverable

Architecture diagram and working project.

---

# Phase 5: Microservices Architecture

## Duration

4 Weeks

## Convert Existing Project

From:

```text
Monolith
```

To:

```text
Microservices
```

## Services

```text
Auth Service
User Service
Subscription Service
Asset Service
Audit Service
Notification Service
```

## Add

### API Gateway

- Request Routing
- Authentication

### Service Discovery

- Eureka
- Consul

### Configuration

- Central Config

### Communication

- REST
- Kafka

## Learn

### Service Boundaries

- Domain Driven Design

### Reliability

- Circuit Breakers
- Bulkheads

### Transactions

- Saga Pattern

---

# Phase 6: Observability

## Duration

2 Weeks

## Topics

### Logging

- Structured Logs

### Monitoring

- Prometheus

### Visualization

- Grafana

### Tracing

- OpenTelemetry
- Jaeger

## Learn

### Golden Signals

- Latency
- Traffic
- Errors
- Saturation

## Deliverable

Observability Stack

```text
Application
      |
Prometheus
      |
Grafana
```

---

# Phase 7: Distributed Systems

## Duration

4 Weeks

## Learn

### Data Replication

- Primary Replica
- Multi Region

### Partitioning

- Sharding

### Consensus

- Leader Election

### Consistency

- Strong Consistency
- Eventual Consistency

### Distributed Locks

- Redis Locks

### Messaging

- Kafka Internals

## Book

Designing Data-Intensive Applications

Read:

- Replication
- Partitioning
- Transactions
- Streams

---

# Phase 8: Cloud Architecture

## Duration

4 Weeks

## AWS Services

### Compute

- EC2
- ECS
- EKS
- Lambda

### Database

- RDS
- DynamoDB

### Messaging

- SQS
- SNS
- MSK

### Networking

- VPC
- Route53
- ALB

### Security

- IAM
- Secrets Manager

### Monitoring

- CloudWatch

## Infrastructure as Code

### Learn

- AWS CDK

or

- Terraform

## Deliverable

Deploy all projects to AWS.

---

# Phase 9: Large Scale Systems

## Duration

4 Weeks

## Design These Systems

### Beginner

- URL Shortener
- Notification Service
- File Storage Service

### Intermediate

- Chat Application
- Food Delivery Platform
- E-commerce Platform

### Advanced

- Uber
- YouTube
- Netflix
- WhatsApp
- LinkedIn

## For Every Design

### Requirements

- Functional
- Non Functional

### Capacity Estimation

- Users
- Requests
- Storage

### APIs

- Endpoints

### Database Design

- Tables
- Sharding Strategy

### High Level Design

- Components

### Scaling Strategy

- Caching
- Replication
- Partitioning

### Failure Handling

- Retries
- Circuit Breakers

---

# Phase 10: Architecture Patterns

## Learn

### Monolith

### Modular Monolith

### Microservices

### Event Driven

### CQRS

### Event Sourcing

### Hexagonal Architecture

### Clean Architecture

### Domain Driven Design

## Deliverable

Implement at least:

- Modular Monolith
- Event Driven Architecture
- Microservices

---

# Books

## Must Read

### Designing Data-Intensive Applications

Topics:

- Replication
- Partitioning
- Transactions
- Streams

### Head First Design Patterns

Topics:

- Strategy
- Factory
- Observer
- Decorator

### Clean Architecture

Topics:

- Architectural Boundaries
- SOLID Principles

---

# Blogs

## Netflix Tech Blog

Learn:

- Reliability
- Distributed Systems

## Uber Engineering

Learn:

- Marketplace Systems
- Event Driven Systems

## Stripe Engineering

Learn:

- Payments
- Idempotency

## AWS Architecture Blog

Learn:

- Cloud Native Architecture

---

# Final Portfolio Projects

## Project 1

Production Ready Rent Management System

Skills:

- Spring Boot
- PostgreSQL
- Redis
- Docker
- AWS

---

## Project 2

Authentication Platform

Skills:

- JWT
- OAuth
- RBAC
- MFA

---

## Project 3

Banking Subscription Platform

Skills:

- Kafka
- Event Driven Architecture
- Saga Pattern

---

## Project 4

Microservices Migration

Skills:

- Service Discovery
- API Gateway
- Distributed Systems

---

## Project 5

E-commerce Platform

Skills:

- Search
- Inventory
- Payments

---

## Project 6

Uber Style Design

Skills:

- Geospatial Queries
- Real Time Systems
- WebSockets

---

# Expected Outcome

After completing this roadmap you should be comfortable discussing:

- HLD
- LLD
- Microservices
- Kafka
- Redis
- PostgreSQL Internals
- Scaling
- Distributed Systems
- Event Driven Architecture
- Authentication Architecture
- API Gateways
- Observability
- AWS Architecture
- Reliability Engineering
- Production Systems

This is typically the knowledge expected from Senior Software Engineers (4-8 years), and it also forms the foundation for Staff Engineer and Solution Architect roles.
