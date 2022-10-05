[Print the following pattern](https://thecodemind.io/app/discription.php?pageCategory=c3pzTm1NaHFsYWVCeFpGMVpkTDloZz09&Tid=WlpUM09ZdklYSzU5ZUxoRENBREdmQT09&Pid=dnpxQ2NyUHBTMjE0Z28xbzFnNHNPZz09&Course=eUdCU2wyQVJUZGx4TjltZnFMNEtyZz09&Technology=L2RYTEdBRUMwdnh0Uzh5N0NlMU1iUT09&Topic=aFBtaDFLWFNhWHgrSGxzTGRjVDRWQT09) 

 write a logic to print the following pattern

Input Format :

A single line contains an integer N.

Output Format :

Print the following pattern

Sample Test Case :

Input :

3

Output :

0xx

x0x

xx0

```python
n = int(input())
for i in range(1, n + 1):
    for j in range(1, n + 1):
        if i == j:
            print("0",end="")
        else:
            print("x",end="")
    print("")
