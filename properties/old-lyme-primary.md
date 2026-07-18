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

- ✅ **Heating system + fuel — Oil-fired forced air.**
- ✅ **Cooling — Central AC.**

## Domestic hot water

- ✅ **Domestic hot water — Oil-associated system; exact tank/coil configuration is not recorded.**

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
2. **Oil-fired forced-air → heat-pump conversion.** The home is fossil-heated, so electrifying onto the existing solar + battery is a live ROI question; a Feb 2026 forwarded thread on heat pumps signals prior interest. Scope the conversion economics against winter oil use, electrical capacity, and Rate 7.
3. **EV load-shifting.** Already modeled in `enphase-usage`; ensure the Level 2 charger schedule tracks whichever rate
   plan is chosen, so charging lands in the off-peak / solar window.

## Cross-module links

- [`../energy`](../energy) — Energy Observer (Enphase production / consumption telemetry)
- `../../../enphase-usage` (sibling repo) — rate-plan modeling, battery policy, EV shift analysis
- [`../finance`](../finance) — Finance Auditor (utility spend verification)
