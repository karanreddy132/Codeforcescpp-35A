# Codeforcescpp-35A
#include <bits/stdc++.h>

using namespace std;

int main() {
	freopen("input.txt", "r", stdin);
	freopen("output.txt", "w", stdout);

	int n, a, b, tmp;
	cin >> n;
	tmp = n;
	for (int i = 0; i < 3; i++) {
		cin >> a >> b;
		if (a == tmp)
			tmp = b;
		else if (b == tmp)
			tmp = a;
	}
	cout << tmp;
	return 0;
}
