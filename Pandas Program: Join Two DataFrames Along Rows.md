# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program

```
import pandas as pd

# Create the first DataFrame
student_data1 = {
    'student_id': ['S1', 'S2', 'S3', 'S4', 'S5'],
    'name': ['Dani', 'Riya', 'John', 'Asha', 'Kiran'],
    'marks': [200, 210, 190, 222, 199]
}

df1 = pd.DataFrame(student_data1)

# Create the second DataFrame
student_data2 = {
    'student_id': ['S6', 'S7', 'S8', 'S9', 'S10'],
    'name': ['Rahul', 'Priya', 'Sam', 'Meera', 'Arun'],
    'marks': [201, 200, 198, 219, 205]
}

df2 = pd.DataFrame(student_data2)

# Concatenate the DataFrames row-wise
new_df = pd.concat([df1, df2], axis=0)

# Display the new DataFrame
print(new_df)
```

## Output
<img width="497" height="428" alt="image" src="https://github.com/user-attachments/assets/50880959-2f5f-4b15-8793-0aa783ab917a" />

## Result
The above program has been executed successfully.
