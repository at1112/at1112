# Coding Discussion 05

# Instructions

For this coding assignment, I'll propose three coding tasks that draws on some of the linear algebra concepts we've been working through. Each prompt considers a world where `numpy` was never created, requiring you to build some of the operations we've been discussing _from scratch_.

## Task 1

Say we live in a world where the `numpy` module doesn't exist and we have to deal with data represented as nested list objects. Write a function that _transposes_ a matrix.

Test it on the following matrix:

```Python
B = [[-1,0,2],
     [2,1,0],
     [8,3,2],
     [1,0,2]]
```

The output should look something like the following:

```Python
transpose(B)

[[-1,  2,  8,  1],
 [ 0,  1,  3,  0],
 [ 2,  0,  2,  2]]
```

Use only Python's standard library to perform the necessary computations. Do not import a third party package.


## Task 2

Again, we still live in a world where the `numpy` module doesn't exist. Write a function that computes the dot product of the following two matrices represented as nested lists.

```python
A = [[1,3,4],
     [0,-1,2],
     [2,4,8]]

B = [[-1,0,2],
     [2,1,0],
     [8,3,2],
     [1,0,2]]
```

Name this function `dot_product()` which takes two nested lists as inputs, and outputs the dot product. Make sure the function throws an error if the inputs are incorrect.

Use only Python's standard library to perform the necessary computations. Do not import a third party package.

## Task 3

Write a function that calculates the inverse of the following matrix. Note that the matrix **A** should be transformed into a 2x2 matrix. Use the functions from tasks 1 and 2 to accomplish this.

```python
A = [[1,3],
     [0,-1],
     [2,4]]
```

Name this function `invert()` which takes a nested list as input and outputs the inversed matrix. Use only Python's standard library to perform the necessary computations. Do not import a third party package.


## Submit

Please submit your answer as a Jupyter Notebook in the `Submissions/` folder. Title the notebook with your lastname_firstname_netid (`doe_john_jd568.ipynb`). Be sure to submit a docstring if you write any functions indicating what your function does and all the arguments it takes.  As per usual, please submit your answer to the class repository by Friday 11:59pm deadline.

## Response

Please do not respond to anyone's code until after the Friday deadline. Please submit a response by Sunday 11:59pm. Your response should come in the form of a contribution or edit to someone else's code (not just a comment).

- Is there a way you could potentially improve open the logic they laid out by say making the code more concise or efficient?
- Is there another way you could structure the manipulation so that it played out in less steps?
