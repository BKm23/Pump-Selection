# Curve Digitization Confidence — Verify Against Goulds PSS

Performance curves are **modelled**, not pixel-digitized. Verify any short-listed
pump's duty, NPSHr, efficiency and BHP in the **Goulds Pump Selection System (PSS)**
before issuing an RFQ.

- Total records: **103**
- `coverage_chart` (per-size, read from GPM9 composite coverage charts): **56**
- `digitized_low` (flagship families, modelled + anchored): **3**
- `envelope_only` (family-level, lowest confidence): **44**

## Stock pumps — now per-size (`coverage_chart`)

Size lists and flow/head windows are read from the published coverage charts, so the
tool selects the correct **model + size** for a duty. The detailed per-size efficiency,
NPSHr and impeller-trim curves are still modelled — confirm those in PSS.

| Model | Sizes | Consistency | Section |
|---|---|---|---|
| 3175 | 17 (3x6-12, 4x6-12, 6x8-12, 8x8-12…) | Up to 6% (low to heavy stock) | PP-1A |
| 3180 / 3185 | 17 (3x6-12, 3x6-14, 4x6-14, 4x6-16…) | Up to 6-7% (heavy stock / process) | PP-1B |
| 3181 / 3186 | 16 (3x6-14, 4x6-14, 4x6-16, 4x6-19…) | Up to 6-7% (HT/HP stock) | PP-1C |
| 3500XD | 6 (6x6-16, 4x6-24, 6x14-22, 4x8-24…) | 8-16% MC (medium consistency) | PP-1D |

## What to confirm in PSS for any selection
1. Actual head-capacity curve and shutoff at the selected size/speed/trim.
2. NPSHr at duty flow (modelled here — do not rely on it).
3. Efficiency & BHP at duty (affects motor sizing).
4. Min continuous stable flow and allowable operating region.
5. Material/seal availability for the actual fluid and temperature.
