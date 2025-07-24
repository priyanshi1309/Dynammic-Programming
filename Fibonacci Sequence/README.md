# 🧮 Fibonacci Sequence Pattern Problems

This folder contains solutions to problems that follow or are inspired by the **Fibonacci sequence**. These problems typically involve **recurrence relations**, **dynamic programming**, and often have optimal **space-optimized** solutions.

---

## 🧠 Problem Pattern

These problems are based on the classic recurrence relation:

T(n) = T(n - 1) + T(n - 2)

Where:
- `T(n)` is the solution for input size `n`
- The result depends on **two previous subproblems**

---

## 🧭 Base Conditions

T(0) = base case 1
T(1) = base case 2

yaml
Copy
Edit

These vary slightly depending on the problem (e.g., number of ways to climb 0 stairs might be 1).

---

## 📌 Key Characteristics

- Typically solved using:
  - **Recursion** (inefficient for large inputs)
  - **Memoization (Top-Down DP)**
  - **Tabulation (Bottom-Up DP)**
  - **Space Optimization** (O(1) space using two variables)

- Common themes:
  - Count total ways to reach an endpoint (e.g., stairs, paths)
  - Max/min cost or value with step-by-step decisions

---

