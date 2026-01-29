### Task
Given an integer,n, and n  space-separated integers as input, create a tuple, , of those  integers. Then compute and print the result of hash(t) .

Note: hash() is one of the functions in the __builtins__ module, so it need not be imported.

### Input Format

The first line contains an integer,n , denoting the number of elements in the tuple.
The second line contains n space-separated integers describing the elements in tuple t.

### Output Format

Print the result of hash(t).

### Sample Input 0

2

1 2

### Sample Output 0

3713081631934410656

### Explaination

The program takes an integer n (number of elements).

It reads n space-separated integers from input.

Converts the list of integers into a tuple (because lists can’t be hashed).

Prints the hash value of that tuple.
