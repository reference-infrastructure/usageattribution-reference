# Scope — Usage Attribution Reference

This document defines the **scope boundaries** of the
**Usage Attribution Reference**.

Usage attribution describes the **deterministic linkage**
between measurable system activity and an **accountable entity**.
It operates independently of pricing, billing, or payment execution.

---

## Included

This reference covers **usage attribution semantics** for
machine-to-machine and system-to-system interactions, including:

- Definition of usage units derived from machine-generated events
- Attribution of usage to identifiable machine, agent, or organizational entities
- Handling of delegation, orchestration, and proxy execution scenarios
- Resolution of one-to-one, one-to-many, and indirect attribution
- Separation of attribution logic from billing and settlement
- Versioned semantics enabling consistent interpretation over time

---

## Excluded

This reference explicitly does **not** cover:

- Billing qualification or settlement determination
- Pricing models, tariffs, or commercial valuation
- Payment processing, clearing, or invoicing
- Identity provisioning, authentication, or access control systems
- Legal, regulatory, or contractual responsibility frameworks
- Product implementations, services, or vendor-specific logic

---

## Terminology Baseline

- **Usage:**  
  Measurable activity resulting from machine-generated actions or interactions.

- **Attribution:**  
  The logical assignment of usage to an accountable entity based on defined rules.

- **Accountable Entity:**  
  A machine, agent, organization, or system identity recognized for responsibility assignment.

---

## Scope Discipline

This repository exists to provide **semantic clarity**
for attribution prior to billing or settlement.

It does **not**:
- prescribe architectures,
- endorse standards or protocols,
- certify systems,
- or define commercial practices.

All scope changes must be documented through **explicit versioning**
and reflected consistently across repository files.
