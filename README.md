# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: Naked twins can be used as the 4th strategy to solve sudoku. In Naked twin we find 2 boxes(twins) with the same 2 possible digits allowed in them, part of the same unit(row/column/square/diagonl). On finding a twin we can eliminate the 2 possible digits in them from all their peers in the unit. Thereby reducing the number of possibilites in constraint propagation.

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: The Strategies used for Diagonal Sudoku will be the same as normal sudoku - Eliminate, Only choice, Naked Twins and Search. The difference will be the units considered. Two new units will be added namely left diagonal and right diagonal to the row, columns and square units. Constraint propagation will now be used on all theses units.

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.

### References
https://github.com/Tuuleh/insight_challenge
https://github.com/nikhilranjan7/sudoku-solver
