<TAGS: searching, finding, sorted>

upper_bound(*begin, *end, x)

A C++ built in function that returns a pointer to the first element whose value is greater than x

COMPLEXITY:
O(log n) time
O(1) space

CODE:
```
vector<int> v = { 0, 1, 3, 4, 6, 6, 8, 9 };
upper_bound(v.begin(), v.end(), 4); // pointer to element 4 (6)
upper_bound(v.begin(), v.end(), 10); // pointer to v.end() as no element greater than 10 exists
```

SEE ALSO:
- binary search
- lower_bound
- equal_range