# 📅 Day 09 – LeetCode Practice

---

## 🧩 Problem: Palindrome Number
🔗 https://leetcode.com/problems/palindrome-number/

### 💡 Approach:
- Store the original number.
- Reverse the digits of the number using a loop.
- Extract last digit using `x % 10`.
- Build reversed number using `rev = rev * 10 + digit`.
- Remove last digit using `x // 10`.
- Compare reversed number with the original number.

### 💻 Code (Python)

```python
class Solution:
    def isPalindrome(self, x: int) -> bool:
        orgi = x
        rev = 0
        
        while x > 0:
            d = x % 10
            rev = rev * 10 + d
            x = x // 10
        
        return orgi == rev
```

---

## 📊 Day 09 Summary:

- Problems Solved Today: 1
- Difficulty: Easy
- Language Used: Python
- Concepts Practiced:
  - Number reversal
  - Modulo and integer division
