<TAGS: searching, finding, sorted>

equal_range(*begin, *end, x)

A C++ built in function that returns a pair containing both the lower_bound (first) and upper_bound (second)

COMPLEXITY:
O(log n) time
O(1) space

CODE:
```
vector<int> v = { 0, 1, 3, 4, 6, 6, 8, 9 };
auto a = equal_range(v.begin(), v.end(), 6); // {pointer to element 4, pointer to element 6}
cout << a.second - a.first << "\n"; // prints the number of elements whose value is 6
```

SEE ALSO:
- binary search
- lower_bound
- upper_bound