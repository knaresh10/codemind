[pattern](https://thecodemind.io/app/discription.php?pageCategory=c3pzTm1NaHFsYWVCeFpGMVpkTDloZz09&Tid=WlpUM09ZdklYSzU5ZUxoRENBREdmQT09&Pid=b3ptTVZKV1BSako3ZkVJNzRMZGJkZz09&Course=eUdCU2wyQVJUZGx4TjltZnFMNEtyZz09&Technology=L2RYTEdBRUMwdnh0Uzh5N0NlMU1iUT09&Topic=aFBtaDFLWFNhWHgrSGxzTGRjVDRWQT09)

 write a logic to print the following pattern.

Input Format :

A single line contains an integer N.

Output Format :

Display the following pattern.

Sample Test Case :

Input :

5

Output :

![image](https://user-images.githubusercontent.com/82667769/194098508-4687b693-1b49-4cd1-89b7-1bd88ff6dff5.png) 


```python
n = int(input())
for i in range(1,n + 1):
    for j in range(1, n + 1):
        if j == 1 or j == i or j == n:
            print("*",end= " ")
        else:
            print(" ",end = " ")
    print("")
