[print the following pattern](https://thecodemind.io/app/discription.php?pageCategory=c3pzTm1NaHFsYWVCeFpGMVpkTDloZz09&Tid=WlpUM09ZdklYSzU5ZUxoRENBREdmQT09&Pid=eDdqYzJidml5cGFLMEhQNThJMHowdz09&Course=eUdCU2wyQVJUZGx4TjltZnFMNEtyZz09&Technology=L2RYTEdBRUMwdnh0Uzh5N0NlMU1iUT09&Topic=aFBtaDFLWFNhWHgrSGxzTGRjVDRWQT09)

 write the logic to print the following pattern

Input Format :

A single line contains an integer N.

Output Format :

Display the following pattern based on integer N.

Sample Test Case :

Input :

5

Output :

54321

54321

54321

54321

54321

```python
n = int(input())
for i in range(n):
    for j in range(n,0,-1):
        print(j,end=" ")
    print("")
