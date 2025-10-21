# Pandas Program: Create and Display a DataFrame with Custom Index Labels

## 🎯 Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

---

## 🧠 Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.

---

## 💻 Program
```
import pandas as pd


data = {
    'name': ['Aman', 'Kamal', 'Amjad', 'Rohan', 'Amit', 'Sumit', 'Matthew', 'Kartik', 'Kavita', 'Pooja'],
    'perc': [79.5, 29.0, 90.5, None, 32.0, 65.0, 56.0, None, 29.0, 89.0],
    'qualify': ['yes', 'no', 'yes', 'no', 'no', 'yes', 'yes', 'no', 'no', 'yes']
}
df = pd.DataFrame(data, index=list('ABCDEFGHIJ'))

print("Original data frame:")
print(df)

row = input().strip()
new_perc = float(input())


df.loc[row, 'perc'] = new_perc

print(f"Change the percentage in row {row} to {new_perc}")
print(df)
```

## Output

<img width="1121" height="870" alt="m5-3" src="https://github.com/user-attachments/assets/c13010e1-e20d-4b18-8f26-b069458b1d3b" />

## Result
successfuly created
