 Convert a Hexadecimal Number to Binary Number

Tevitt is Playing with number system and his teacher has given him a task to convert Hexadecimal number to its respective Bnary number, help him to complete the task

Input Format:

First line contains an integer Q which indicates the number of queries.

Next Q lines contains a number.

Output Format:

Display its respective Binary number in Q lines.

Sample Input:

3

1A

123B

12C

Sample Output:

00011010
0001001000111011
000100101100

```cpp
#include<bits/stdc++.h>
using namespace std;
int main() {
	unordered_map<char, string>hexa{{'0',"0000"},{'1',"0001"},
	{'2',"0010"},{'3',"0011"},{'4',"0100"},{'5',"0101"},
	{'6',"0110"},{'7',"0111"},{'8',"1000"},{'9',"1001"},
	{'A',"1010"},{'B',"1011"},{'C',"1100"},{'D',"1101"},
	{'E',"1110"},{'F',"1111"},};
	int tc;
	cin >> tc;
	while(tc--) {
		string s;
		cin >> s;
		for(auto x : s)
			cout << hexa[x];
		cout << "\n";
	}
}

```
