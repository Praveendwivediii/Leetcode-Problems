# [66. Plus One](https://leetcode.com/problems/plus-one/)

## 🧠 Problem Statement:  
You are given a **large integer** represented as an integer array `digits`, where each `digits[i]` is the `iᵗʰ` digit of the integer.  
The digits are ordered from **most significant to least significant**.  

Increment the large integer by **one** and return the resulting array of digits.  

---

## ✅ Solution Approach:  
- Start from the **last digit** of the array and add `1`.  
- If the digit becomes `10`, set it to `0` and carry `1` to the next digit on the left.  
- Continue propagating the carry until:
  - No carry remains, or  
  - All digits are processed.  
- If a carry still exists after processing all digits, insert `1` at the beginning of the array.  
- This approach runs in **O(n)** time with **O(1)** extra space (excluding output array).  
