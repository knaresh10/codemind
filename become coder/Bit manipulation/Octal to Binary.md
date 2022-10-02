 Convert an Octal Number to Binary Number

Tevitt is Playing with number system and his teacher given him a task to convert Octal number to its respective Binary number, help him to complete the task

Input Format:

First line contains an integer Q which indicates the number of queries.

Next Q lines contains a number.

Output Format:

Display its respective Binary number in Q lines.

Sample Input:

3

33

70

210

Sample Output:

11011

111000

10001000

```python
tc = int(input())
for i in range(tc):
    print(bin(int(input(),8))[2:])
