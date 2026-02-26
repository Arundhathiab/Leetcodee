# Day 04 – LeetCode Practice

---

##  Problem 1: Ant on the Boundary
🔗 https://leetcode.com/problems/ant-on-the-boundary/

### 💡 Approach:
- Maintain a variable `current_pos = 0`.
- Traverse through nums.
- Add each value to current_pos.
- Whenever current_pos becomes 0 → increment boundary_count.
- Return boundary_count.

### 💻 Code (Python)

```python
class Solution(object):
    def returnToBoundaryCount(self, nums):
        current_pos = 0
        boundary_count = 0
        
        for num in nums:
            current_pos += num
            if current_pos == 0:
                boundary_count += 1
                
        return boundary_count
```

---

##  Problem 2: Average Value of Even Numbers Divisible by 3
🔗 https://leetcode.com/problems/average-value-of-even-numbers-that-are-divisible-by-three/

### 💡 Approach:
- Traverse the array.
- A number divisible by both 2 and 3 is divisible by 6.
- Collect numbers where `i % 6 == 0`.
- If none found → return 0.
- Otherwise return floor(sum / count).

###  Code (Python)

```python
class Solution(object):
    def averageValue(self, nums):
        res = []
        for i in nums:
            if i % 6 == 0:
                res.append(i)
                
        if len(res) == 0:
            return 0
        
        return sum(res) // len(res)
```

---

##  Problem 3: Maximum Nesting Depth of Parentheses
🔗 https://leetcode.com/problems/maximum-nesting-depth-of-the-parentheses/

### 💡 Approach:
- Use a counter to track current depth.
- Increment when '(' is found.
- Decrement when ')' is found.
- Track maximum depth reached.
- Return the maximum depth.

### 💻 Code (Python)

```python
class Solution(object):
    def maxDepth(self, s):
        count = 0
        maxcnt = 0
        
        for i in s:
            if i == '(':
                count += 1
                if count > maxcnt:
                    maxcnt = count
            if i == ')':
                count -= 1
                
        return maxcnt
```

---

##  Day 04 Summary:

- Problems Solved Today: 3
- Difficulty: Easy
- Language Used: Python

