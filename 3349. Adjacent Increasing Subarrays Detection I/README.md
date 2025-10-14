# [3349. Adjacent Increasing Subarrays Detection I](https://leetcode.com/problems/adjacent-increasing-subarrays-detection-i/)

## 🧠 Problem Statement:  
You are given an integer array `nums` and an integer `k`.  
Your task is to determine whether there exist **two adjacent subarrays** of length `k` such that both are **strictly increasing**.  

Return `true` if such subarrays exist, otherwise return `false`.  

---

## ✅ Solution Approach:  
- We need to check **every window of size `2k`** to see if both halves (each of length `k`) are strictly increasing.  
- For each possible starting index:
  - Verify the first subarray (`nums[i : i + k - 1]`) is strictly increasing.  
  - Verify the next subarray (`nums[i + k : i + 2k - 1]`) is also strictly increasing.  
- If both conditions hold for any index, return `true`.  
- If no such pair exists, return `false`.  
- This approach takes **O(n × k)** time with **O(1)** extra space.  
