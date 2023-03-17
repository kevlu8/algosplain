<TAGS: searching, finding, datastructures, hashmap>

unordered_set<>

A data structure that stores elements in no particular order

THEORY:
- uses a hashmap to check if element is in set
- can only contain 1 of each kind of element

COMPLEXITY:
O(1) insert
O(1) find
O(1) erase

CODE:
```
unordered_set<int> s;
s.insert(1); { 1 }
s.insert(5); { 1, 5 } (could be in any order)
s.count(1); // true
s.count(2); // false
s.find(5); // pointer to 5
s.erase(1); // { 5 }
```

SEE ALSO:
- set