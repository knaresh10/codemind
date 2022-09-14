Given an array of length N consisting of only 0s and 1s in random order. Modify the array to segregate 0s on left side and 1s on the right side of the array (Sort the array).

Note: Don't use sort function or any sorting techniques. 

Example 1:

Input:
5

0 0 1 1 0

Output: 0 0 0 1 1



Example 2:

Input:
4

1 1 1 1

Output: 1 1 1 1

Explanation: There are no 0 in the given array, so the modified array is 1 1 1 1.

Your Task:

You don't need to read input or print anything. Your task is to write the program that takes n and arr elements as input and sorts arr[] in-place without using any extra memory. Print the elements separated by a space.



Expected Time Complexity: O(N)

Expected Auxiliary Space: O(1)


```python
n = int(input())
li = list(map(int,input().split()))

l = 0
r = n - 1

while l < r:
    while li[l] == 0 and l < r:
        l += 1
    while li[r] == 1 and r > l:
        r -= 1
    
    if l < r:
        li[l], li[r] = li[r], li[l]
        l += 1
        r -= 1

print(*li)
        
