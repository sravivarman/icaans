---
title: Data Structures - Introduction to Arrays
published: 2026-02-01
description: 'Fundamental concepts of arrays, their implementation, and common operations'
tags: [Arrays, Data Structures, CS Fundamentals]
category: Computer Science
draft: false
---

# Data Structures - Introduction to Arrays

Arrays are one of the most fundamental data structures in computer science. They provide a way to store multiple elements of the same type in a contiguous block of memory.

## What is an Array?

An array is a collection of elements (values or variables), each identified by at least one array index or key. Arrays are stored in contiguous memory locations, which makes them efficient for accessing elements by index.

### Key Characteristics:
- **Fixed size**: In most programming languages, arrays have a fixed size that's determined at creation time
- **Homogeneous**: All elements in an array are of the same data type
- **Indexed**: Elements can be accessed using indices (typically starting from 0)
- **Contiguous memory**: Elements are stored in consecutive memory locations

## Array Operations

### 1. Access/Read
Accessing an element in an array is a constant time operation O(1).

```python
arr = [1, 2, 3, 4, 5]
element = arr[2]  # Returns 3
```

### 2. Insert
- At the beginning: O(n) - requires shifting all elements
- At the end: O(1) if space is available
- At arbitrary position: O(n) - requires shifting elements

```python
# Insert at beginning
arr.insert(0, 10)  # [10, 1, 2, 3, 4, 5]

# Insert at end
arr.append(6)      # [10, 1, 2, 3, 4, 5, 6]

# Insert at position
arr.insert(3, 15)  # [10, 1, 2, 15, 3, 4, 5, 6]
```

### 3. Delete
Similar to insertion, deletion complexity depends on the position:

```python
# Delete by index
del arr[2]         # Removes element at index 2

# Delete by value
arr.remove(15)     # Removes first occurrence of 15
```

## Time Complexity Summary

| Operation | Time Complexity |
|-----------|----------------|
| Access    | O(1)          |
| Search    | O(n)          |
| Insertion | O(1) to O(n)  |
| Deletion  | O(1) to O(n)  |

## Advantages and Disadvantages

### Advantages:
- Fast access to elements by index
- Memory efficient - no extra memory needed for pointers
- Cache friendly due to locality of reference
- Simple to use and understand

### Disadvantages:
- Fixed size in many implementations
- Insertion and deletion can be expensive
- Memory allocation must be contiguous

## Common Applications

1. **Storing sequential data**: Lists, queues, stacks
2. **Mathematical computations**: Matrices, vectors
3. **Implementing other data structures**: Hash tables, heaps
4. **Algorithm implementations**: Sorting, searching

## Practice Problems

Try implementing these array operations:
1. Find the maximum element in an array
2. Reverse an array in-place
3. Remove duplicates from a sorted array
4. Merge two sorted arrays

## Next Topics

In our next lesson, we'll explore:
- Dynamic arrays (vectors in C++, lists in Python)
- Multi-dimensional arrays
- Array-based algorithms like binary search

---

*This is part of the Computer Science course series. For more data structure topics, check out the full course syllabus.*