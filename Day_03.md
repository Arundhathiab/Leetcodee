# 📅 Day 03 – LeetCode Practice

---

## 🧩 Problem 1: Fizz Buzz
🔗 https://leetcode.com/problems/fizz-buzz/

### 💡 Approach:
- Iterate from 1 to n.
- If divisible by both 3 and 5 → append "FizzBuzz".
- If divisible by 3 → append "Fizz".
- If divisible by 5 → append "Buzz".
- Otherwise append the number as string.

### 💻 Code (Python)

```python
class Solution(object):
    def fizzBuzz(self, n):
        result = []
        for i in range(1, n + 1):
            if i % 3 == 0 and i % 5 == 0:
                result.append("FizzBuzz")
            elif i % 3 == 0:
                result.append("Fizz")
            elif i % 5 == 0:
                result.append("Buzz")
            else:
                result.append(str(i))
        return result
```

---

## 🧩 Problem 2: Smallest Even Multiple
🔗 https://leetcode.com/problems/smallest-even-multiple/

### 💡 Approach:
- If n is even → return n.
- If n is odd → return 2 * n.
- This works because answer = LCM(2, n).

### 💻 Code (Python)

```python
class Solution(object):
    def smallestEvenMultiple(self, n):
        if n % 2 == 0:
            return n
        return 2 * n
```

---

## 🧩 Problem 3: Convert the Temperature
🔗 https://leetcode.com/problems/convert-the-temperature/

### 💡 Approach:
- Convert Celsius to Kelvin using:
  Kelvin = Celsius + 273.15
- Convert Celsius to Fahrenheit using:
  Fahrenheit = Celsius * 1.80 + 32.00
- Return both values in a list.

### 💻 Code (Python)

```python
class Solution(object):
    def convertTemperature(self, celsius):
        kelvin = celsius + 273.15
        fahrenheit = celsius * 1.80 + 32.00
        return [kelvin, fahrenheit]
```

---

## 📊 Day 03 Summary:

- Problems Solved Today: 3
- Difficulty: Easy
- Language Used: Python
