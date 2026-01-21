# Model — Usage Attribution Semantics

This document defines the **conceptual reference model**
for **usage attribution** in machine-to-machine and system-to-system environments.

The model describes how **measurable activity**
is linked to an **accountable entity** before any billing or settlement logic applies.

---

## Model Overview

The Usage Attribution reference model consists of **three sequential layers**:

1. Event
2. Usage
3. Attribution

Each layer refines the previous one.
Attribution is only valid when all prior layers are resolved.

---

## Layer 1 — Event

An **Event** represents an observable, machine-generated action
or state change with operational relevance.

### Characteristics
- Emitted by a system, agent, or automated process
- Timestamped and uniquely identifiable
- Contextualized by source, target, and execution environment

### Examples (non-exhaustive)
- API request execution
- Task initiation or completion
- Resource activation or release
- State transition affecting availability or capacity

Events alone do not establish responsibility.
They form the raw input for usage determination.

---

## Layer 2 — Usage

**Usage** represents quantified or qualified activity
derived from one or more events.

### Characteristics
- Aggregates or normalizes events
- Defines units of measure (time, volume, executions, distance, etc.)
- Filters non-qualifying or duplicate events
- Establishes boundaries for measurement periods

### Purpose
Usage answers:
> “What happened, and to what measurable extent?”

Usage does not assign responsibility.

---

## Layer 3 — Attribution

**Attribution** links measured usage to an **accountable entity**.

### Characteristics
- Resolves which entity is responsible for the usage
- Supports direct, delegated, and proxied execution
- Allows one-to-one, one-to-many, and hierarchical attribution
- Operates independently of billing or settlement logic

### Purpose
Attribution answers:
> “Who is accountable for this usage?”

Without attribution, usage cannot be meaningfully evaluated or settled.

---

## Layer Independence

- Layers must be evaluated **in order**
- Outputs of one layer become inputs to the next
- Attribution cannot be inferred directly from raw events

Skipping layers leads to ambiguous or non-reproducible attribution.

---

## Model Discipline

This model:
- does not prescribe architectures or protocols
- does not define billing or settlement rules
- does not introduce commercial or legal interpretations

The model exists to provide a **shared semantic structure**
for interoperable usage attribution.

Changes to the model require **explicit versioning**.
