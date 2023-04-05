<TAGS: segmenttree>

Sparse segment tree

A variation on a segment tree that uses much less memory when most of the elements are going to be 0

THEORY:
- only construct nodes that we are going to actually use (nonzero)
- use a struct to represent nodes

COMPLEXITY:
O(log n) time
O(n) space

SEE ALSO:
- lazy propagation
- segment tree