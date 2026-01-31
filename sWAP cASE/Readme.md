You are given a string and your task is to swap cases. In other words, convert all lowercase letters to uppercase letters and vice versa.

### For Example:

Www .HackerRank. com → wWW .hACKERrANK. COM

Pythonist 2 → pYTHONIST 2 

## Function Description

Complete the swap_case function in the editor below.

swap_case has the following parameters:

string s: the string to modify

## Returns

string: the modified string

## Input Format

A single line containing a string s.

### Constraints

0<len(s)<1000

## Sample Input 0

HackerRank.com presents "Pythonist 2".

## Sample Output 0

hACKERrANK.COM PRESENTS "pYTHONIST 2".

## Explaination:

def swap_case(s):
    return s.swapcase()
    
### Creates a function that changes uppercase to lowercase and lowercase to uppercase using Python’s built-in swapcase() method.

if __name__ == '__main__':

### Runs the code only when the file is executed directly.

s = input()

### Takes input from the user.

result = swap_case(s)
print(result)

### Calls the function and prints the swapped string.
