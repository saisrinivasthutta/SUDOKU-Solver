# Sudoku solver

Sudoku solver using backtracking

Basically in sudoku, we want to be able to solve a sudoku puzzle given an input like this,
which represents a sudoku board:

```
[[x00, x01, x02, x03... x08],
 [x10, x11, x12, x13... x18],
 ...
 [x80, x81, x82, x83... x88]]
```

These x_rc values correspond to the value at the rth row, cth column (starting with 0-index)
These values could be empty (we will represent this with -1)

So for example,

```
[[-1,  1,  5, ...],
 [-1, -1, -1, ...],
 [ 6, -1, -1, ...]
 ...]
```

would represent a board like this:

```
 -----------
|     1   5 | ...
|           | ...
| 6         | ...
 -----------
 ...
```

Now, our goal is to solve our sudoku puzzle using Python! :D

By running sudoku.py file we are able to solve this problem

You can see the output upon running
Solve This Board :
[[3, 9, -1, -1, 5, -1, -1, -1, -1],
    [-1, -1, -1, 2, -1, -1, -1, -1, 5],
    [-1, -1, -1, 7, 1, 9, -1, 8, -1],
    [-1, 5, -1, -1, 6, 8, -1, -1, -1],
    [2, -1, 6, -1, -1, 3, -1, -1, -1],
    [-1, -1, -1, -1, -1, -1, -1, -1, 4],
    [5, -1, -1, -1, -1, -1, -1, -1, -1],
    [6, 7, -1, 1, -1, 5, -1, 4, -1],
    [1, -1, 9, -1, -1, -1, 2, -1, -1]]
Board Solved :
[[3, 9, 1, 8, 5, 6, 4, 2, 7],
    [8, 6, 7, 2, 3, 4, 9, 1, 5],
    [4, 2, 5, 7, 1, 9, 6, 8, 3],
    [7, 5, 4, 9, 6, 8, 1, 3, 2],
    [2, 1, 6, 4, 7, 3, 5, 9, 8],
    [9, 3, 8, 5, 2, 1, 7, 6, 4],
    [5, 4, 3, 6, 9, 2, 8, 7, 1],
    [6, 7, 2, 1, 8, 5, 3, 4, 9],
    [1, 8, 9, 3, 4, 7, 2, 5, 6]]

To run this in your System Download the file and run the file in command line
(Make sure you have python installed in your system)
