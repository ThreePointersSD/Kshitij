# 📘 Day 1 – Arrays: Foundations & Traversal  

## 🎯 Goal  
Understand how arrays are stored in memory, basic syntax, and how to traverse (iterate through) them.

---

## 🧠 Part 1 – Foundations (60–75 mins)

### 📌 Theory

- **What is an Array?**  
  An array is a collection of elements of the same data type stored in contiguous memory locations.  
  It allows storing multiple values under a single variable name.

- **Why Use Arrays Instead of Individual Variables?**  
  - Avoids creating multiple variables (`a1, a2, a3...`)  
  - Makes data easier to manage  
  - Enables looping and bulk operations  
  - Improves code readability and efficiency  

- **Indexing (0-Based vs 1-Based)**  
  - Most programming languages (C, C++, Java, Python) use **0-based indexing**.  
  - First element → index `0`  
  - Last element → index `N-1`  

- **Memory Layout (Contiguous Storage)**  
  - Array elements are stored next to each other in memory.  
  - Example:  
    If `arr[0]` is stored at address `1000`,  
    `arr[1]` will be at `1004` (for `int`, assuming 4 bytes).  
  - This allows fast access using index calculation.

---

## 💻 Part 2 – Basic Array Practice (60–75 mins)

### ✅ Tasks

- **Declare an Array**
  ```c
  int arr[5];
  ```

- **Take User Input & Print Elements**
  ```c
  for(int i = 0; i < 5; i++) {
      scanf("%d", &arr[i]);
  }

  for(int i = 0; i < 5; i++) {
      printf("%d ", arr[i]);
  }
  ```

- **Access Specific Element by Index**
  ```c
  printf("%d", arr[4]);  // Access 5th element
  ```

---

## 🔁 Part 3 – Traversing Arrays (45–60 mins)

### 📌 Concepts

- **Looping Structures**
  - `for` loop → Best when number of iterations is known.
  - `while` loop → Useful when iterations depend on a condition.

- **Forward Traversal**
  ```
  0 → N-1
  ```

- **Reverse Traversal**
  ```
  N-1 → 0
  ```

---

## 💻 Traversal Practice (75–90 mins)

### ✅ Tasks

- **Print All Elements (New Line Format)**
  ```c
  for(int i = 0; i < 5; i++) {
      printf("%d\n", arr[i]);
  }
  ```

- **Print Elements in Reverse Order**
  ```c
  for(int i = 4; i >= 0; i--) {
      printf("%d ", arr[i]);
  }
  ```

- **Count Total Number of Elements**
  ```c
  int size = sizeof(arr) / sizeof(arr[0]);
  printf("Total elements: %d", size);
  ```

---

## ⏱ Estimated Total Time  
🕒 3–4 Hours  

---

## 🚀 Outcome After Day 1

By the end of this day, you should be able to:

- Define and declare arrays confidently  
- Understand memory behavior of arrays  
- Access elements using indexing  
- Traverse arrays forward and backward  
- Perform basic input/output operations  
