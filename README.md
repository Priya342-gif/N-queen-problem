# N-Queen Problem using Backtracking

## 📌 Problem Statement
The **N-Queen Problem** is a classic backtracking problem where the goal is to place **N queens** on an **N × N chessboard** such that **no two queens attack each other**.

A queen can attack another queen if they are placed on:
- The same row
- The same column
- The same diagonal

---

## 🧠 Approach: Backtracking

Backtracking is used to explore all possible arrangements of queens step by step and **undo (backtrack)** the placement when a conflict occurs.

### 🔹 Key Idea
- Place one queen in each column.
- For every column, try all rows.
- Check if placing a queen is **safe**.
- If safe → place the queen and move to the next column.
- If not safe → try the next row.
- If no row is valid → backtrack to the previous column.

---

## ✔️ Safety Check Conditions
A position `(row, col)` is safe if:
- No queen is present in the same row on the left side
- No queen is present on the upper-left diagonal
- No queen is present on the lower-left diagonal

---

## ⏱️ Time and Space Complexity
- **Time Complexity:** `O(N!)` (worst case)
- **Space Complexity:** `O(N²)` (for the chessboard)

---

## 🧪 Example (N = 4)

One valid solution:


. Q . .
. . . Q
Q . . .
. . Q .

