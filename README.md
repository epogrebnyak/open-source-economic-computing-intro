Introduction to numerical analysis in R, python/pandas and Julia
================================================================

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

### 2. Installation

Setup/installation of packages and access to online environments

  - language versions and their compatibility 
  - installation on Windows
  - command line, text editors and IDEs
    - command line examples
      - what runs a text file with program code 
      - what opens an interpreter
    - popular text editors (bare [Notepad+][npp], but also [a lot more][IDEs])
    - IDEs
      - standard (IDLE for python, R.exe, Juno for Julia)
      - third-party (Spyder for python in Anaconda)
      - note: given we aim 3 languages it would be nice to have an IDE to run them all 
  - packages management (install.packages, pip)
  - online environments
    - Julia stands out as having a stable and 'official' online IDE <https://www.juliabox.org>

[npp]:https://notepad-plus-plus.org
[IDEs]:https://spin.atomicobject.com/2014/03/13/light-table-github-atom-ide
  
### 3. General programming exercises
Excercises with language cross-reference (e.g. as in [here](http://hyperpolyglot.org/numerical-analysis))
  - basic operations
    - data structures
    - mathematic operations 
    - flow control operators
    - functions 
  - econometrics-related building blocks
    - dataframes
    - time series data types 
    - functions
  - data access
    - read csv
    - read from web
    - usually "Sorry, no Excel"
  - plotting
    - native plotting procedures
    - [matlibplot](http://matplotlib.org/)
    - [ggplot](http://ggplot2.org/)
    - [Gadfly](http://dcjones.github.io/Gadfly.jl/)
  - additional topics
    - debugging tools 
    - unit testing 

### 4. Econometric excecises 

This section is really why why introdice and dig into R, python and julia. It has three parts:
descriptive statistics, estimation methods, applications. 

For *descriptive statistics* the purpose is rather clear - is to be able to access data, do some manipulations/transforms/summaries over it and plot.  

In *estimation methods* I suggest looking and OLS and max likelihood (ML) and to do own 
simple code for it as well as introduce related packages. It should make it more clear what 
the packages are doing as compared to core algorithm (ususally more precision, border cases, statistics) 
and how to work better with them (not treating as pure 'black boxes'). 

- For max likelihood I already wrote some code in python and r which we can use <https://github.com/epogrebnyak/mle-for-nowcasting>. 
- Introducing OLS should not be too hard, but I think rewarding to follow, again in own code and in standard packages, like ```ls()``` in R. 

For both methods, as an excecise, I like the idea of generating the data by known data generating process and looking at how regression works or fails on this data. 

For **applications** part need your suggestion - it could be good to port at least some of your Eviews time series code to R/pandas and also provide an example where Julia code is much faster than in R/python to prove Julia useful (maybe some simulation excercise).

  - Descriptive statistics
    - Load data from web source or local file 
    - Look at sample sizes, mean/variance, correlations, missing data etc. 
    - Plot some data and summaries (e.g. distribution histogram for time series)
    
  - Estimation methods
    - ordinary least squares (OLS)
    - maximum likelihood (ML)
      - in r and python: <https://github.com/epogrebnyak/mle-for-nowcasting>
       
  - Applications
    - to be decided 
 
Comment - would be nice to have:
- some simulation excercises 
- some task where Julia would stand out (maybe simulation above)
- time series analysis topics
 
### Extras

- Other enabling programming tools
  - [github](https://guides.github.com/introduction/flow/) for code sharing 
  - [stackoverflow (SO)](http://stackoverflow.com/) for good advice on solving programming tasks
    - quality answered enforced- example: question [best language for econometrics][so1] closed as not constructive
  - [markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) for quick and clean text organisation 
  - [pandoc](http://pandoc.org/) to convert between text file formats (HTML, doc, rtf, pdf, etc)

  [so1]:http://stackoverflow.com/questions/3064178/best-programming-language-for-teaching-econometrics

- Not covered
  - Matlab/Octave
  - gretl
  - IPython
  
  May provide some demos or excercises for Matlab/Octave and gretl. 
  
Language versions:
------------------

- R: <https://www.r-project.org>
  -  Suggested build: [RStudio](https://www.rstudio.com/)

- Python: <https://www.python.org> 
  -  Suggested build: [Anaconda](https://www.continuum.io/downloads) - many scientific packages preinstalled

- Julia: <http://julialang.org>

Notes
----
- all are interpreted languages
- may have different IDEs for ease of use
- can even use Notepad.exe to edit code 



View on evolution of applications of programming languages
----------------------------------------------------------

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

Oroginal short plan:
--------------------

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
   Econometrics-specific building blocks
   
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
   Expression/readability of code, persoanl aesthetic pleasure  
   Your skillset and background
   Job market popularity 


Good teaching in econometrics = intuition + math formulas + code & data ?

```

Some links
----------

- [Quantitative Economics](http://quant-econ.net) by Thomas Sargent and John Stachurski 

- [Comparison of economics software](http://economics.sas.upenn.edu/~jesusfv/comparison_languages.pdf)

- Comparison of Matlab, R, python, Julia syntax:
  - <http://hyperpolyglot.org/numerical-analysis>
  - <http://www.math.umaine.edu/~hiebeler/comp/matlabR.pdf>
  - <http://mathesaurus.sourceforge.net/matlab-python-xref.pdf>
