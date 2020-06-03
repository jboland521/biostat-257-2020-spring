*Joanna Boland*

### Overall Grade: 129/135

### Quality of report: 9/10

* Is the homework submitted (git tag time) before deadline?

    - No. Tagged at `Mon Jun 1 20:39:09`. `(-1 pt)`

* Is the final report in a human readable format html?

    - Yes.

* Is the report prepared as a dynamic document (Jupyter notebook) for better reproducibility?
    
    - Yes.

* Is the report clear (whole sentences, typos, grammar)? Do readers have a clear idea what's going on and how are results produced by just reading the report?
    
    - Yes.


### Correctness and efficiency of solution: 105/110

* Q1

    * Q1.1 (9/15 **bonus** pts)

        - Missing gradient wrt **L**. `(-5 pts)`

        - You dont have much detail for your derivation, its easy to get the gradient wrt **β**, but it isn't as clear to get the gradient wrt σ<sup>2</sup>. `(-1 pt)`

    * Q2.2 (0/15 **bonus** pts)

        - No derivation given `(-15 pts)`

* Q2

    * Q2.1 (10/10 pts)
    
    * Q2.2 (10/10 pts)

* Q3

* Q4

    * Q4.2 (10/10 pts)
    
    * Q4.3 (0/10 pts)

        - You have a line `BLAS.axpby!(T(con), ones(1), T(0), obs.∇σ²)` when evaluating the gradient, this allocates a 1 by 1 vector on each evaluation of gradient since we evaluate this for every person in the data. So 96 bytes * 1000 persons is about 96 KiB. Which is very close to your actual allocation.

* Q5

    * Q5 Starting Point (10/10 pts)

        - Note: ∥A∥<sup>2</sup><sub>F</sub> = Tr(A<sup>T</sup>A). You have a small typo.

        - Good job on getting the correct starting point.
    
    * Q5.1 (10/10 pts)
    
    * Q5.2 (10/10 pts)

* Q6

* Q7

    * Q7.1 (10/10 pts)

        - The optimality condition has been slightly relaxed. Since your ∥gradient∥ < 0.17, you get full points.
    
    * Q7.2 (10/10 pts)

* Q8 (8/10 pts)

    - You've given a table, but haven't summarized the results in words. `(-2 pts)`

* Q9 (8/10 pts)

    - You've given a table, but haven't summarized the results in words. `(-2 pts)`

* Q10


### Usage of Git: 5/5

* Is the hw submission put into the `master` branch?

    - Yes.

* Are there enough commits? Are commit messages clear? 

    - Yes.

* Is the hw4 submission tagged?

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


### Julia code style: 5/5

* Rule (4): 4 spaces for indenting. 
    
* Rule (6): Never place more than 80 characters on a line.

* Rule (7): Always include a single space after a comma. 

* Rule (8):  Never insert a space before a comma.

* Rule (9): Always insert a single space before and after an operator, except for the `^` and `:` operators, which never have spaces around them.

* Rule (12): When naming variables or functions, use short lowercase names if possible.

* Rule (13): If a variable or function name is too long to be read in all lowercase, insert underscores at word boundaries.

* Rule (16): When naming constants, use all caps.
