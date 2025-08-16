# [1323. Maximum 69 Number](https://leetcode.com/problems/maximum-69-number/)

## 🧠 Problem Statement:  
You are given a positive integer `num` consisting only of digits `6` and `9`.  
You may **change at most one digit (6 → 9 or 9 → 6)** to get the maximum possible number.  
Return the maximum number you can obtain.  

---

## ✅ Solution Approach:  
- Since we want the largest number possible, we should change the **first occurrence of digit `6`** to `9`.  
- If no `6` is found, the number is already the maximum.  
- Steps:  
  1. Convert the number to a string.  
  2. Replace the first `6` with `9`.  
  3. Convert back to integer.  
