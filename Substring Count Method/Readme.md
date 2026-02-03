<h2><a href="https://leetcode.com/problems/department-highest-salary">Substring Count Method</a></h2> <img src='https://img.shields.io/badge/Difficulty-Medium-orange' alt='Difficulty: Medium' /><hr>

In this challenge, the user enters a string and a substring. You have to print the number of times that the substring occurs in the given string. String traversal will take place from left to right, not from right to left.

### NOTE: String letters are case-sensitive.

### Input Format

The first line of input contains the original string. The next line contains the substring.

### Constraints
1<=len(String)<=200

Each character in the string is an ascii character.

### Output Format

Output the integer number indicating the total number of occurrences of the substring in the original string.

### Sample Input
ABCDCDC
CDC

### Sample Output
2

### Concept

There are a couple of new concepts:
In Python, the length of a string is found by the function len(s), where s is the string.
To traverse through the length of a string, use a for loop:

for i in range(0, len(s)):

    print (s[i])
A range function is used to loop over some length:

range (0, 5)

Here, the range loops over 0 to 4. 5 is excluded.

### Example

This program counts how many times a substring appears inside a string.

It checks each position using slicing and increments count when matched.

Finally, it prints the total count.

