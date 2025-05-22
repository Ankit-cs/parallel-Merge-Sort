
🚀 Parallel Merge Sort in C++

This project implements Parallel Merge Sort using the multithreading capabilities of C++. It significantly improves sorting performance on large datasets by distributing tasks across multiple CPU cores.



 ✅ Features

* 🔀 Parallel Processing: Uses multiple threads to sort different parts of the array concurrently.
* 🧵 Thread Pool: Efficiently manages threads, reducing overhead and improving performance.
* 📊 Performance Benchmarking: Compares standard Merge Sort with Parallel Merge Sort.


 ⚙️ How It Works

 1. Recursive Division
The input array is recursively divided into halves until a base threshold (like 1,000 elements) is reached.

 2. Parallel Sorting

 The smaller subarrays are sorted in parallel using threads from the thread pool.

3. Efficient Merging
Sorted subarrays are merged back into a single sorted array using the traditional merge step.



🧵 Thread Pool Usage

 A thread pool is used to manage worker threads instead of creating new threads each time.
 This avoids the overhead of creating and destroying threads repeatedly.
 Threads are synchronized efficiently to avoid race conditions.


Performance Results

| Version             | Time Taken (WIndows) |
| ------------------- | --------------------------- |
| Standard Merge Sort | \~25 seconds                |
| Parallel Merge Sort | \~1 second                  |

> ✅ Result: 25x speedup with parallel processing.

C++ Compiler: Ensure you have a C++ compiler that supports C++11 or later.
CMake: Used for building the project.


 📦 Summary

This implementation showcases the power of multithreading in C++ to optimize one of the classic sorting algorithms—**Merge Sort**. By integrating parallelism and thread pooling, it delivers impressive performance on modern multi-core processors.

