 Convert an Binary Number to Octal Number

Tevitt is Playing with number system and his teacher has given him a task to convert Binary number to its respective Octal number, help him to complete the task

Input Format:

First line contains an integer Q which indicates the number of queries.

Next Q lines contains a number.

Output Format:

Display its respective Octal number in Q lines.

Sample Input:

3

11011

111000

10001000

Sample Output:

33

70

210

```python
tc = int(input())
for i in range(tc):
    print(oct(int(input(),2))[2:])
