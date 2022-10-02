Convert a Decimal Number to Binary Number

Vivek is Playing with number system and his teacher given him a task to convert Decimal number to its respective Binary number, help him to complete the task

Input Format:

First line contains an integer Q which indicates the number of queries.

Next Q lines contains a number.

Output Format:

Display its respective Binary number in Q lines.

Sample Input:

3

7

9

12

Sample Output:

111

1001

1100

Constraints:

1<=Q<=100

1<=N<=1000

```python
tc = int(input())
for i in range(tc):
    print(bin(int(input()))[2:])
