# Solar-Desalination-ML
Project 1: "ML project for predicting freshwater yield in solar desalination systems using Final Year Design Project data"

## About My FINAL YEAR DESIGN PROJECT
This project is an extension of my Final Year Design Project (FYDP) titled 
"Solar Powered Water Desalination Using Evaporation Technique."
This project focused on designing a solar-powered desalination system that uses 
a parabolic solar collector, spray-assisted evaporation, and fan-driven 
condensation to produce freshwater from saline water. The system achieved 
32.35% thermal efficiency.
This ML project uses the experimental data from the FYDP to predict 
freshwater yield using operating parameters (temperature, air flow, 
solar irradiance, etc.).

# September Progress
- [x] python basics
- [x] Functions (def, return, docstring, default args)
- [x] Higher-order functions & key arguments
- [x] Booleans and Conditionals
- [x] Lists & tuple
- [x] For and while loops, and list comprehensions
- [x] CSV file with FYDP datasets


# Daily Progress log

## 9 September 2026
- Set up project folder and GitHub repository
- Learned Python basics: variables, data types, loops, lists, dictionaries

## 10-11 September 2026
- Learned Python functions: def, return, docstring, None, default arguments
- Learned higher-order functions and key arguments
- Created variable list for the project (docs/variables_list.md)
  
## 12 September 2026
- Booleans has two possible values TRUE & FALSE
- Learned Comparison Operations ==, <, >, <=, >=, !=
- how to combine boolean values

| operator | rule |
|--------|------|
| AND | True + True = True |
| OR | True + False = True |
| NOT | not True = False |

- how to use Conditional Statements if-elif-else
- boolean conversion
- X-OR (Exclusive OR) if one condition is right then true otherwise false
- De Morgan's Law	not (A and B) = (not A) or (not B)
- Weather Bug	(the importance of brackets)

## 13 September 2026
- Learned about lists, must use second brackets
  
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

- Learned about Indexing how it used for a specific list element, zero-based indexing 
- how to do slicing
- Learned about a list can be changed and modified (changing lists) 
- List functions. ex: len gives the length of a list, sorted returns a sorted version of a list, sum does what you might expect, min & max to get the minimum or maximum of several arguments.
- "Interlude: objects" everything in python (Type, variable, method) are object and with '.' attribute/method can be access. Exm: "solar".upper()` → `"SOLAR", .imag & .real attributes for complex number, int attribute: `.numerator`, `.denominator`
- Learned Tuples: Immutable (unchangeable) list, uses first bracket `(1, 2, 3)`, fast and secured than List, Unpacking: `a, b, c = (1, 2, 3)`, works as Dictionary key

## 14 September 2026

## 15 September 2026
- I created the csv file for my first project
- The file contains My FYDP datasets
- I took help from Google, different sites and AI to understand making pandas data frame and how to make a csv file. Finally understand that PANDAS = PYTHON'S EXCEL
- while justifying the csv file learned about two functions how these works df.head() and df.describe()

| Sl | work |
|--------|------|
| 1 | extracted the datas from FYDP datasets |
| 2 | understood the data structure |
| 3 | learned the pandas dataframe |
| 4 | understood the process and made the desalination csv file |
| 5 | learned how to justify the csv file |
| 6 | learned how to download the csv file from colab |

## 16 September 2026

| Resource | Link |
|--------|------|
| W3Schools NumPy | w3schools.com/python/numpy |
| Kaggle Python Course | https://www.kaggle.com/learn/python |
| NumPy Official Docs | numpy.org/doc/stable/user/absolute_beginners.html |
| YouTube | "NumPy Tutorial for Beginners" |

- NumPy Introduction: what is NumPy, NumPy Install, Creating Array's, Verifying dimensions
- Array Operations: NumPy Array Indexing, NumPy Array Slicing
- Array Attributes
  
# Future Work
- October: Machine Learning Models (Linear Regression, Random Forest, XGBoost)
- November: Project 2 (PV Forecasting)

# Author
Ishra Ismat Kamal
