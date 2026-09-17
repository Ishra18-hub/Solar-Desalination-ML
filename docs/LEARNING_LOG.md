# Learning Log — Solar Desalination ML

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

## 10–11 September 2026
- Learned Python functions: `def`, `return`, docstring, `None`, default arguments
- Learned higher-order functions and key arguments
- Created variable list for the project (`docs/variables_list.md`)

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

---

## Next Steps
- [ ] NumPy Advanced (broadcasting, axis operations)
- [ ] Pandas deep dive (groupby, merge, filtering)
- [ ] Matplotlib/Seaborn for visualization
- [ ] Scikit-learn: Linear Regression
- [ ] Scikit-learn: Random Forest
- [ ] XGBoost
