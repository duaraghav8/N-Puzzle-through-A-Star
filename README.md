This Python 3.4 implementation solves the N-Puzzle using the A* Search Algorithm with the Hamming function as its admissible Heuristic. The program is extremely slow though. Even for a 3x3 Puzzle, it took about 4 seconds to solve it.

It uses the heapq Data Structure to simulate a priority queue.

**Input Format**

Upon launching the program, the first line must contain an integer *n* to create an NxN Puzzle

n^2 lines follow. Each line contains only 1 integer, which is the tile number for the ith tile. i starts at the top left and ends at bottom right.

0 indicates the empty cell.

The target state is assumed to be:

0 1 2

3 4 5

6 7 8

For example:

**Input**

> python3 n_puzzle.py

3

0

3

8

4

1

7

2

6

5

**Output**

20

DOWN

DOWN

RIGHT

RIGHT

UP

LEFT

LEFT

UP

RIGHT

DOWN

RIGHT

UP

LEFT

DOWN

DOWN

RIGHT

UP

LEFT

LEFT

UP

The Puzzle, upon Input, looks like:

0 3 8

4 1 7

2 6 5

In Output, the first line gives a number *k* - the number of steps it will take to solve the puzzle.
This is followed by k lines, each containing either LEFT, RIGHT, UP, DOWN - the direction in which the empty cell '0' should move.
