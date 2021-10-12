# ProblemSolvingNote
- 알고리즘을 다시 공부하면서 정리하는 노트입니다

## 템플릿
```c++
#define _CRT_SECURE_NO_WARNINGS
#define _USE_MATH_DEFINES
#include <bits/stdc++.h>
#define fastio cin.tie(NULL); cin.sync_with_stdio(false);
#define endl "\n"
#define FOR(x, y) for(int x = 0; x < y; x++)
#define pb push_back
#define all(x) x.begin(),x.end()
#define sz(x) ((int)x.size())
#define ini(x, y) memset(x, y, sizeof(x));
#define INF 987654321
#define y1 omg
#define fi first
#define se second
#define mp make_pair
#define ceildv(x, y) ((x) / (y) + ((x) % (y) != 0))
#define sumn(x) ((x) * ((x) + 1) / 2)
#define square(x) ((x) * (x))
#define int ll
using namespace std;
using ll = long long;
using vi = vector<int>;
using ii = pair<int, int>;
using iii = pair<pair<int, int>, int>;
using vii = vector<ii>;
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
## 에라토스테네스의 체
```c++
const int MAX = 1'000'000 + 10;
int prime[MAX];

FOR(i, MAX) prime[i] = 1;
prime[1] = 0;
for (ll i = 2; i < MAX; i++) if (prime[i]) {
	for (ll j = i * i; j < MAX; j += i) {
		prime[j] = 0;
	}
}
```
