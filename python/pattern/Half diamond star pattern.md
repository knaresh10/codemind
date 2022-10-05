 Write a program to print the half diamond star pattern. The pattern is printing depending upon the input value which is supplied by the user. The input value is in between 3 and 100.

Constrains:

3<=n<=100 if n is input value.

Example 1:  If input value is 5 then the pattern is

Input:

5

Output:

![image](https://user-images.githubusercontent.com/82667769/194090578-85b98e04-5393-4e6c-b9d9-d9811b3e79c8.png)


Input Format

First Line specifying the number 
Output Format

Display pattern


```python
n = int(input())
if(n < 3 or n > 100):
    print("The pattern is not possible")
else:
    for i in range(1,n + 1):
        print("*"*i)
    for i in range(n -1, 0, -1):
        print("*"*i)
