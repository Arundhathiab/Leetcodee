# 📅 Day 13 – LeetCode Practice

---

## 🧩 Problem: Count Integers With Even Digit Sum
🔗 https://leetcode.com/problems/count-integers-with-even-digit-sum/

### 💡 Approach:
- Loop from `1` to `num`.
- For each number:
  - Calculate the **digit sum** using `% 10` and `// 10`.
- If the digit sum is **even**, increment the count.
- Return the total count.

### 💻 Code (Python)

```python
class Solution:
    def countEven(self, num: int) -> int:
        
        count = 0
        
        for i in range(1, num + 1):
            digit_sum = 0
            temp = i
            
            while temp > 0:
                digit_sum += temp % 10
                temp //= 10
                
            if digit_sum % 2 == 0:
                count += 1
                
        return count
```

---

## 📊 Day 13 Summary

- Problems Solved Today: 1
- Difficulty: Easy
- Language Used: Python
- Concepts Practiced:
  - Digit extraction
  - Loop iteration
  - Even/Odd checking
