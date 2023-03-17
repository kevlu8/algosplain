<TAGS: searching, finding, sorted>

Binary search

A way to quickly find an element in a sorted data structure. 
It is generally recommended to use binary search when you know that the input will be sorted, as built in find functions usually run a complete search (O(n))

THEORY:
- guess in the middle of the data structure
- if our desired element is less than the guess, guess in between the previous guess and 0
- if our desired element is greater than the guess, guess in between the previous guess and n

COMPLEXITY:
O(log n) time
O(1) space

CODE:
```
int a = 0, b = n - 1;
while (a <= b) {
	int k = (a + b) / 2;
	if (array[k] == x) {
		// we found the element
	}
	else if (array[k] > x) b = k - 1;
	else a = k + 1;
}
```

SEE ALSO:
- set
- complete search
- lower_bound
- upper_bound
- equal_range