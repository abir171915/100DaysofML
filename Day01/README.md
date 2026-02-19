# Data Preprocessing Pipeline (Scikit-learn) — `DataPreprocess.ipynb`

This repository contains a simple, end-to-end **data preprocessing workflow** implemented in a Jupyter Notebook using **NumPy, Pandas, and Scikit-learn**. The notebook demonstrates the common preprocessing steps required before training a machine learning model:

- Loading a CSV dataset
- Separating features (`X`) and target (`y`)
- Handling missing values (mean imputation)
- Encoding categorical variables (label + one-hot encoding)
- Splitting into training and test sets
- Feature scaling (standardization)

---

## Contents

- `DataPreprocess.ipynb` — main notebook containing the preprocessing steps
- `Data.csv` — your dataset (must be added to the repo, see below)

---

## Dataset Expectations

The notebook currently assumes:

- The dataset is stored as **`Data.csv`** in the **same directory** as the notebook.
- The dataset has **4 columns** (0–3):
  - **Column 0**: categorical feature (e.g., country/category)
  - **Columns 1–2**: numeric features (may contain missing values)
  - **Column 3**: target/label column

This is based on the lines in the notebook:

```python
df = pd.read_csv("Data.csv")
X = df.iloc[:,:-1].values
y = df.iloc[:,3].values
