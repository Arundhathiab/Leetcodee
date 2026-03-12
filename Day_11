# 📅 Day 11 – LeetCode Practice

---

## 🧩 Problem: Subtract the Product and Sum of Digits of an Integer
🔗 https://leetcode.com/problems/subtract-the-product-and-sum-of-digits-of-an-integer/

### 💡 Approach:
- Extract each digit using `n % 10`.
- Add the digit to `sum`.
- Multiply the digit to `product`.
- Remove the last digit using `n // 10`.
- After processing all digits, return `product - sum`.

### 💻 Code (Python)

```python
class Solution:
    def subtractProductAndSum(self, n: int) -> int:
        sum = 0
        product = 1
        
        while n > 0:
            d = n % 10
            sum += d
            product *= d
            n = n // 10
            
        return product - sum
```

---

## 📊 Day 11 Summary

- Problems Solved Today: 1
- Difficulty: Easy
- Language Used: Python
- Concepts Practiced:
  - Digit extraction
  - Arithmetic operations
  - Loop processing
