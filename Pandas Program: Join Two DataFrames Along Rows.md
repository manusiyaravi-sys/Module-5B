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
a=pd.DataFrame({'student_id': ['S1', 'S2', 'S3', 'S4', 'S5'],'name': ['Danniella Fenton', 'Ryder Storey', 'Bryce Jensen', 'Ed Bernal', 'Kwame Morin'],'marks': [200, 210, 190, 222, 199]})
b=pd.DataFrame({'student_id': ['S4', 'S5', 'S6', 'S7', 'S8'],'name': ['Scarlette Fisher', 'Carla Williamson', 'Dante Morse', 'Kaiser William', 'Madeeha Preston'],'marks': [201, 200, 198, 219, 201]})

print('Original DataFrames:')
print(a)
print(b)
a=pd.DataFrame({'student_id': ['S1', 'S2', 'S3', 'S4', 'S5'],'name_x': ['Danniella Fenton', 'Ryder Storey', 'Bryce Jensen', 'Ed Bernal', 'Kwame Morin'],'marks_x': [200, 210, 190, 222, 199]})
b=pd.DataFrame({'student_id': ['S4', 'S5', 'S6', 'S7', 'S8'],'name_y': ['Scarlette Fisher', 'Carla Williamson', 'Dante Morse', 'Kaiser William', 'Madeeha Preston'],'marks_y': [201, 200, 198, 219, 201]})

c=pd.merge(a,b,on=['student_id'],how='inner')
print('Merged data (inner join):')
print(c)
```

## Output

<img width="1613" height="404" alt="m5-4" src="https://github.com/user-attachments/assets/75ab976c-e71d-44b9-8c66-b0d03f1ab8d9" />

## Result
successfuly created
