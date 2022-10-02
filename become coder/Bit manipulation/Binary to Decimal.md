 Convert a Binary Number to Decimal Number

Vivek is Playing with number system and his teacher given him a task to convert Binary number to its respective Decimal number, help him to complete the task

Input Format:

First line contains an integer Q which indicates the number of queries.

Next Q lines contains a number.

Output Format:

Display its respective Binary number in Q lines.

Sample Input:

3

111

1001

1100

Sample Output:

7

9

12

```python
tc = int(input())
for i in range(tc):
    print(int(input(),2))
