[question](https://thecodemind.io/app/discription.php?pageCategory=c3pzTm1NaHFsYWVCeFpGMVpkTDloZz09&Tid=WlpUM09ZdklYSzU5ZUxoRENBREdmQT09&Pid=dTdrdlk2aUNpclJod0JGbkpYZi9SQT09&Course=eUdCU2wyQVJUZGx4TjltZnFMNEtyZz09&Technology=L2RYTEdBRUMwdnh0Uzh5N0NlMU1iUT09&Topic=aFBtaDFLWFNhWHgrSGxzTGRjVDRWQT09) 

write  a logic to print the following pattern

Input Format :

A single line contains an integer N.

Output Format :

Display the following pattern.

Sample Test Case :

Input

5

Output

x000x

0x0x0

00x00

0x0x0

x000x

Input :

4

Output :

x00x

0xx0

0xx0

x00x


```python
n = int(input())
for i in range(1, n + 1):
    for j in range(1, n + 1):
        if j == i or j == n - i + 1:
            print("x",end="")
        else:
            print("0",end="")
    print("")
