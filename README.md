# DSA Assignment - Question 1

## Topic
Hospital Priority Queue using Max Heap, Heap Sort and Quick Sort.

## Input
45, 72, 30, 90, 65, 50, 85

## Final Max Heap

90 72 85 45 65 30 50

## Heap Sort Result

30 45 50 65 72 85 90

## Quick Sort Result

30 45 50 65 72 85 90

## Highest Priority

The highest severity score is **90**.

## Files

- `question1.c` - C source code
- `input.txt` - Input values
- `output.txt` - Program output
- `complexity_analysis.md` - Complexity analysis and comparison

## Conclusion

A Max Heap is useful for a hospital priority queue because the highest-severity patient is maintained at the root. The maximum element can be accessed in O(1) time, while insertion and deletion take O(log n) time.
## Comparison

| Feature | Max Heap / Heap Sort | Quick Sort |
|---|---|---|
| Best Time | O(n log n) | O(n log n) |
| Average Time | O(n log n) | O(n log n) |
| Worst Time | O(n log n) | O(n²) |
| Space | O(1) for Heap Sort | O(log n) average |
| Priority Queue | Suitable | Not suitable |

## Conclusion

Max Heap is suitable for the hospital priority queue because
the highest-severity patient is maintained at the root and can
be accessed immediately. Insertion and deletion take O(log n)
time, making it suitable when patients continuously arrive
and the highest-priority patient must be handled first.
