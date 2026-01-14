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

# Task 4

Given the participants' score sheet for your University Sports Day, you are required to find the runner-up score. You are given n scores. Store them in a list and find the score of the runner-up.

### Input Format

The first line contains n.
The second line contains an array A[] of n integers each separated by a space.

### Constraints

2 ≤ n ≤ 10

−100 ≤ A[i] ≤ 100

### Output Format

Print the runner-up score.

### Sample Input 0
5

2 3 6 6 5

### Sample Output 0
5

### Explanation 0

Given list is [2, 3, 6, 6, 5]. The maximum score is 6, second maximum is 5. Hence, we print 5 as the runner-up score.

# Task 5

The provided code stub will read in a dictionary containing key/value pairs of name:[marks] for a list of students. Print the average of the marks array for the student name provided, showing 2 places after the decimal.

## Example

marks key:value pairs are

'alpha': [20, 30, 40]
'beta': [30, 50, 70]

query_name = 'beta'

The query_name is 'beta'. beta's average score is

(
30
+
50
+
70
)
/
3
=
50.0
(30+50+70)/3=50.0

### Input Format

The first line contains the integer n, the number of students' records.
The next n lines contain the names and marks obtained by a student, each value separated by a space.
The final line contains query_name, the name of a student to query.

### Constraints

2
≤
𝑛
≤
10
2≤n≤10

0
≤
marks
[
𝑖
]
≤
100
0≤marks[i]≤100

length of marks arrays = 3

### Output Format

Print one line: The average of the marks obtained by the particular student correct to 2 decimal places.

### Sample Input 0
3
Krishna 67 68 69
Arjun 70 98 63
Malika 52 56 60
Malika

### Sample Output 0
56.00

Explanation 0

Marks for Malika are {52, 56, 60} whose average is:

52
+
56
+
60/
3
=
56

### Sample Input 1
2
Harsh 25 26.5 28
Anurag 26 28 30
Harsh

### Sample Output 1

26.50

# Task 6

You are given the firstname and lastname of a person on two different lines. Your task is to read them and print the following:

Hello firstname lastname! You just delved into python.

## Function Description

Complete the print_full_name function in the editor below.

print_full_name has the following parameters:

string first: the first name
string last: the last name

### Prints

string: 'Hello firstname lastname! You just delved into python.' where firstname and lastname are replaced with first and last.

### Input Format
The first line contains the first name, and the second line contains the last name.

### Constraints
The length of the first and last names are each ≤ 10.

### Sample Input 0

Ross
Taylor


### Sample Output 0

Hello Ross Taylor! You just delved into python.

### Explanation 0

The input read by the program is stored as a string data type. A string is a collection of characters.

# Task 7

Happiness score

## Problem

You are given an array and two sets A and B.
For each element:

+1 happiness if in A

-1 happiness if in B

Print the final happiness score.

 ### Sample Input
3 2
1 5 3
3 1
5 7

### Sample Output
1

# Task 8

We have seen that lists are mutable (they can be changed), and tuples are immutable (they cannot be changed).

Let's try to understand this with an example.

You are given an immutable string, and you want to make changes to it.

## Example

>>> string = "abracadabra"
You can access an index by:

>>> print string[5]
a
What if you would like to assign a value?

>>> string[5] = 'k' 
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'str' object does not support item assignment
How would you approach this?

One solution is to convert the string to a list and then change the value.

## Example

>>> string = "abracadabra"
>>> l = list(string)
>>> l[5] = 'k'
>>> string = ''.join(l)
>>> print string
abrackdabra
Another approach is to slice the string and join it back.

## Example

>>> string = string[:5] + "k" + string[6:]
>>> print string
abrackdabra

### Task
Read a given string, change the character at a given index and then print the modified string.
Function Description

Complete the mutate_string function in the editor below.

mutate_string has the following parameters:

string string: the string to change
int position: the index to insert the character at
string character: the character to insert

### Returns

string: the altered string

### Input Format

The first line contains a string, string.
The next line contains an integer position, the index location and a string character, separated by a space.

### Sample Input
STDIN           Function
-----           --------
abracadabra     s = 'abracadabra'
5 k             position = 5, character = 'k'

### Sample Output
abrackdabra

