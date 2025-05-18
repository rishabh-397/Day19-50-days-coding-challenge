# Day19-50-days-coding-challenge
## 🔹 Problem 1: Valid Parentheses

### Problem Statement:
Given a string `s` containing just `'('`, `')'`, `'{'`, `'}'`, `'['`, and `']'`, determine if the input string is **valid**.

### ✅ Validity Rules:
- Open brackets must be closed by the same type of brackets.
- Open brackets must be closed in the correct order.

### 💡 Approach:
- Use a stack.
- Push opening brackets onto the stack.
- For every closing bracket, check the top of the stack.
- If the match is correct, pop the stack; otherwise, return `false`.

### ✅ Examples:
```plaintext
Input: "()[]{}"    → Output: true  
Input: "(]"        → Output: false  
Input: "([])"      → Output: true

🔹 Problem 2: Best Time to Buy and Sell Stock
Problem Statement:
You're given an array prices where prices[i] is the stock price on the i-th day.
Return the maximum profit by choosing a day to buy and another to sell later.

✅ Constraints:
1 <= prices.length <= 10⁵

0 <= prices[i] <= 10⁴

💡 Approach:
Track the minimum price encountered so far.

For each price, calculate the profit if sold on that day.

Keep updating the max profit found.

✅ Examples:
Input: [7,1,5,3,6,4] → Output: 5  
(Buy at 1, Sell at 6)

Input: [7,6,4,3,1]   → Output: 0  
(No profitable trade)
