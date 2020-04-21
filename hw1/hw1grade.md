**Joanna Boland**

### Overall Grade: 79/85

### Quality of report: 8/10

* Is the homework submitted (git tag time) before deadline?

    - Yes, `Fri Apr 17 17:37:00`

* Is the final report in a human readable format html?  
	
    - No. `(-2 pts)`

* Is the report prepared as a dynamic document (Jupyter notebook) for better reproducibility?

    - Yes.

* Is the report clear (whole sentences, typos, grammar)? Do readers have a clear idea what's going on and how are results produced by just reading the report?

    - Yes.
 
### Correctness and efficiency of solution: 51/55

* Q1 - N/A

* Q2 (9/10 pts) 

    - `Q2.3` doesn't print `false`, make sure to add `@show` on line 3 or include a separate code chunk to make sure that your output is clear. `(-1 pt)`
	
* Q3 (9/10 pts)

    - `Q3.3` Good observation that the loop using floating point numbers takes many more flops. The reason this is possible is because integer operations fully obey the associative and distributive rules from basic arithmetic. Missing explanation `(-1 pt)`

* Q4 (10/10 pts)

* Q5 (15/15 pts)

    - `Q5.1-3` are good, just note that you're approaching the problem by showing the most general case `Q5.3` first.

    - For question `5.4`, make sure that you are clear about the dimensions of **A**, **U**, **V**, and **I**. The proof is correct, but the detail is helpful. 

* Q6 (8/10 pts)

    - The example for `Q6.5` doesn't demonstrate anything about orthogonality. The identity is **Q****Q**' = **Q**'**Q** = **I**. The given example only shows that **I** **I** = **I**.


### Usage of Git: 5/5

* Is the hw submission put into the `master` branch? 

    - Yes.

* Are there enough commits? Are commit messages clear? 

    - Yes.

* Is the hw1 submission tagged?

    - Yes.

* Are the folders (`hw1`, `hw2`, ...) created correctly?

    - Yes.

* Do not put a lot auxillary files into version control.

    - Yes.


### Reproducibility: 5/5

* Are the materials (files and instructions) submitted to the `master` branch sufficient for reproducing all the results?

    - Yes.

* If necessary, are there clear instructions, either in report or in a separate file, how to reproduce the results?  

    - Not applicable for hw1.


### `Julia` code style: 10/10

* Rule (4): 4 spaces for indenting. 
    
* Rule (6): Never place more than 80 characters on a line.

* Rule (7): Always include a single space after a comma. 
 
* Rule (8):  Never insert a space before a comma.

* Rule (9): Always insert a single space before and after an operator, except for the `^` and `:` operators, which never have spaces around them.

* Rule (12): When naming variables or functions, use short lowercase names if possible.

* Rule (13): If a variable or function name is too long to be read in all lowercase, insert underscores at word boundaries.

* Rule (16): When naming constants, use all caps.
