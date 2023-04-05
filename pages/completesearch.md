<TAGS: searching, finding, bruteforce>

Complete search

A way to find elements in a data structure by going through all of them.

THEORY:
- start at the beginning of the data structure
- iterate through elements until we find the desired element(s)

COMPLEXITY:
O(n) time

CODE:
```
int i;
for (i = 0; i < n; i++) {
	if (a[i] == 123) break;
}
cout << "123 found at " << i << '\n'
```

SEE ALSO:
- binary search
- find