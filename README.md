# java-dsa-roadmap
.

📘 Bubble Sort in Java – DSA Practice
📌 Overview

This repository contains my implementation and practice problems on Bubble Sort using Java.
The goal of this module is to build strong fundamentals in sorting algorithms and improve problem-solving skills using DSA.

Bubble Sort is a simple comparison-based sorting algorithm where adjacent elements are repeatedly compared and swapped if they are in the wrong order.

🧠 What is Bubble Sort?

Bubble Sort works by repeatedly stepping through the list, comparing adjacent elements, and swapping them if they are in the wrong order.
After each pass, the largest element moves to the end, just like a bubble rising to the surface.

⚙️ Algorithm Steps

Traverse the array from index 0 to n-2

Compare arr[j] and arr[j+1]

Swap if arr[j] > arr[j+1]

After each pass, the last element is fixed

Repeat for n-1 passes or stop early if no swaps occur

💻 Java Implementation
public static void bubbleSort(int[] arr) {
    int n = arr.length;

    for (int i = 0; i < n - 1; i++) {
        boolean swapped = false;

        for (int j = 0; j < n - 1 - i; j++) {
            if (arr[j] > arr[j + 1]) {
                int temp = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = temp;
                swapped = true;
            }
        }

        if (!swapped) break;
    }
}

⏱️ Time and Space Complexity
Case	Complexity
Best Case	O(n)
Average Case	O(n²)
Worst Case	O(n²)
Space	O(1) (In-place)
✅ Features Implemented

Ascending order bubble sort

Optimized version using swap flag

In-place sorting

Beginner-friendly implementation

🎯 Practice Problems Covered

Sort array in ascending order

Sort array in descending order

Count number of swaps

Stop early if array already sorted

Find k-th largest element

🚀 Learning Outcomes

Understood how comparison-based sorting works

Improved loop control and swapping logic

Learned time complexity analysis

Built foundation for advanced sorting algorithms

🛠️ Tech Stack

Language: Java

IDE: IntelliJ IDEA / VS Code

Concepts: Arrays, loops, conditionals, optimization

📂 Folder Structure
/bubble-sort
   ├── BubbleSortEasy.java
   ├── BubbleSortDescending.java
   ├── BubbleSortSwapCount.java
   └── README.md

📈 Progress

✔ Arrays
✔ Bubble Sort
⬜ Selection Sort
⬜ Insertion Sort
⬜ Merge Sort
⬜ Quick Sort

✍️ Author

Akansh Kumar
B.Tech CSE | Java Backend & DSA
