# Properties — State Index

The Guardian's rollup of physical-asset and environmental state across all properties.
Each property has a record under `properties/`. This file is the durable index and the
**Open Money Considerations** rollup — the items that cost money if they sit forgotten.

## Properties

| Property | Role | Heating | Cooling | EV charging | Solar / battery | Record |
|---|---|---|---|---|---|---|
| Old Lyme | Primary residence | ✅ Oil-fired forced air | ✅ Central AC | ✅ Level 2 (grid / battery) | 🔍 Enphase + IQ Battery | [old-lyme-primary.md](properties/old-lyme-primary.md) |

## Open money considerations (rollup)

- **[Old Lyme] Eversource Rate 7 (TOU) vs Rate 1** — pick the wrong one and it leaks monthly. Analysis lives in the `enphase-usage` repo docs.
- **[Old Lyme] Oil-fired forced-air → heat-pump conversion** — active ROI question given the on-site solar + battery; scope against winter oil use, electrical capacity, and Rate 7.
- *(extend as more properties or considerations are recorded)*

## Cross-module

- [`../energy`](../energy) — Energy Observer (usage telemetry)
- [`../finance`](../finance) — Finance Auditor (spend verification)

---
*Confidence key: ✅ confirmed by Braydon · 🔍 verifiable from a source · ❓ unconfirmed*
