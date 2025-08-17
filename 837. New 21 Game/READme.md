# [837. New 21 Game](https://leetcode.com/problems/new-21-game/)

## 🧠 Problem Statement:  
Alice starts with `0` points and draws numbers while her total score is less than `K`.  
Each draw is an integer between `1` and `W` (inclusive), chosen uniformly at random.  
Alice stops drawing when she reaches at least `K` points.  

Return the probability that Alice’s final score is **at most `N`**.  

---

## ✅ Solution Approach:  
- This is a **Dynamic Programming (DP)** probability problem.  
- Define `dp[x]` = probability of reaching exactly `x` points.  
- Use the sliding window idea:
  - For each score `x < K`, we distribute its probability equally among the next `W` scores.  
  - Once `x >= K`, Alice stops and contributes to the final probability.  
- Finally, sum probabilities `dp[x]` for all `K ≤ x ≤ N`.  
