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
```python
import pandas as pd

student_data1 = {
    'name': ['Anu', 'Bala'],
    'age': [20, 22],
    'score': [85, 92]
}

student_data2 = {
    'name': ['Chitra', 'David'],
    'age': [23, 21],
    'score': [76, 88]
}

df1 = pd.DataFrame(student_data1)
df2 = pd.DataFrame(student_data2)

df_combined = pd.concat([df1, df2], axis=0, ignore_index=True)

print("Result:\n", df_combined)
```
## Output
<img width="389" height="201" alt="438874180-87454350-90c1-4a5b-a4cd-b3e97cea8970" src="https://github.com/user-attachments/assets/f9c90b35-5960-4ed9-90d1-840e9cbc9d87" />

## Result
Thus the program has been successfully executed
