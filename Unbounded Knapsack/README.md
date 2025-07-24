# ♾️ Unbounded Knapsack Problems

This folder contains solutions to problems that follow the **Unbounded Knapsack** pattern — where **you can use each item multiple times**. These problems are common in **dynamic programming**, especially when dealing with combinations, partitions, or coin-related questions.

---

## 🧠 Problem Pattern

The recurrence relation for Unbounded Knapsack is:

T(i, w) = max(
T(i - 1, w), // Exclude the current item
T(i, w - weight[i]) + value[i] // Include the item again
)

Key difference from 0/1 Knapsack:
- Instead of `T(i - 1, w - weight[i])`, we **stay on the same item** when we include it (`T(i, ...)`), because the item can be reused.

---

## 🧭 Base Conditions

T(0, w) = 0 // No items available
T(i, 0) = 0 // Zero capacity → no value

yaml
Copy
Edit

---

## 📌 Key Concepts

- Items can be chosen **unlimited number of times**.
- Used in problems involving:
  - **Combinations** (e.g., coin denominations)
  - **Rod cutting**
  - **Ways to achieve a total using repeatable elements**
- Often requires **nested loops** or **1D DP optimization**.

---
