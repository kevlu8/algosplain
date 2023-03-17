<TAGS: searching, finding, sorted>

lower_bound(*begin, *end, x)

A C++ built in function that returns a pointer to the first element whose value is at least x

COMPLEXITY:
O(log n) time
O(1) space

CODE:
```
vector<int> v = { 0, 1, 3, 5, 6, 6, 8, 9 };
lower_bound(v.begin(), v.end(), 4); // pointer to element 3 (5)
lower_bound(v.begin(), v.end(), 10); // pointer to v.end() as no element equal to or greater than 10 exists
```

SEE ALSO:
- binary search
- upper_bound
- equal_range