# Variables List — Solar Desalination ML Project

**Project:** Predicting Freshwater Yield in Solar Desalination Systems
**Author:** Ishra Ismat Kamal
**Last Updated:** 17 September 2026

---

## Overview

This document lists all variables used in the ML project, extracted from the
CFD simulation data of my Final Year Design Project (FYDP).

- **Total Features:** 5 input variables
- **Target Variable:** 1 output variable
- **Data Source:** ANSYS Fluent CFD simulations (FYDP)

---

## Input Features (Independent Variables)

### 1. Inlet Water Temperature (T_in)

| Property | Value |
|----------|-------|
| **Symbol** | T_in |
| **Unit** | Kelvin (K) |
| **Range** | 320 – 365 K |
| **Description** | Temperature of saline water entering the evaporation chamber after solar heating |
| **Source** | FYDP Table 5.15, 5.21 |
| **Physical Meaning** | Higher temperature → more evaporation → more freshwater yield |
| **Importance** | ⭐⭐⭐⭐⭐ (Highest expected impact) |

---

### 2. Air Flow Rate (v_air)

| Property | Value |
|----------|-------|
| **Symbol** | v_air |
| **Unit** | meters per second (m/s) |
| **Range** | 5 – 15 m/s |
| **Description** | Velocity of air from the fan that carries vapor to the condensation section |
| **Source** | FYDP Table 5.16, 5.22 |
| **Physical Meaning** | Optimal around 10 m/s; too low = poor vapor transport, too high = droplet entrainment |
| **Importance** | ⭐⭐⭐⭐ |

---

### 3. Droplet Diameter (d_drop)

| Property | Value |
|----------|-------|
| **Symbol** | d_drop |
| **Unit** | micrometers (μm) |
| **Range** | 50 – 500 μm |
| **Description** | Size of water droplets produced by the spray nozzle |
| **Source** | FYDP Table 5.17, 5.23 |
| **Physical Meaning** | Smaller droplets → more surface area → faster evaporation |
| **Importance** | ⭐⭐⭐⭐ |

---

### 4. Solar Irradiance (G)

| Property | Value |
|----------|-------|
| **Symbol** | G |
| **Unit** | Watts per square meter (W/m²) |
| **Range** | 400 – 1200 W/m² |
| **Description** | Intensity of solar radiation incident on the parabolic collector |
| **Source** | FYDP Table 5.18, 5.24 |
| **Physical Meaning** | Directly affects achievable water temperature |
| **Importance** | ⭐⭐⭐⭐⭐ |

---

### 5. Ambient Temperature (T_amb)

| Property | Value |
|----------|-------|
| **Symbol** | T_amb |
| **Unit** | Kelvin (K) |
| **Range** | 285 – 305 K |
| **Description** | Surrounding air temperature affecting heat loss and condensation |
| **Source** | FYDP Table 5.19, 5.25 |
| **Physical Meaning** | Lower ambient temp → better condensation → more yield |
| **Importance** | ⭐⭐⭐ |

---

## Target Variable (Dependent Variable)

### Freshwater Yield (Y_f)

| Property | Value |
|----------|-------|
| **Symbol** | Y_f |
| **Unit** | Relative (normalized) |
| **Range** | 0.40 – 1.20 |
| **Description** | Normalized freshwater production per unit time |
| **Baseline** | 1.00 = yield at (354 K, 10 m/s, 200 μm, 1000 W/m², 300 K) |
| **Source** | FYDP Table 5.21 |
| **Interpretation** | 1.20 = 20% more yield than baseline; 0.40 = 60% less than baseline |

---

## Summary Table

| # | Variable | Symbol | Unit | Type | Range |
|---|----------|--------|------|------|-------|
| 1 | Inlet Water Temperature | T_in | K | Feature | 320 – 365 |
| 2 | Air Flow Rate | v_air | m/s | Feature | 5 – 15 |
| 3 | Droplet Diameter | d_drop | μm | Feature | 50 – 500 |
| 4 | Solar Irradiance | G | W/m² | Feature | 400 – 1200 |
| 5 | Ambient Temperature | T_amb | K | Feature | 285 – 305 |
| 6 | Freshwater Yield | Y_f | relative | **Target** | 0.40 – 1.20 |

---

## Feature Engineering (Planned)

Additional features that may be created during ML:

| New Feature | Formula | Purpose |
|-------------|---------|---------|
| Temperature Difference | T_in − T_amb | Driving force for evaporation |
| Solar-to-Thermal Ratio | G / T_in | Efficiency indicator |
| Droplet Surface Area | 4π(d_drop/2)² | Evaporation surface proxy |
| Air-Temp Interaction | v_air × T_in | Combined effect on evaporation |

---

## Notes

1. **All data is from CFD simulations**, not physical experiments.
2. **Freshwater yield is normalized** — actual volume (L/day) requires scaling.
3. **No missing values** in the dataset.
4. **Small dataset** (~25–30 rows) — appropriate for demonstrating methodology,
   not for industrial-grade prediction.

---

## References

- FYDP Report: *"Solar Powered Water Desalination Using Evaporation Technique"*,
  Independent University, Bangladesh, 2026.
- Tables 5.15 – 5.25 (Parametric Investigation Results)
- Supervisor: Dr. Khosru Mohammad Salim, Dept. of EEE, IUB

---

*End of Variables List*
