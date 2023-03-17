<TAGS: segmenttree>

Lazy Propagation

A way to support fast range updates in a segment tree

THEORY:
- instead of looping through the range, we add a "lazy" variable to each node
- add the update to the lazy variable in the highest possible nodes
- when the node needs to be queried, only then do we update the tree in log(n) time

COMPLEXITY:
O(log n) time
O(n) space

SEE ALSO:
- segment tree