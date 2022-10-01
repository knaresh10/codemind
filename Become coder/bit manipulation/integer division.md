 Problem Statement

Given an integer X between −10 ^18 and 10^18 (inclusive), print ⌊X/10⌋.

Notes
For a real number x, ⌊x⌋ denotes "the maximum integer not exceeding x". For example, we have ⌊4.7⌋=4,⌊−2.4⌋=−3, and ⌊5⌋=5. (For more details, please refer to the description in the Sample Input and Output.)


All values in input are integers.
Input
Input is given from Standard Input in the following format:

X
Output
print ⌊X/10⌋.

Note that it should be output as an integer.

Sample Input 1 
47
Sample Output 1 
4
[47/10] =4.7 are all the negative integers, 0,1,2,3, and 4. The maximum integer among them is 4, so we have  [47/10] =4.

Sample Input 2 
-24
Sample Output 2 
-3
Since the maximum integer not exceeding  
−24/10 =−2.4 is −3, we have [−24/10]=−3.
Note that −2 does not satisfy the condition, as −2 exceeds −2.4.

Sample Input 3 
50
Sample Output 3 
5

Sample Input 4 
-30
Sample Output 4 
-3

Sample Input 5 
987654321987654321
Sample Output 5 
98765432198765432
The answer is 98765432198765432. Make sure that all the digits match.

```python
 n = int(input())
print(n // 10)
