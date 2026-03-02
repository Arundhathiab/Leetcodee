#  Day 08 – LeetCode Practice

---

## Problem 1: Robot Return to Origin
🔗 https://leetcode.com/problems/robot-return-to-origin/

### Approach:
- Maintain two variables `x` and `y` for coordinates.
- For each move:
  - 'R' → x += 1
  - 'L' → x -= 1
  - 'U' → y += 1
  - 'D' → y -= 1
- After processing all moves:
  - If x == 0 and y == 0 → return True
  - Otherwise → return False

###  Code (Python)

```python
class Solution:
    def judgeCircle(self, moves: str) -> bool:
        x = 0
        y = 0
        
        for i in moves:
            if i == "R":
                x += 1
            elif i == "L":
                x -= 1
            elif i == "U":
                y += 1
            else:
                y -= 1
                
        return x == 0 and y == 0
```

---

## Problem 2: To Lower Case
🔗 https://leetcode.com/problems/to-lower-case/

###  Approach:
- Use built-in string method `.lower()`.
- Convert entire string to lowercase.
- Return the result.

### Code (Python)

```python
class Solution:
    def toLowerCase(self, s: str) -> str:
        return s.lower()
```

---

##  Day 08 Summary:

- Problems Solved Today: 2
- Difficulty: Easy
- Language-python
