# [1. Two Sum](https://leetcode.com/problems/two-sum/)

## 🧠 Problem Statement:  
Given an array of integers `nums` and an integer `target`, return the indices of the **two numbers** such that they add up to `target`.  
You may assume that each input would have **exactly one solution**, and you may not use the same element twice.  
Return the answer in any order.  

---

## ✅ Solution Approach:  
- We use a **brute-force approach** by checking all possible pairs of numbers.  
- For each element at index `i`, loop through the remaining elements (`j > i`) and check if `nums[i] + nums[j] == target`.  
- If a valid pair is found, return the indices `[i, j]`.  
- Since every pair is checked, the **time complexity is O(n²)** and **space complexity is O(1)**.  
