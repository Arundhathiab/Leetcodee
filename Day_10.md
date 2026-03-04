#  Day 10 – LeetCode Practice

---

##  Problem: Furthest Distance From Origin
🔗 https://leetcode.com/problems/furthest-distance-from-origin/

###  Approach:
- Count number of 'L', 'R', and '_' in the string.
- 'L' moves left, 'R' moves right.
- '_' can be used as either 'L' or 'R' to maximize distance.
- The maximum distance from origin is:

distance = abs(L - R) + number_of_underscores

###  Code (Python)

```python
class Solution:
    def furthestDistanceFromOrigin(self, moves: str) -> int:
        x = moves.count("L")
        y = moves.count("R")
        z = moves.count("_")
        return abs(x - y) + z
```

---

##  Day 10 Summary

- Problems Solved Today: 1
- Difficulty: Easy
- Language Used: Python
- Concepts Practiced:
  - String counting
  - Greedy thinking
