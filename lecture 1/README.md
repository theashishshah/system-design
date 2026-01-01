# System Design – Day 1 Notes

## Why System Design Exists

System design exists to protect business from change:

-   scale
-   cost
-   failures
-   vendor lock-in

---

## Design Layers

### 1. Architectural Design

-   High-level components
-   Service boundaries
-   Communication paths

### 2. Logical Design (Business Logic)

-   Rules
-   Algorithms
-   Invariants
-   Consistency guarantees

### 3. Physical Design

-   CPU, memory, disk
-   Backup & restore
-   Redundancy
-   Availability

---

## Scope Definition

### Functional Scope

-   User-visible features
-   APIs

### Non-Functional Scope

-   Latency
-   Availability
-   Scalability
-   Operability

---

## Building Systems

-   Start small
-   Build incrementally
-   Avoid premature optimization
-   Build components, not tight coupling

---

## Core System Axes

-   Database
-   Caching
-   Scaling
-   Logging
-   Concurrency
-   Communication

---

## Database Design

-   Relational vs Non-relational
-   Separate OLTP and search
-   Use ElasticSearch for text search
-   Use soft deletes
-   Choose correct data types

---

## Caching

-   Exists at all levels
-   Reduces disk IO
-   Protects databases

### Types

-   Application cache
-   Centralized cache (Redis)
-   Distributed cache
-   CDN

### Write Strategies

-   Write-through
-   Write-around
-   Write-back

### Eviction Policies

-   FIFO
-   LIFO
-   LRU
-   MRU
-   LFU
-   Random

---

## Key Principles

-   Business logic must be isolated
-   Abstract vendor dependencies
-   Design for failure
-   Optimize for change
