# Reverse String


## Question

Write a function that takes a string as input and returns the string reversed.

**Example:**
Given s = "hello", return "olleh".



## Solution  



### C++

```c++
class Solution {
public:
    
    string reverseString(string s) {
        
        int left = 0;
        int right = s.size() - 1;
        
        while (left < right) {
            
            char t = s[left];
            s[left++] = s[right];
            s[right--] = t;
        }
        return s;
    }
};
```

