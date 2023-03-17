<TAGS: sorting>

Bubble sort

A simplistic sorting algorithm that is easy to implement, however it is slow.

DISCLAIMERS:
- it is highly discouraged to make a custom sorting implementation, as most languages have a built in sorting function

THEORY:
- n rounds are performed
- on each round, go through the array and if two adjacent elements are out of order, swap them
- if you count the number of swaps, you get the number of inversions

COMPLEXITY:
O(n^2) time
O(1) space

CODE:
```
for (int i = 0; i < n; i++) {
	for (int j = 0; j < n - 1; j++) {
		if (array[j] > array[j + 1]) {
			swap(array[j], array[j + 1])
		}
	}
}
```

SEE ALSO:
- inversions
- sorting