

Problem StatementIn the figure shown in the image below, are the points numbered a and b directly connected by a line segment?

Constraints
1≤a
a and b are integers.
InputInput is given from Standard Input in the following format:

a b


OutputIf the points numbered a and b are directly connected by a line segment, print Yes; otherwise, print No.
The judge is case-sensitive: be sure to print uppercase and lowercase letters correctly.

Sample Input 14 5


Sample Output 1Yes


Explanation:

In the figure shown in the Problem Statement, the points numbered 4 and 5 are directly connected by a line segment.
Thus, Yes should be printed.

Sample Input 2 3 5


Sample Output 2 No


Explanation:

In the figure shown in the Problem Statement, the points numbered 33 and 55 are not directly connected by a line segment.
Thus, No should be printed.

```python 
a, b = map(int,input().split())
if abs(a - b) == 1 or (a == 10 and b == 1) or (a == 1 and b == 10):
    print('Yes')
else:
    print('No')
