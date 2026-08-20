# Python Data Structures and Algorithms (DSA) Notes

Implementations and complexity notes for core sorting algorithms and data structure practice problems in Python.

---

## 1. Sorting Algorithms

### Bubble Sort Implementation
```python
def bubble_sort(arr):
    n = len(arr)
    for i in range(n):
        swapped = False
        for j in range(0, n - i - 1):
            if arr[j] > arr[j + 1]:
                arr[j], arr[j + 1] = arr[j + 1], arr[j]
                swapped = True
        if not swapped:
            break
    return arr

# Test
sample_data = [64, 34, 25, 12, 22, 11, 90]
print("Sorted Array:", bubble_sort(sample_data))
```

- **Time Complexity**: $\mathcal{O}(N^2)$ worst-case, $\mathcal{O}(N)$ best-case (already sorted).
- **Space Complexity**: $\mathcal{O}(1)$ in-place auxiliary space.

---

## 2. Problem-Solving Patterns

- **Two Pointers Technique**: Used for searching pairs in sorted arrays or checking string palindromes.
- **Sliding Window**: Used for contiguous subarray or substring target optimization.
