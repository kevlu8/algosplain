<TAGS: functions, searching, finding>

find(*begin, *end, x)

A C++ built in function that returns a pointer to the first element whose value is equal to x. If no such element exists, *end is returned.

COMPLEXITY:
O(n) time

CODE:
```
vector<int> v = { 0, 1, 3, 5, 6, 4, 6, 8, 11, 9 };
find(v.begin(), v.end(), 5); // pointer to element 3 (5)
find(v.begin(), v.end(), 10); // pointer to v.end() as no element is equal to 1
```

SEE ALSO:
- binary search
- upper_bound
- equal_range