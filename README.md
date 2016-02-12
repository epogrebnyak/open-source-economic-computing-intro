Introduction to open source numerical analysis software: overview of R, python/pandas and Julia
===============================================================================================

### 1. Introduction to R, python/pandas and Julia
  - scope of application - what are these programming languages for?
  - history of developement
    - personalities
    - workflow for language development
    - more in 'ecosystem': journals, events
    - relation to other programming languages
  - charts
    - speed comparison
    - number of packages
    - version maturity
    - job search popularity
    - github
    - stackoverflow references
      - as of Feb 12, 2016, thousands: python 532.2, r 124.3, julia 1.5 (also matlab 57.0)
    - other stats
      - lines of code per sample task
      - size of language core
      - distribution package Mb 

### 2. General programming exercises
- setup/installation of packages and access to online environments
  - language versions and their compatibility 
  - installation on Windows
  - command line and IDEs
  - packages management (install.packages, pip)
- excercises (with language cross-reference, as [here](http://hyperpolyglot.org/numerical-analysis))
  - basic operations
  - econometrics-ralted building blocks
  - data access

### 3. Econometric excecises 
- ordinary least squares (OLS)
- maximum likelihood (ML)
  - in r and python: <https://github.com/epogrebnyak/mle-for-nowcasting>
 
More:
- simulation
- time series analysis topics: ...
 
### Extras
- other enabling tools
  - github
  - stackoverflow (SO)
  - markdown/pandoc
- mention and some excercises
  - Matlab/Octave
  - gretl


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
