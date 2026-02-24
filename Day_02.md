# 📅 Day 02 – LeetCode Practice

## 🧩 Problem: Concatenation of Array
🔗 https://leetcode.com/problems/concatenation-of-array/

---

## 💡 Approach:
- Create a new array of size 2 * n.
- Copy original array elements into first half.
- Copy same elements again into second half.
- Return the new array.

---

## 💻 Code (Java)

```java
class Solution {
    public int[] getConcatenation(int[] nums) {
        int n = nums.length;
        int[] result = new int[2 * n];

        for(int i = 0; i < n; i++) {
            result[i] = nums[i];
            result[i + n] = nums[i];
        }

        return result;
    }
}
```

---

## 📊 Progress:

- Problems Solved Today: 1
- Total Problems Solved: 2
- Difficulty: Easy
- Language Used: Java
- Time Taken: __ minutes
