# Learning Log — Solar Desalination ML

**Author:** Ishra Ismat Kamal
**Started:** 9 September 2026
**Environment:** Google Colab
**Goal:** Build a strong ML portfolio for Master's applications

Daily progress notes for my Python + ML learning journey.

---
# September Progress
- [x] python basics
- [x] Functions (def, return, docstring, default args)
- [x] Higher-order functions & key arguments
- [x] Booleans and Conditionals
- [x] Lists & tuple
- [x] For and while loops, and list comprehensions
- [x] CSV file with FYDP datasets
- [x] NumPy Basics
- [ ] NumPy Advanced

## 9 September 2026
- Set up project folder and GitHub repository
- Learned Python basics: variables, data types, loops, lists, dictionaries
- Created notebook: `01_python_basics_practice.ipynb`

## 10–11 September 2026
- Learned Python functions: `def`, `return`, docstring, `None`, default arguments
- Learned higher-order functions and key arguments
- Created variable list for the project (`docs/variables_list.md`)
- Created notebook: `02_python_functions_practice.ipynb`

## 12 September 2026
- Learned Booleans: `True` / `False`
- Comparison operators: `==`, `<`, `>`, `<=`, `>=`, `!=`
- Logical operators: `AND`, `OR`, `NOT`, `XOR`

| operator | rule |
|--------|------|
| AND | True + True = True |
| OR | True + False = True |
| NOT | not True = False |

- Conditional statements: `if-elif-else`
- De Morgan's Law: `not (A and B) = (not A) or (not B)`
- Weather Bug	(the importance of brackets)
- Created notebook: `03_boolean_conditionals_practice.ipynb`

## 13 September 2026
- Learned about lists and their methods (`.append()`, `.pop()`, `.remove()`, `.insert()`, `.sort()`, `.reverse()`, `.index()`, `.count()`)

| Method | work |
|--------|------|
| `.append(x)` | adds in last |
| `.pop()` | removes the last one |
| `.remove(x)` | removes the specific value |
| `.insert(i, x)` | adds in specific place |
| `.sort()` | sorting |
| `.reverse()` | reversing |
| `.index(x)` | finds the place of value |
| `.count(x)` | how many times are in the list |

- Learned indexing and slicing
- Learned about tuples (immutable, unpacking, dictionary keys)
- Learned that everything in Python is an object
- Created notebook: `04_list_and_tuples.ipynb`

## 15 September 2026

| Sl | work |
|--------|------|
| 1 | extracted the datas from FYDP datasets |
| 2 | understood the data structure |
| 3 | learned the pandas dataframe |
| 4 | understood the process and made the desalination csv file |
| 5 | learned how to justify the csv file |
| 6 | learned how to download the csv file from colab |

- Created CSV file for Project 1 with FYDP datasets
- Learned Pandas DataFrame — "Pandas = Python's Excel"
- Learned `df.head()`, df.info and `df.describe()`
- Created notebook: `05_fydp_data_creating.ipynb`

## 16 September 2026

| Resource | Link |
|--------|------|
| W3Schools NumPy | w3schools.com/python/numpy |
| Kaggle Python Course | https://www.kaggle.com/learn/python |
| NumPy Official Docs | numpy.org/doc/stable/user/absolute_beginners.html |
| YouTube | "NumPy Tutorial for Beginners" |

- Learned NumPy basics: array creation, indexing, slicing
- Array attributes: `.shape`, `.ndim`, `.size`, `.dtype`
- Array math: element-wise operations, dot product, matrix operations
- Practiced dot product with FYDP efficiency calculation
- Created notebook: `06_numpy_basics.ipynb`

## 17 September 2026 
**Topic:** README Writing + Data Honesty
- Learned the difference between **simulation data** and **experimental data**
- Realized my FYDP data is from **CFD simulations**, not physical experiments
- Decided to separate `README.md` (project) from `learning_log.md` (personal journey)

**Important lesson:** Always be truthful about data sources.

## Next Steps
- [ ] NumPy Advanced (broadcasting, axis operations)
- [ ] Pandas deep dive (groupby, merge, filtering)
- [ ] Matplotlib/Seaborn for visualization
- [ ] Scikit-learn: Linear Regression
- [ ] Scikit-learn: Random Forest
- [ ] XGBoost

---

## Upcoming Plan

### October 2026 — Machine Learning
- [ ] Exploratory Data Analysis (EDA)
- [ ] Linear Regression
- [ ] Random Forest Regressor
- [ ] XGBoost Regressor
- [ ] Model evaluation (R², RMSE, MAE)
- [ ] Feature importance analysis

### November 2026 — Project 2
- Solar PV Power Forecasting using real-world weather data

### December 2026
- Complete Project 2
- IELTS exam
- Update portfolio for Master's applications

---

## Master Resource List

| Resource | Link |
|----------|------|
| Kaggle Python Course | kaggle.com/learn/python |
| Hands-on Machine Learning with Scikit-learn, keras and Tensor flow (2nd edition) | A book by Aurélien Géron |
| W3Schools NumPy | w3schools.com/python/numpy |
| NumPy Docs | numpy.org/doc/stable |
| Pandas Docs | pandas.pydata.org/docs |
| Scikit-learn Docs | scikit-learn.org |

---

*Last updated: 17 September 2026*
