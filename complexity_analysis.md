# Complexity Analysis

## 1. Max Heap

A Max Heap keeps the largest element at the root.

### Time Complexity

| Operation | Best Case | Average Case | Worst Case |
|---|---|---|---|
| Insertion | O(1) | O(log n) | O(log n) |
| Delete Maximum | O(log n) | O(log n) | O(log n) |
| Access Maximum | O(1) | O(1) | O(1) |

### Space Complexity

O(n)

---

## 2. Heap Sort

Heap Sort first builds a Max Heap and then repeatedly removes the maximum element.

### Time Complexity

| Case | Complexity |
|---|---|
| Best Case | O(n log n) |
| Average Case | O(n log n) |
| Worst Case | O(n log n) |

### Space Complexity

O(1) auxiliary space.

---

## 3. Quick Sort

Quick Sort selects a pivot and partitions the array around the pivot.

### Time Complexity

| Case | Complexity |
|---|---|
| Best Case | O(n log n) |
| Average Case | O(n log n) |
| Worst Case | O(n²) |

The worst case can occur when the pivot repeatedly produces very unbalanced partitions.

### Space Complexity

O(log n) average recursion space.

---

## 4. Comparison

| Feature | Max Heap | Heap Sort | Quick Sort |
|---|---|---|---|
| Main purpose | Priority Queue | Sorting | Sorting |
| Best Time | O(1) insertion | O(n log n) | O(n log n) |
| Average Time | O(log n) insertion | O(n log n) | O(n log n) |
| Worst Time | O(log n) insertion | O(n log n) | O(n²) |
| Highest element access | O(1) | O(1) after heap construction | O(n) if unsorted |
| Extra Space | O(n) | O(1) | O(log n) average |

---

## 5. Application to Hospital Priority Queue

The Max Heap is useful for a hospital priority queue because the patient with the highest severity score is maintained at the root.

For the given input:

45, 72, 30, 90, 65, 50, 85

the highest severity score is:

90

Therefore, the patient with severity score 90 has the highest priority.

## Conclusion

A Max Heap is appropriate for continuously managing patients according to severity because it allows the highest-priority patient to be accessed in O(1) time, while insertion and deletion of the maximum take O(log n) time.
