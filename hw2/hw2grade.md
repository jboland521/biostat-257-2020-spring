*Joanna Boland*

### Overall Grade: 92/110

### Quality of report: 9/10

* Is the homework submitted (git tag time) before deadline?

    - No. Tagged at `Sun May 3 19:08:48`. Additional commits made after submission. No points deducted for tag time per email, but make sure that the repository is complete with `.ipynb` *and* `.html` when submitting. `(-1 pt)`

* Is the final report in a human readable format html?  
	
    - Yes.

* Is the report prepared as a dynamic document (Jupyter notebook) for better reproducibility?
    
    - Yes.

* Is the report clear (whole sentences, typos, grammar)? Do readers have a clear idea what's going on and how are results produced by just reading the report?
    
    - Yes.


### Correctness and efficiency of solution: 83/100

* Q1 (10/10 pts)

* Q2 
	
* Q3 (10/15 pts)

    - In your `logl!` function, be careful when calling `mul!(obs.ztz, obs.storage_qq2, (1/σ²))` and `M = cholesky!(Symmetric(obs.ztz))`. Since `obs.ztz` is an input parameter you want to make sure that you are not modifying it when computing the log-likelihood. On a second run, the function will not return the correct answer. This appears to be why you failed the `@assert!` call. `(-5 pts)`

* Q4 (19/30 pts)

    - Your code could be made substantially faster by thinking about the dimensions carefully at each step of the algorithm. Note that `(y - Xβ)` and `Zᵀ (y - Xβ)` can be computed in an easier way. Since `(y - Xβ)ᵀ (y - Xβ) = yᵀy -2yᵀXβ + βᵀXᵀXβ` and `Zᵀ (y - Xβ) = Zᵀy - ZᵀXβ)`. Note that many of these quantities can be **precomputed** before the main function call since they only depend on `Z`, `X`, and `y`.
    
    - Use `transpose(X)` rather than `X'`, using adjoint has additional overhead.

* Q5 (30/30 pts)

* Q6 (14/15 pts) 

    - See below.


### Usage of Git: 5/5

* Is the hw submission put into the `master` branch?

    - Yes.

* Are there enough commits? Are commit messages clear? 

    - Yes.

* Is the hw2 submission tagged?

    - Yes.

* Are the folders (`hw1`, `hw2`, ...) created correctly?

    - Yes.

* Do not put a lot auxillary files into version control.  
    
    - Yes.

### Reproducibility: 5/5

* Are the materials (files and instructions) submitted to the `master` branch sufficient for reproducing all the results? 

    - Yes.

* If necessary, are there clear instructions, either in report or in a separate file, how to reproduce the results?  

    - Yes.


### Julia code style: 4/5

* Rule (4): 4 spaces for indenting. 
    
* Rule (6): Never place more than 80 characters on a line.

* Rule (7): Always include a single space after a comma. 

* Rule (8):  Never insert a space before a comma.

* Rule (9): Always insert a single space before and after an operator, except for the `^` and `:` operators, which never have spaces around them. `(-1 pt)`

    - `1/ (2 * σ²) * dot(obs.res, obs.res)` Missing spaces around `/`
    
    - `mul!(obs.ztz, obs.storage_qq2, (1/σ²))` Missing spaces around `/`

* Rule (12): When naming variables or functions, use short lowercase names if possible.

* Rule (13): If a variable or function name is too long to be read in all lowercase, insert underscores at word boundaries.

* Rule (16): When naming constants, use all caps.
