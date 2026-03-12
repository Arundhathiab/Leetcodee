# 📅 Day 12 – LeetCode Practice

---

## 🧩 Problem: Difference Between Element Sum and Digit Sum of an Array
🔗 https://leetcode.com/problems/difference-between-element-sum-and-digit-sum-of-an-array/

### 💡 Approach:
- Calculate **element sum** using `sum(nums)`.
- Calculate **digit sum** by:
  - Converting each number to a string.
  - Extracting each digit.
  - Converting it back to an integer and summing.
- Return the **absolute difference** between element sum and digit sum.

### 💻 Code (Python)

```python
class Solution:
    def differenceOfSum(self, nums: List[int]) -> int:
        
        element_sum = sum(nums)
        digit_sum = sum(int(d) for num in nums for d in str(num))
        
        return abs(element_sum - digit_sum)
```

---

## 📊 Day 12 Summary

- Problems Solved Today: 1
- Difficulty: Easy
- Language Used: Python
- Concepts Practiced:
  - List comprehension
  - Digit extraction
  - Built-in functions (`sum`, `abs`)
