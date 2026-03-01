# Day 07 – LeetCode Practice

---

##  Problem 1: Two Sum
🔗 https://leetcode.com/problems/two-sum/

###  Approach (Brute Force):
- Use two nested loops.
- Check every pair of elements.
- If their sum equals target → return indices.
- Time Complexity: O(n²)

###  Code (Python)

```python
class Solution:
    def twoSum(self, nums, target):
        for i in range(len(nums)):
            for j in range(i + 1, len(nums)):
                if nums[i] + nums[j] == target:
                    return [i, j]
```

---

###  Better Approach (Optimal – O(n))
- Use a dictionary (hash map).
- Store number and its index.
- For each number, check if (target - number) exists.
- Time Complexity: O(n)

```python
class Solution:
    def twoSum(self, nums, target):
        seen = {}
        for i, num in enumerate(nums):
            complement = target - num
            if complement in seen:
                return [seen[complement], i]
            seen[num] = i
```

---

##  Problem 2: Minimum Number Game
🔗 https://leetcode.com/problems/minimum-number-game/

###  Approach:
- Sort the array.
- Remove two smallest elements each round.
- First append Bob’s number, then Alice’s.
- Continue until array is empty.

### 💻 Code (Python)

```python
class Solution:
    def numberGame(self, nums):
        ans = []
        nums.sort()
        
        while nums:
            alice = nums.pop(0)
            bob = nums.pop(0)
            ans.append(bob)
            ans.append(alice)
            
        return ans
```

---

##  Day 07 Summary:

- Problems Solved Today: 2
- Difficulty: Easy
- Language Used: Python
