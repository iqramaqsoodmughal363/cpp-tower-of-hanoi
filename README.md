# 🗼 Tower of Hanoi in C++

> A C++ program solving the **Tower of Hanoi** problem using recursion, moving disks from source to destination with an auxiliary peg.

---

## 📋 Overview

The **Tower of Hanoi** is a classic recursion problem involving three pegs and a set of disks of different sizes. The goal is to move all disks from the source peg to the destination peg, following these rules:

1. Only one disk can be moved at a time.
2. A disk can only be placed on a larger disk.
3. The auxiliary peg is used as a temporary storage.

**Key Concepts:**
- **Recursion:** The problem is broken into smaller subproblems.
- **Divide and Conquer:** Move n-1 disks to auxiliary, move the largest disk, then move n-1 disks to destination.
- **Base Case:** When only one disk remains, move it directly.

---

## ✨ Features

- ✅ Recursive solution to the Tower of Hanoi problem
- ✅ Clear step-by-step output showing disk movements
- ✅ Uses characters for peg labels ('A', 'B', 'C')
- ✅ Handles any number of disks (tested with n = 3)
- ✅ Clean and modular implementation
- ✅ Beginner-friendly with proper comments

---

## ⏱️ Complexity Analysis

| Measure | Value |
| :---: | :--- |
| **Time Complexity** | O(2ⁿ) – Exponential, as each disk requires two recursive calls. |
| **Space Complexity** | O(n) – Recursion stack uses n frames. |

> **Note:** The number of moves required is exactly `2ⁿ - 1` for `n` disks.

---

## 💻 Sample Input / Output

**Input:**
n = 3
Source: A, Auxiliary: B, Destination: C


**Output:**
Move disk 1 from A to C
Move disk 2 from A to B
Move disk 1 from C to B
Move disk 3 from A to C
Move disk 1 from B to A
Move disk 2 from B to C
Move disk 1 from A to C



---

## 🧮 Program Logic & Execution Flow

### 1. **`towerOfHanoi(n, src, aux, dest)`**
- **Base Case:** If `n == 1`, move disk 1 from `src` to `dest`.
- **Recursive Step:**
  1. Move `n-1` disks from `src` to `aux` (using `dest` as auxiliary).
  2. Move disk `n` from `src` to `dest`.
  3. Move `n-1` disks from `aux` to `dest` (using `src` as auxiliary).

### 2. **`main()`**
- Sets `n = 3` and calls `towerOfHanoi(3, 'A', 'B', 'C')`.

---

## 🛠️ How to Compile and Run (Windows & Linux)

### 🪟 For Windows Users
| Step | Command |
| :---: | :--- |
| **1. Compile** | `g++ -std=c++11 tower_of_hanoi.cpp -o tower_of_hanoi.exe` |
| **2. Run** | `tower_of_hanoi.exe` |

### 🐧 For Linux / macOS Users
| Step | Command |
| :---: | :--- |
| **1. Compile** | `g++ -std=c++11 tower_of_hanoi.cpp -o tower_of_hanoi` |
| **2. Run** | `./tower_of_hanoi` |

---

## 📂 Project Structure
cpp-tower-of-hanoi/
│
├── tower_of_hanoi.cpp # Main source code file
└── README.md # Project documentation (this file)



---

## 🔍 Real-World Applications

- **Educational Tool:** Teaching recursion and problem-solving.
- **Algorithm Design:** Understanding divide-and-conquer strategies.
- **Optimization Problems:** Disk movement optimization.
- **AI and Planning:** Similar to planning problems in artificial intelligence.
- **Game Theory:** Insights into problem-solving and strategy.

---

## 🧠 Key Learnings

- **Recursion:** Breaking a problem into smaller subproblems.
- **Base Case:** Essential to stop recursion.
- **Exponential Complexity:** 2ⁿ - 1 moves are required for n disks.
- **Divide and Conquer:** The largest disk is moved only once.
- **Auxiliary Peg:** Used as temporary storage for intermediate steps.

---

## 🔧 Potential Enhancements

- **User Input:** Allow the user to enter the number of disks.
- **Visualization:** Add a visual representation of the pegs and disks.
- **Iterative Solution:** Implement an iterative version using a stack.
- **Move Counter:** Track and display the total number of moves.
- **Generic Peg Labels:** Use any characters for peg labels.

---

## 👩‍💻 Author

**Iqra Maqsood Mughal**  
*C++ Developer | Programming Enthusiast*

---

## 📅 Date

**August 6, 2026**

---

## 📄 License

This project is open-source and intended for educational purposes.
