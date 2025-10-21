# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program
```
import numpy as np

# Create a 2D array
arr = np.array([[15, 12, 18],
                [10, 25, 8],
                [30, 5, 20]])

print("Original Array:")
print(arr)

# Sort each column in ascending order
sorted_arr = np.sort(arr, axis=0)

print("\nArray after sorting each column in ascending order:")
print(sorted_arr)
```

## Output
```
Original Array:
[[15 12 18]
 [10 25  8]
 [30  5 20]]

Array after sorting each column in ascending order:
[[10  5  8]
 [15 12 18]
 [30 25 20]]
```
## Result
successfully created
