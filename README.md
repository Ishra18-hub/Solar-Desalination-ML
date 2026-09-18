# Solar-Desalination-ML

**Predicting freshwater yield in solar-powered desalination systems using Machine Learning**

This project is an extension of my Final Year Design Project (FYDP) titled
*"Design and Simulation of Solar Powered Water Desalination Using Evaporation Technique."*

---

## About My Final Year Design Project (FYDP)

My FYDP focused on designing a solar-powered desalination system that uses:
- A **parabolic solar collector** to heat saline water
- **Spray-assisted evaporation** through a nozzle to increase surface area
- **Fan-driven condensation** to collect freshwater

The system was analyzed using **ANSYS Fluent CFD simulations** and achieved a
simulated **32.35% thermal efficiency**, outperforming conventional solar stills
(typically 20–30%).

This ML project uses the **CFD simulation data** from the FYDP to predict
freshwater yield based on operating parameters.

---

## Dataset

### Source
The dataset was extracted from the **CFD simulation results** of my FYDP,
conducted in **ANSYS Fluent 2024 R1**.

> ⚠️ **Important Note:** This is **simulation data**, not experimental data.
> No physical prototype was built during the FYDP. The simulation was validated
> against thermodynamic principles and literature, but real-world performance
> may differ.

### Features (Input Variables)

| Feature | Unit | Range | Description |
|---------|------|-------|-------------|
| Inlet Water Temperature | K | 320–365 | Temperature of saline water entering the evaporation chamber |
| Air Flow Rate | m/s | 5–15 | Velocity of air from the fan |
| Droplet Diameter | μm | 50–500 | Size of sprayed water droplets |
| Solar Irradiance | W/m² | 400–1200 | Incident solar radiation on the collector |
| Ambient Temperature | K | 285–305 | Surrounding air temperature |

### Target Variable (Output)

| Target | Unit | Description |
|--------|------|-------------|
| Freshwater Yield | relative | Normalized freshwater production |

### Data File
The cleaned dataset is available at: `data/desalination_data.csv`

---

## 🗂️ Project Structure

Solar-Desalination-ML/
├── data/
│   └── desalination_data.csv
├── docs/
│   ├── variables_list.md
│   └── learning_log.md
├── notebooks/
│   ├── 01_python_basics_practice.ipynb
│   ├── 02_python_functions_practice.ipynb
│   ├── 03_boolean_conditionals_practice.ipynb
│   ├── 04_python_basics_practice.ipynb
│   ├── 05_fydp_data_creating.ipynb
│   └── 06_numpy_basics.ipynb
├── README.md
└── requirements.txt


---

## 🛠️ Tools & Technologies

| Category | Tools |
|----------|-------|
| Programming Language | Python 3 |
| Environment | Google Colab |
| Data Manipulation | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning (upcoming) | Scikit-learn, XGBoost |
| Version Control | Git, GitHub |

---

## Progress

### September 2026 — Python & NumPy Foundations
- [x] Python basics (variables, data types, loops, conditionals)
- [x] Functions (def, return, docstring, default arguments)
- [x] Boolean logic, comparison operators
- [x] Lists, tuples, and their methods
- [x] Extracted FYDP simulation data → `desalination_data.csv`
- [x] Pandas basics (`.head()`, `.info()`, `.describe()`)
- [x] NumPy basics (arrays, indexing, slicing, math)
- [x] NumPy advanced (broadcasting, random, linear algebra)
- [x] Pandas basics: CSV file upload, basic info, missing values, correlation, column names
- [x] Pandas groupby & EDA

### Upcoming Machine Learning till 6th OCTOBER 2026 (Planned)
- [x] Exploratory Data Analysis (EDA)
- [ ] Linear Regression
- [ ] Random Forest Regressor
- [ ] XGBoost Regressor
- [ ] Model evaluation (R², RMSE, MAE)
- [ ] Feature importance analysis

### November 2026 — Project 2 (Planned)
- Solar PV Power Forecasting using real-world weather data

---

## Limitations

1. **Simulation-based data**: No physical prototype was built.
2. **Small dataset size**: ~25–30 data points from CFD parameter sweeps.
3. **Steady-state assumption**: Real systems are transient.
4. **No uncertainty quantification**: Simulation errors not propagated.

---

## Future Work

- **October 2026**: Train and evaluate ML models
- **November 2026**: Start Project 2 — Solar PV Power Forecasting with real weather data
- **Future**: Validate model with experimental prototype data
- **Long-term**: Publish a short technical paper

---

## References

- FYDP Report: *"Design and Simulation of Solar Powered Water Desalination Using Evaporation Technique"*, Independent University, Bangladesh, 2026.
- Supervisor: Dr. Khosru Mohammad Salim, Department of EEE, IUB.

---

## Author

**Ishra Ismat Kamal**
- Final-year EEE student, Independent University, Bangladesh (IUB)
- Email: ismatkamlalishra@gmail.com
- GitHub: [@Ishra18-hub](https://github.com/Ishra18-hub)
- Open to Master's opportunities in Renewable Energy, Data Science, and Computational Engineering

---

## License

This project is for academic and educational purposes.
