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

# Get the number of rows and columns
rows = int(input("Enter the number of rows: "))
cols = int(input("Enter the number of columns: "))

# Read the elements of the array
print("Enter the elements of the array:")
elements = []

for i in range(rows):
    row = list(map(int, input().split()))
    elements.append(row)

# Create the NumPy array
arr = np.array(elements)

# Sort the array column-wise
sorted_arr = np.sort(arr, axis=0)

# Display the results
print("Original Array:")
print(arr)

print("Column-wise Sorted Array:")
print(sorted_arr)
```

## Output
<img width="563" height="573" alt="image" src="https://github.com/user-attachments/assets/26c09bd9-e44b-4a1b-8550-c789345db39d" />


## Result
The above Program has been executedd successfully.
