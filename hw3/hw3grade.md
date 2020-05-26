*Joanna Boland*

### Overall Grade: 118/125

### Quality of report: 10/10

* Is the homework submitted (git tag time) before deadline?

    - Yes. `Fri May 15 20:02:14`

* Is the final report in a human readable format html?

    - Yes.

* Is the report prepared as a dynamic document (Jupyter notebook) for better reproducibility?
    
    - Yes.

* Is the report clear (whole sentences, typos, grammar)? Do readers have a clear idea what's going on and how are results produced by just reading the report?
    
    - Yes.


### Correctness and efficiency of solution: 93/100

* Q1 (3/5 pts)

    - There is a mistake in the expression of **P**. The transition matrix **P** should be the sum of a matrix product involving **A** and say **D** and the outer product of a rank-one vector (say **z**) and **1'**. ie. **P** = **DA** + **Z1**'. Your code further down appears correct, so be clearer with your notation. `(-2 pts)`

* Q2 

* Q3 (10/10 pts)

* Q4 (5/5 pts) 

* Q5

    * Step 1 (12/15 pts)

        - Note that `sleep(1e-2)` should be removed from your final code, its just a placeholder. This is where your extra allocations happen.

        - `pgrksol.csv` in repository. This was specifically asked to **avoid** doing. `(-3 pts)`

    * Step 2 (18/20 pts)

    * Step 3 (20/20 pts)

    * Step 4 (20/20 pts)

* Q6 (5/5 pts) 

* Q7


### Usage of Git: 5/5

* Is the hw submission put into the `master` branch?

    - Yes.

* Are there enough commits? Are commit messages clear? 

    - Yes.

* Is the hw3 submission tagged?

    - Yes.

* Are the folders (`hw1`, `hw2`, ...) created correctly?

    - Yes.

* Do not put a lot auxillary files into version control.  
    
    - Yes.


### Reproducibility: 5/5

* Are the materials (files and instructions) submitted to the `master` branch sufficient for reproducing all the results? 

    - Yes.

* If necessary, are there clear instructions, either in report or in a separate file, how to reproduce the results?  

    - Not Applicable.


### Julia code style: 5/5

* Rule (4): 4 spaces for indenting. 
    
* Rule (6): Never place more than 80 characters on a line.

* Rule (7): Always include a single space after a comma. 

* Rule (8):  Never insert a space before a comma.

* Rule (9): Always insert a single space before and after an operator, except for the `^` and `:` operators, which never have spaces around them.

* Rule (12): When naming variables or functions, use short lowercase names if possible.

* Rule (13): If a variable or function name is too long to be read in all lowercase, insert underscores at word boundaries.

* Rule (16): When naming constants, use all caps.
