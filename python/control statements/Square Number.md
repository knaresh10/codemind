Given an integer n, write a function to return True, if it is possible to represent it as a sum of the squares of two different integers, else return False.

Sample input:

25

Sample output:

True

```python
n = int(input())
flag = 0
for i in range(int(n ** 0.5) + 1):
    for j in range(int(n ** 0.5) + 1):
        if i * i + j * j == n:
            print("True")
            flag = 1
            break
    if flag :
        break
else:
    print("False")
