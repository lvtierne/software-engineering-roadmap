# Sorting Algorithms

Sorting algorithms are used to arrange elements in a specific order (ascending or descending).

## Key Algorithms
- **Bubble Sort**: Simple comparison-based sorting algorithm.
- **Merge Sort**: Divide-and-conquer algorithm for efficient sorting.
- **Quick Sort**: Efficient sorting algorithm using partitioning.

## Example: Python Quick Sort
```python
def quick_sort(arr):
    if len(arr) <= 1:
        return arr
    pivot = arr[len(arr) // 2]
    left = [x for x in arr if x < pivot]
    middle = [x for x in arr if x == pivot]
    right = [x for x in arr if x > pivot]
    return quick_sort(left) + middle + quick_sort(right)

# Example usage
arr = [3, 6, 8, 10, 1, 2, 1]
print(quick_sort(arr))
```

## Learning Resources

- [Sorting Algorithms - GeeksforGeeks](https://www.geeksforgeeks.org/sorting-algorithms/)
- [Sorting Algorithms in Python - Tutorialspoint](https://www.tutorialspoint.com/python_data_structure/python_sorting_algorithms.htm)

## Next Steps

1. Implement and compare different sorting algorithms.
2. Solve sorting problems on coding platforms.
