# Architecture Decision Records

## Decision 1: Three-Tier Architecture

### Why?

The application is separated into:

- Presentation Layer
- Application Layer
- Data Layer

Benefits:

- Independent scaling
- Better security
- Easier maintenance
- Reduced blast radius

---

## Decision 2: Aurora PostgreSQL

Aurora was selected because:

- Healthcare and claims workloads are relational
- ACID transaction support
- High Availability
- Automatic failover

---

## Decision 3: Multi-AZ Deployment

The system is deployed across multiple Availability Zones.

Benefits:

- Improved resiliency
- Reduced downtime
- Better disaster recovery
