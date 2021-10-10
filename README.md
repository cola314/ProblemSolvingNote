# ProblemSolvingNote
- 알고리즘을 다시 공부하면서 정리하는 노트입니다

## 템플릿
```c++
#define _CRT_SECURE_NO_WARNINGS
#include <bits/stdc++.h>
#define fastio cin.tie(NULL); cin.sync_with_stdio(false);
#define endl "\n"
#define FOR(x, y) for(int x = 0; x < y; x++)
#define pb push_back
#define all(x) x.begin(),x.end()
#define sz(x) ((int)x.size())
#define ini(x, y) memset(x, y, sizeof(x));
using namespace std;
using vi = vector<int>;
using ll = long long;
```

## 소수점 출력
```c++
cout << fixed << setprecision(3) << 3.141592;
```

## 문자열 split
```c++
vector<string> split(string s, char seperator) {
	vector<string> ret;
	stringstream ss(s);
	string out;
	while (getline(ss, out, seperator)) {
		ret.pb(out);
	}
	return ret;
}
```
