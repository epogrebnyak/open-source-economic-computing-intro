Introduction to open source numerical analysis software: overview of R, python/pandas and Julia
===============================================================================================

### Introduction to R, python/pandas and Julia
  - scope of application - what are these programming languages for?
  - history of developement
  - relation to other programing languages
  - charts: speed comparison, packages, versions, popularity, github/stackoverflow references

### 'Dive in' general excercises
- setup/installation of packages/access to online environments
- excercises with language cross-reference: 
  - basic operations 
  - econometircs-ralted building blocks
  - data access

### Econometric excecises 
- ordinary least squares (OLS)
- maximum likelihood (ML)
 
More:
- simulation
- time series analysis topics: ...
 
### Extras
- other enabling tools: github, SO, md/pandoc
- mention and some excercises: Matlab/Octave, gretl


Language versions:
------------------

- R: https://www.r-project.org/

- Python: https://www.python.org/ + http://www.scipy.org/. 
  Suggested build: Scientific Anaconda Python https://www.continuum.io/downloads.

- Julia: http://julialang.org/

Notes: 
- all are interpreted languages
- may have different IDEs for ease of use
- can still use even Notepad.exe to edit code 
- have package installers
- IPython

View on evolution of applications of programming languages

```
Various programming tasks:
Entrprise software building:    FORTRAN(?), Java, ... -> Python
Learn programming:                   BASIC, Pascal, C -> Python  
Learn/apply OOP:                 C++, Java, smalltalk -> Python  
Desktop automation (incl MS Office):              VBA -> Python (sometimes e.g. ExcelWings)
Desktop scripting                                     -> Python

Rather econometric tasks:
Scientific/engineering computing:              MATLAB -> R, Python (with SciPy/NumPy), 
Econometrics:                           EViews, gretl -> R, Python (with Pandas and statmodels), Julia
High performance statistic computing:             C++ -> Julia
```

Suggested topics:
-----------------

```
1. What is this software for?

   Types of end-user tasks solved using this software.   

2. Getting started: Installation 

   What needs to de done before you can get (a) 1+1=2, (b) print("Hello, world!")

3. Basic operations in R, Python and Julia

   Data structures
   Mathematic operations 
   Flow control operators
   Functions
   Modules
   
4. Data import and plotting

   4.1. Data import  

   4.2. Plotting

5. Econometric examples

   We do basic case of econometric estimation both as own simple code and 
   also by calling a specialized library. Own code is for understanding the 
   procedure.

   - Ordinary least squares 

   - Maximum likelihood

6. Conclusion: which is software is best?

   Depends of type of task you are solving 
   Expression/readability of code 
   Skillset and background
   Job market popularity 

   Modern teaching in econometrics = intuition + math formulas + code

```

Links
-----

quant-econ.net

comparison of software: http://economics.sas.upenn.edu/~jesusfv/comparison_languages.pdf

comparison of syntax

Questions
---------

1. Maybe add gretl? Octave? Probably as an appendix, not to be endorsed for learning 
   instead of R/python. Can provide code for excercises, though. 
