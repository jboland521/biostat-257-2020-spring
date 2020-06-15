*Joanna Boland*

### Overall Grade: 93/135

### Quality of report: 4/10

* Is the homework submitted (git tag time) before deadline?

    - No. `Thu Jun 11 13:12:08` `(-6 pts)`

* Is the final report in a human readable format html?

    - Yes.

* Is the report prepared as a dynamic document (Jupyter notebook) for better reproducibility?
    
    - Yes.

* Is the report clear (whole sentences, typos, grammar)? Do readers have a clear idea what's going on and how are results produced by just reading the report?
    
    - Yes.


### Correctness and efficiency of solution: 74/110

* Q1 (10/10 pts)

* Q2 (16/20 pts)
    
    - Make sure to index your updates `(-3 pts)` 
        
        - **β**<sup>(t+1)</sup>>|**γ**, **y**, σ<sup>2</sup> <sup>(t)</sup>

        - σ<sup>2</sup> <sup>(t+1)|**γ**, **y**, **β**<sup>(t+1)</sup>

        - **Σ** <sup>(t+1)</sup> | **γ** **γ**<sup>T</sup>

    - You have **β** = ∑<sub>i</sub> <big>(</big> **X** <sub>i</sub><sup>T</sup>**y**<sub>i</sub> + **X**<sub>i</sub><sup>T</sup>**Z**<sub>i</sub> 𝔼(**γ**<sub>i</sub>∣**y**<sub>i</sub>) <big>)</big> / ∑<sub>i</sub> <big>(</big>**X**<sub>i</sub><sup>T</sup> **X**<sub>i</sub> <big>)</big>. This is incorrect notation, use (∑<sub>i</sub> <big>[</big>**X**<sub>i</sub><sup>T</sup> **X**<sub>i</sub>)<sup>-1</sup>. `(-1 pts)`


* Q3

    - Q3.1 (8/10 pts)

            - You forgot to run with `updater = true`, I've rerun with fixing the input argument. `(-2 pts)`
    
    - Q3.2 (10/10 pts) 

* Q4

* Q5

* Q6
    
    - Q6.1 (0/10 pts)

        - Your update to σ<sup>2</sup> is incorrect.
    
    - Q6.2 (0/10 pts)

    - Q6.3 (0/10 pts)

* Q7

* Q8

* Q9 
    
    - Q9.1 (10/10 pts)

    - Q9.2 (10/10 pts)

* Q10 (10/10 pts)

    - The quasi-newton based algorithms are actually much *faster* (about 10x) than EM. If you actually evaluate the Hessian you can get 30x faster on this problem. The advantage of EM is in fact that the each update is much easier to compute than a newton step.

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
    
    -  Yes.


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
