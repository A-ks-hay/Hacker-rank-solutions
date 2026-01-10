# Hacker-rank-solutions

# Task 1

Given an integer, n, perform the following conditional actions:

If n is odd, print Weird

If n is even and in the inclusive range of 2 to 5, print Not Weird

If n is even and in the inclusive range of 6 to 20, print Weird

If n is even and greater than 20, print Not Weird

# Input Format

A single line containing a positive integer, n.

Constraints

1≤𝑛≤100

# Output Format

Print Weird if the number is weird. Otherwise, print Not Weird.

## Sample Input 0

3


## Sample Output 0

Weird

## Explanation 0

n = 3
n is odd and odd numbers are weird, so print Weird.


## Sample Input 1

24


## Sample Output 1

Not Weird


## Explanation 1

n = 24

n > 20 and n is even, so it is not weird.


# Task 2

An extra day is added to the calendar almost every four years as February 29, and the day is called a leap day. It corrects the calendar for the fact that our planet takes approximately 365.25 days to orbit the sun. A leap year contains a leap day.

In the Gregorian calendar, three conditions are used to identify leap years:

The year can be evenly divided by 4, is a leap year, unless:

The year can be evenly divided by 100, it is NOT a leap year, unless:

The year is also evenly divisible by 400. Then it is a leap year.

This means that in the Gregorian calendar, the years 2000 and 2400 are leap years, while 1800, 1900, 2100, 2200, 2300 and 2500 are NOT leap years.
Source

## Problem

Given a year, determine whether it is a leap year. If it is a leap year, return the Boolean True, otherwise return False.

Note that the code stub provided reads from STDIN and passes arguments to the is_leap function. It is only necessary to complete the is_leap function.

### Input Format

Read year, the year to test.

#### Constraints

1900 ≤ year ≤ 10⁵

### Output Format

The function must return a Boolean value (True/False). Output is handled by the provided code stub.

### Sample Input 
1990

### Sample Output 
False

### Explanation 

1990 is not a multiple of 4, hence it's not a leap year.


# Task 3

Let’s learn about list comprehensions! You are given three integers x, y, and z representing the dimensions of a cuboid along with an integer n. Print a list of all possible coordinates given by (i, j, k) on a 3D grid where the sum of i + j + k is not equal to n.
Here,
0 ≤ i ≤ x, 0 ≤ j ≤ y, 0 ≤ k ≤ z.

Please use list comprehensions rather than multiple loops, as a learning exercise.

## Example
x = 1
y = 1
z = 2
n = 3


All permutations of [i, j, k] are:

[[0, 0, 0], [0, 0, 1], [0, 0, 2], [0, 1, 0], [0, 1, 1], [0, 1, 2],
 [1, 0, 0], [1, 0, 1], [1, 0, 2], [1, 1, 0], [1, 1, 1], [1, 1, 2]]


Print an array of the elements that do not sum to n = 3:

[[0, 0, 0], [0, 0, 1], [0, 0, 2], [0, 1, 0], [0, 1, 1],
 [1, 0, 0], [1, 0, 1], [1, 1, 0], [1, 1, 2]]

### Input Format

Four integers x, y, z, and n, each on a separate line.

### Constraints

Print the list in lexicographic increasing order.

### Sample Input 0
1

1

1

2

### Sample Output 0
[[0, 0, 0], [0, 0, 1], [0, 1, 0], [1, 0, 0], [1, 1, 1]]

### Explanation 0

Each variable x, y, and z will have values of 0 or 1.
All permutations of lists in the form [i, j, k] are:

[[0, 0, 0], [0, 0, 1], [0, 1, 0], [0, 1, 1],
 [1, 0, 0], [1, 0, 1], [1, 1, 0], [1, 1, 1]]


Remove all arrays that sum to n = 2 to leave only the valid permutations.

### Sample Input 1
2

2

2

2

### Sample Output 1

[[0, 0, 0], [0, 0, 1], [0, 1, 0], [0, 1, 2], [0, 2, 1], [0, 2, 2], [1, 0, 0], [1, 0, 2], [1, 1, 1], [1, 1, 2], [1, 2, 0], [1, 2, 1], [1, 2, 2], [2, 0, 1], [2, 0, 2], [2, 1, 0], [2, 1, 1], [2, 1, 2], [2, 2, 0], [2, 2, 1], [2, 2, 2]]
