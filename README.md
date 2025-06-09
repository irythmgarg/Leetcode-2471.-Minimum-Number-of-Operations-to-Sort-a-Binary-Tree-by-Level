# Leetcode-2471.-Minimum-Number-of-Operations-to-Sort-a-Binary-Tree-by-Level
# 🌲 Minimum Operations to Make the Binary Tree Level-wise Sorted

## 🧩 Problem Statement

Given the root of a binary tree, determine the **minimum number of operations** needed to sort the values at each level of the tree in ascending order. Each operation consists of swapping any two values at the same level.

---

## 🧠 Approach Explanation

### 🔁 Level Order Traversal

* Perform a **BFS traversal** to get the nodes at each level.
* Store the values of nodes in a vector `vec` for each level.

### 🔄 Minimum Swaps to Sort

* For each level vector `vec`, calculate the **minimum number of swaps** needed to sort it.
* This is done using a **value-to-index map** and simulating the sorting process by placing each element at its correct position via swaps.

### 🔧 Core Functions

* `countMinSwapsToSort`: Finds the minimum number of swaps required to sort an array.
* `minimumOperations`: Applies BFS and sums swaps needed for each level.

---

## ⏱️ Time Complexity

* **O(N log N)** overall where N is the total number of nodes.
* Sorting each level takes O(K log K), and each level is processed once.

## 💾 Space Complexity

* **O(N)** for queues, vectors, and maps used in BFS and sorting simulation.

---

## 📌 Example

```cpp
Input: [1,4,3,7,6,8,5,null,null,null,null,null,9,null,null]
Output: 3
Explanation:
- Level 0: [1] — Already sorted
- Level 1: [4, 3] — 1 swap needed
- Level 2: [7, 6, 8, 5] — 2 swaps needed
Total = 3 operations
```

---

## 📂 File Overview

* `MinimumOperations.cpp` – Contains the full solution with helper function.

---

## 👨‍💻 Author

**Ridham Garg**

> Made with 💡 and ☕ by Ridham Garg.

---

## 🚀 Happy Coding!
