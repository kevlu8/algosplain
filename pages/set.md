<TAGS: searching, datastructures, sorted>

set<>

A self-sorting data structure that can only contain one of each kind of element.

THEORY:
- uses a red-black tree as the internal representation
- does not support random access (i.e. cannot do set[1] etc)
- has own finding operations (e.g. set.lower_bound(), set.upper_bound())


COMPLEXITY:
O(log n) find
O(log n) erase
O(log n) insert

CODE:
```
set<int> s; // {}
s.insert(1); // { 1 }
s.count(1); // true
s.erase(1); // {}
```

SEE ALSO:
- unordered_set
- binary search
- lower_bound
- upper_bound