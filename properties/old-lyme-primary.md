# Old Lyme — Primary Residence

> The Guardian's asset-state record for the Old Lyme primary residence.
> This record captures what the home **has**. Usage telemetry lives in the `energy`
> module (and the sibling `enphase-usage` repo); money math lives in `finance`.

**Confidence key:** ✅ confirmed by Braydon · 🔍 verifiable from a source · ❓ unconfirmed — fill in

## Identity

| Field | Value |
|---|---|
| Role | Primary residence |
| Location | Old Lyme, CT 06371 |
| Occupants | Braydon, Alexandra, Adrian (+ family) |
| Ownership | Braydon / Alexandra — ❓ confirm title |
| Record first captured | 2026-07-18 |

## Climate & envelope

- ❓ **Heating system + fuel — CONFIRM** (oil / propane / electric resistance / heat pump / natural gas).
  - *Searched and not found:* paia-memory, `house/property` files, `enphase-usage` docs, and the email archive.
  - *One lead, not confirmed here:* a 2019 "Propane contract" email (Intempio era, sent before the 2020 CT move) — likely a prior property, **not** established for this home.
  - *Implication if fossil:* an oil/propane → heat-pump conversion becomes a live money consideration (see below).
- ✅ **Cooling — Central AC.**

## Domestic hot water

- ❓ Confirm — likely follows heating fuel (indirect tankless coil / separate tank / electric).

## Electricity & generation

- 🔍 **Enphase solar + IQ Battery** installed on site.
- 🔍 Utility: **Eversource (Connecticut)**.
- ❓ Rate plan currently enrolled — **Rate 1 (flat) vs Rate 7 (TOU)** is the open decision (below).
- ❓ Electrical service — panel amps and headroom for further electrification (heat pump, second EV) — confirm.

## EV charging

- ✅ **Level 2, 240V** — draws from grid and the IQ Battery, possibly solar-tied.

## Other infrastructure

- ❓ Water source (well vs municipal), sewer vs septic, standby generator, insulation / build age — confirm.

## Open money considerations

> Items that cost money if they sit forgotten. This section is the durable memory.

1. **[TOP] Eversource Rate 7 (TOU) vs Rate 1.** Active analysis in the sibling `enphase-usage` repo
   (`docs/ev-charging-and-rate-7.md`, `docs/eversource-rate-7.md`). Choosing the wrong plan leaks money every month.
2. **Oil / propane → heat-pump conversion** — *conditional on confirming heating fuel.* If the home is fossil-heated,
   electrifying onto the existing solar + battery is a material ROI question; a Feb 2026 forwarded thread on heat pumps
   signals prior interest. Cannot be scoped until heating fuel is confirmed.
3. **EV load-shifting.** Already modeled in `enphase-usage`; ensure the Level 2 charger schedule tracks whichever rate
   plan is chosen, so charging lands in the off-peak / solar window.

## Cross-module links

- [`../energy`](../energy) — Energy Observer (Enphase production / consumption telemetry)
- `../../../enphase-usage` (sibling repo) — rate-plan modeling, battery policy, EV shift analysis
- [`../finance`](../finance) — Finance Auditor (utility spend verification)
