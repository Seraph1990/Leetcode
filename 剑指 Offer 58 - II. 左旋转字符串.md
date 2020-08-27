1. 
```cpp
class Solution {
public:
    string reverseLeftWords(string s, int n) {
        reverse(s.begin(), s.end());
        reverse(s.begin(), s.end() - n);
        reverse(s.end() - n, s.end());
        return s;
    }
};
```

2
```cpp
class Solution {
public:
    string reverseLeftWords(string s, int n) {
        return (s+s).substr(n,s.size());
    }
};
```
