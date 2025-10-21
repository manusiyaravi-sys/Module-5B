# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program

```
import numpy as np
a=np.array(eval(input()))
b=np.array(eval(input()))
print("Before inserting new column")
print(f" {a}")
a=np.insert(a,a.shape[1],b,axis=1)
print("After inserting new column")
print(f" {a}"
```
## Output

<img width="1312" height="734" alt="m5-2" src="https://github.com/user-attachments/assets/4fdadb32-4346-446c-bc5d-3ee3f788b604" />

## Result
successfuly created
