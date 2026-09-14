# Solar Desalination - Variable List

## Input Variables (Features / X)

| Variable | Unit | Description | Source | Availability |
|----------|------|-------------|--------|--------------|
| Temperature | K | Inlet water temperature after solar heating | Table 5.21 | Available (5 values) |
| Air Flow Rate | m/s | Air velocity in evaporation chamber | Table 5.22 | Available (5 values) |
| Solar Irradiance | W/m² | Solar radiation intensity | Table 5.24 | Available (5 values) |
| Ambient Temperature | K | Outside air temperature | Table 5.25 | Available (5 values) |
| Droplet Size | μm | Spray nozzle droplet diameter | Table 5.23 | Available (5 values) |

## Output Variables (Target / y)

| Variable | Unit | Description | Source | Priority |
|----------|------|-------------|--------|----------|
| Freshwater Yield | relative | Relative freshwater production | Table 5.21 | Primary Target |
| Evaporation Rate | relative | Relative evaporation rate | Table 5.21 | Secondary Target |
| Thermal Efficiency | % | System efficiency | Table 5.12 | Secondary Target |

## Performance Variables (For Analysis)

| Variable | Unit | Description | Source |
|----------|------|-------------|--------|
| Condensation Efficiency | % | Vapor condensation rate | Table 5.22 |
| Heat Loss | % | Heat lost to environment | Table 5.25 |
| Recovery Ratio | % | Freshwater / Feedwater ratio | Table 5.11 |
| Brine Concentration | g/L | Salt concentration in brine | Table 5.14 |

## Variables NOT Available (Excluded)

| Variable | Reason |
|----------|--------|
| Operating Time | No actual data in FYDP report |
| Droplet Surface Area Ratio | Only calculated, not measured |
| Economic Parameters | Not relevant for ML prediction |

## ML Model Plan

### Target Variable (y)
- **Primary:** Freshwater Yield (relative)
- **Reason:** Directly measured, continuous, most important for system performance

### Feature Variables (X)
1. Temperature (K)
2. Air Flow Rate (m/s)
3. Solar Irradiance (W/m²)
4. Ambient Temperature (K)
5. Droplet Size (μm)

### Data Summary
- **Total observations:** 5 per variable
- **Total features:** 5
- **Target:** 1
- **Dataset size:** 5 rows × 6 columns (small but usable for baseline models)

## Notes
- Only variables with actual data will be used for ML models.
- Primary target for prediction: **Freshwater Yield (relative)**
- Small dataset (5 rows) — suitable for Linear Regression and Decision Tree (not deep learning)
- Will expand dataset in future with more experimental data

## Version History
| Version | Date | Changes |
|---------|------|---------|
| 1.0 | 11 Sep 2026 | Initial variable list |
| 1.1 | 14 Sep 2026 | Added Availability column, excluded unavailable variables, added ML plan |
