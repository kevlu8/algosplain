<TAGS: array, dynamic, dynamicarray>

vector<>

A C++ built in dynamic array data structure

THEORY:
- the array changes in size as you add more elements - there is no fixed size, as long as you have enough memory

CODE:
```
vector<int> v; // {}
v.push_back(3); // {3}
v.size(); // 1
v.pop_back(); // {}
```

SEE ALSO:
- binary search
- lower_bound
- upper_bound