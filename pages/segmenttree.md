<TAGS: tree, graphtheory, datastructures>

Segment tree

Data structure supporting fast range queries and updates

THEORY:
- construct a binary tree from an array
- left end of array used for tree nodes, right end for the actual array
- traverse up the tree when an element is updated

COMPLEXITY:
- O(log n) updates
- O(log n) queries

CODE:
```
struct SegTree {
	int size=1; // size of the array, to the next highest power of 2
	vector<int> a; // the internal representation of the tree

	void init(int n) {
		while (size < n) size *= 2;
		a.resize(2*size); // the first half is for the higher nodes of the tree, while the second half are the actual array elements
	}

	void update(int i, int v) {
		i += size;
		a[i] = v;
		while (i > 1) {
			i /= 2; // traverse up the tree
			a[i] = a[2*i] + a[2*i+1];
		}
	}

	int calculate(int i, int j) {
		i += size;
		j += size;
		int ans = 0;
		while (i <= j) {
			// try to find the largest range that fits in the desired range
			if (i % 2 == 1) ans += a[i++];
			if (j % 2 == 0) ans += a[j--];
			i /= 2;
			j /= 2;
		}
		return ans;
	}
};
```

SEE ALSO:
- sparse table
- lazy propagation
- sparse segment tree