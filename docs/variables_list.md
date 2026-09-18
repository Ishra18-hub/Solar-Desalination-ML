# Variables List — Solar Desalination ML Project

**Project:** Predicting Freshwater Yield in Solar Desalination Systems
**Author:** Ishra Ismat Kamal
**Last Updated:** 18 September 2026

---

## Overview

This document lists all variables used in the ML project, extracted from the
CFD simulation data of my Final Year Design Project (FYDP).

- **Total Features:** 8 input variables
- **Target Variable:** 1 output variable (Freshwater_Yield_relative)
- **Data Source:** ANSYS Fluent CFD simulations (FYDP, IUB 2026)
- **Dataset Size:** 5 rows (small — for methodology demonstration)

---

## Input Features (Independent Variables)

### 1. Temperature_K

| Property | Value |
|----------|-------|
| **Column Name** | `Temperature_K` |
| **Unit** | Kelvin (K) |
| **Range** | 320 – 365 K |
| **Description** | Temperature of saline water entering the evaporation chamber |
| **Source** | FYDP Table 5.21 |

---

### 2. Air_Flow_ms

| Property | Value |
|----------|-------|
| **Column Name** | `Air_Flow_ms` |
| **Unit** | meters per second (m/s) |
| **Range** | 5 – 15 m/s |
| **Description** | Velocity of air from the fan |
| **Source** | FYDP Table 5.22 |

---

### 3. Solar_Irradiance_Wm2

| Property | Value |
|----------|-------|
| **Column Name** | `Solar_Irradiance_Wm2` |
| **Unit** | Watts per square meter (W/m²) |
| **Range** | 400 – 1200 W/m² |
| **Description** | Solar radiation incident on the parabolic collector |
| **Source** | FYDP Table 5.24 |

---

### 4. Ambient_Temperature_K

| Property | Value |
|----------|-------|
| **Column Name** | `Ambient_Temperature_K` |
| **Unit** | Kelvin (K) |
| **Range** | 285 – 305 K |
| **Description** | Surrounding air temperature |
| **Source** | FYDP Table 5.25 |

---

### 5. Droplet_Size_um

| Property | Value |
|----------|-------|
| **Column Name** | `Droplet_Size_um` |
| **Unit** | micrometers (μm) |
| **Range** | 50 – 500 μm |
| **Description** | Size of water droplets from the spray nozzle |
| **Source** | FYDP Table 5.23 |

---

### 6. Evaporation_Rate_relative

| Property | Value |
|----------|-------|
| **Column Name** | `Evaporation_Rate_relative` |
| **Unit** | Relative (normalized) |
| **Range** | 0.45 – 1.28 |
| **Description** | Relative evaporation rate (1.0 = baseline) |
| **Source** | FYDP Table 5.21 |
| **Note** | This is an intermediate output, not the final target |

---

### 7. Condensation_Efficiency

| Property | Value |
|----------|-------|
| **Column Name** | `Condensation_Efficiency` |
| **Unit** | Fraction (0–1) |
| **Range** | 0.83 – 0.92 |
| **Description** | Fraction of vapor that condenses to freshwater |
| **Source** | FYDP Table 5.25 |

---

### 8. Heat_Loss

| Property | Value |
|----------|-------|
| **Column Name** | `Heat_Loss` |
| **Unit** | Fraction (0–1) |
| **Range** | 0.18 – 0.27 |
| **Description** | Fraction of heat lost to environment |
| **Source** | FYDP Table 5.25 |

---

## Target Variable (Dependent Variable)

### Freshwater_Yield_relative

| Property | Value |
|----------|-------|
| **Column Name** | `Freshwater_Yield_relative` |
| **Unit** | Relative (normalized) |
| **Range** | 0.40 – 1.20 |
| **Description** | Relative freshwater production (1.0 = baseline) |
| **Source** | FYDP Table 5.21 |

---

## Summary Table

| # | Column Name | Unit | Type | Range |
|---|-------------|------|------|-------|
| 1 | `Temperature_K` | K | Feature | 320 – 365 |
| 2 | `Air_Flow_ms` | m/s | Feature | 5 – 15 |
| 3 | `Solar_Irradiance_Wm2` | W/m² | Feature | 400 – 1200 |
| 4 | `Ambient_Temperature_K` | K | Feature | 285 – 305 |
| 5 | `Droplet_Size_um` | μm | Feature | 50 – 500 |
| 6 | `Evaporation_Rate_relative` | relative | Feature | 0.45 – 1.28 |
| 7 | `Condensation_Efficiency` | fraction | Feature | 0.83 – 0.92 |
| 8 | `Heat_Loss` | fraction | Feature | 0.18 – 0.27 |
| 9 | `Freshwater_Yield_relative` | relative | **Target** | 0.40 – 1.20 |

---

## Important Notes

### 1. Small Dataset
My dataset has only **5 rows**. This is very small for ML.
- But Good for demonstrating methodology
- Not suitable for accurate prediction
- Future work: collect more data (real experiments)

### 2. Some Columns Are Outputs, Not Inputs
- `Evaporation_Rate_relative` — intermediate output
- `Condensation_Efficiency` — output
- `Heat_Loss` — output
- For ML, you may want to use only the **true inputs** (columns 1–5)

### 3. Recommended Features for ML

| Use for ML | Column |
|------------|--------|
| ✅ Input | `Temperature_K` |
| ✅ Input | `Air_Flow_ms` |
| ✅ Input | `Solar_Irradiance_Wm2` |
| ✅ Input | `Ambient_Temperature_K` |
| ✅ Input | `Droplet_Size_um` |
| ⚠️ Maybe | `Evaporation_Rate_relative` |
| ❌ Output | `Condensation_Efficiency` |
| ❌ Output | `Heat_Loss` |
| **Target** | `Freshwater_Yield_relative` |

---

## Feature Engineering (Planned)

| New Feature | Formula | Purpose |
|-------------|---------|---------|
| Temperature Difference | `Temperature_K − Ambient_Temperature_K` | Driving force for evaporation |
| Solar-to-Temp Ratio | `Solar_Irradiance_Wm2 / Temperature_K` | Efficiency indicator |
| Air-Temp Interaction | `Air_Flow_ms × Temperature_K` | Combined effect |

---

## References

- FYDP Report: *"Design and Simulation of Solar Powered Water Desalination Using Evaporation Technique"*, IUB, 2026
- Tables 5.21, 5.22, 5.23, 5.24, 5.25
- Supervisor: Dr. Khosru Mohammad Salim

---

*End of Variables List*
