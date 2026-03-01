---

##  Problem 5: Three Divisors
🔗 https://leetcode.com/problems/three-divisors/

### 💡 Approach:
- Count the number of positive divisors of n.
- Loop from 1 to n//2.
- If n is divisible by i → increment count.
- If total divisors equal 3 → return True.
- Otherwise return False.

###  Code (Python)

```python
class Solution:
    def isThree(self, n: int) -> bool:
        count = 1
        m = n // 2 + 1
        
        for i in range(1, m):
            if n % i == 0:
                count += 1
                
        if count == 3:
            return True
        else:
            return False
```
##  Day 05 Summary:

- Problems Solved Today: 4
- Difficulty: Easy
- Language Used: Python
