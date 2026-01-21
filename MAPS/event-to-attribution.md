# Mapping — Event to Attribution (Usage Attribution)

This mapping documents how machine-generated activity
progresses from **events** to **attribution**
within the Usage Attribution reference.

The mapping is **descriptive**, not prescriptive.

---

## End-to-End Mapping

| Layer       | Input                    | Processing Focus                               | Output                     | Notes |
|-------------|--------------------------|------------------------------------------------|----------------------------|-------|
| Event       | Raw machine action       | Identification, timestamping, context capture | Qualified event record     | Events are observable, not attributable |
| Usage       | Qualified event records  | Aggregation, normalization, filtering          | Measured usage             | Measurement without responsibility |
| Attribution | Measured usage           | Entity resolution, delegation handling         | Attributed usage           | Accountability established |

---

## Layer Relationships

- **Event → Usage**  
  Events must be normalized and quantified before responsibility can be considered.

- **Usage → Attribution**  
  Attribution without quantified usage is ambiguous and non-reproducible.

---

## Boundary Conditions

The following are **explicitly out of scope** of this mapping:

- Billing or settlement qualification
- Pricing, tariffs, or valuation logic
- Payment execution or invoicing
- Legal or contractual responsibility determination
- Identity provisioning or authentication mechanisms

---

## Consistency Rule

Any change to:
- layer definitions,
- their order,
- or their semantic meaning

requires a corresponding update to:
- `MODEL.md`
- `SCOPE.md`
- and the `CHANGELOG.md`.

This mapping exists to ensure **interpretability and auditability**
across independent systems.
