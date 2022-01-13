# Sudoko_solver
How to solve suduko using Python and recursions concept.

First of all we take input of suduko as a grid of 9/9 matrix type and the zeros in the input are the ones we should find correct ones which replaces those zeros with the numbers between 1 to 9(inclusive)

and we import numpy function to manipulaate the grid look like a suduko or matrix type rather than array type

They are two functions with different work to do

1.possible : This function checks whether a number can be fit in a position suggested.
It checks by the way we solve a suduko puzzle. We generally check wheter any element we are thinking would be a
answer (say element) that element shouldn't be in that particular row('y') and column('x') and we check whether the element is in the seperate 3X3 grid and we return whether the element is possible or not

solve : We generally go to check first the position where the value of the element is zero. So that we can enquire about possibilites in that position. and then we will check all the possible values from 1 to 9 whether they can be replaced with zero in the position using possible. Now we use recursive function to check whether there are any further possible values which can be fit in that position and after all the recursion we will get a grid which is solved.
