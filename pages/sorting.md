<TAGS: order>

Sorting

A way to convert a number of elements into a desired order

THEORY:
- there are many sorting algorithms that accomplish the same thing
- search up more specific sorting algorithms for an explanation of how they work
- we can sort just about any data structure that contains multiple elements - e.g. strings

COMPLEXITY:
O(n log n) time
O(1) space

CODE:
```
vector<int> v = { 1, 3, 2, 5, 4 };
// sort in increasing order
sort(v.begin(), v.end());
// sort in decreasing order
sort(v.rbegin(), v.rend());
// sort in a custom order
sort(v.begin(), v.end(), [](const int& a, const int& b) {
	return (a * 4) < (b * 3);
});
```

SEE ALSO:
- inversions