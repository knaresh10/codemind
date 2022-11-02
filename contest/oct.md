```cpp
#include<bits/stdc++.h>
using namespace std;
int helper(int ind, string &s, vector<int>&v, int cnt) {
	if (ind == v.size()) {
		return cnt;
	}
	int a = 0;
	//cout << s[ind] << " " << s[ind + 1] << " " << cnt << endl;
	if (ind != v.size() - 1 && s[ind] == '0' && s[ind + 1] == '1') {
		//cout << "hello";
		swap(s[ind], s[ind + 1]);
		a = helper(ind + 1, s, v, cnt + v[ind]);
		swap(s[ind], s[ind + 1]);
		int b = helper(ind + 1, s, v, cnt);
		cnt = max(a, b);
		return cnt;
	}
	else if (s[ind] == '1') {
		return helper(ind + 1, s, v, cnt + v[ind]);
	}
	else if (ind != v.size() - 1 and s[ind] == '0' && s[ind + 1] == '0')
		return helper(ind + 1, s, v, cnt);
	else
		return helper(ind + 1, s, v, cnt);
	return 1;
}
int main() {
	int t;
	cin >> t;
	while (t--) {
		int n;
		cin >> n;
		string s;
		cin >> s;
		vector<int>v(n);
		for (int i = 0; i < n; i++) cin >> v[i];
		if (n == 1) {
			if (s[0] == '1')
				cout << v[0];
			else cout << 0;
			cout << endl;
			continue;
		}
// 		cout << n << endl;
// 		cout << s << endl;
// 		for (auto x : v) cout << x << " ";
// 		cout << endl;
		cout << helper(0, s, v, 0);
		cout << "\n";
	}
}
