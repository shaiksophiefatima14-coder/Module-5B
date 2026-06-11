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

# Get the dimensions of the array
rows = int(input("Enter the number of rows: "))
cols = int(input("Enter the number of columns: "))

# Read the elements of the array
print("Enter the elements of the array:")
data = []

for i in range(rows):
    row = list(map(int, input().split()))
    data.append(row)

# Create the NumPy array
arr = np.array(data)

# Read the new column values
print("Enter the elements of the new column:")
new_col = list(map(int, input().split()))

# Delete the second column (index 1)
arr_deleted = np.delete(arr, 1, axis=1)

# Insert the new column at index 1
updated_arr = np.insert(arr_deleted, 1, new_col, axis=1)

# Display the results
print("Original Array:")
print(arr)

print("Updated Array:")
print(updated_arr)
```

## Output
<img width="557" height="467" alt="image" src="https://github.com/user-attachments/assets/d15e6489-457e-4421-8123-18d8d440a577" />

## Result
The above reuslt has been executed successfully.
