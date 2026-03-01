#  Day 06 – LeetCode Practice

---

##  Problem 1: Number of Common Factors
 https://leetcode.com/problems/number-of-common-factors/

###  Approach:
- Find the minimum of a and b.
- Iterate from 1 to min(a, b).
- Count numbers that divide both a and b.
- Return the count.

###  Code (Python)

```python
class Solution:
    def commonFactors(self, a: int, b: int) -> int:
        mini = min(a, b)
        cnt = 0
        
        for i in range(1, mini + 1):
            if a % i == 0 and b % i == 0:
                cnt += 1
                
        return cnt
```

---

##  Problem 2: Find Greatest Common Divisor of Array
🔗 https://leetcode.com/problems/find-greatest-common-divisor-of-array/

###  Approach:
- Find smallest and largest number in array.
- Use built-in `math.gcd()` to compute GCD.
- Return the result.

###  Code (Python)

```python
import math

class Solution:
    def findGCD(self, nums):
        return math.gcd(max(nums), min(nums))
```

---

##  Problem 3: Defanging an IP Address
🔗 https://leetcode.com/problems/defanging-an-ip-address/

###  Approach:
- Traverse each character in the string.
- If digit → append as it is.
- If '.' → replace with "[.]".
- Join and return final string.

### 💻 Code (Python)

```python
class Solution:
    def defangIPaddr(self, address: str) -> str:
        ans = []
        for ch in address:
            if ch.isdigit():
                ans.append(ch)
            else:
                ans.append("[.]")
        return "".join(ans)
```

---

##  Day 06 Summary:

- Problems Solved Today: 3
- Difficulty: Easy
- Language Used: Python
- Concepts Practiced:
  - Factor counting
  - GCD
  - String manipulation
