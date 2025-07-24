# 🎒 0/1 Knapsack Problems

This folder contains solutions to problems that follow the classic **0/1 Knapsack** pattern—where each item can be **either picked once or not at all**. These are fundamental **Dynamic Programming** problems involving optimization under constraints.

---

## 🧠 Problem Pattern

The core idea is:
T(i, w) = max(
T(i - 1, w), // Exclude the current item
T(i - 1, w - weight[i]) + value[i] // Include the current item (if it fits)
)
- `i` = index of the current item
- `w` = remaining weight/capacity
- `T(i, w)` = maximum value achievable using first `i` items with capacity `w`

---

## 🧭 Base Conditions

T(0, w) = 0 // No items to pick
T(i, 0) = 0 // Zero capacity means no item can be included

---

## 📌 Key Concepts

- **Each item can be picked at most once**.
- **Optimal substructure**: The solution to the problem can be built from solutions to smaller subproblems.
- **Overlapping subproblems**: The same subproblems are solved multiple times → perfect for **memoization** or **tabulation**.

---
