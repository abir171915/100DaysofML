# Multiple Linear Regression (Scikit-learn) — `MultipleLinearReg.ipynb`

This notebook implements an end-to-end **Multiple Linear Regression** workflow using **Pandas, NumPy, and Scikit-learn** on the classic **`50_Startups.csv`** dataset.

It covers:
- Loading a CSV dataset
- Splitting into features (`X`) and target (`y`)
- Encoding a categorical feature using **One-Hot Encoding** via `ColumnTransformer`
- Train/test split (80/20)
- Training a `LinearRegression` model
- Making predictions on the test set

---

## Files

- `MultipleLinearReg.ipynb` — main notebook
- `50_Startups.csv` — dataset file (must be present locally for the notebook to run)

> **Important:** The notebook expects `50_Startups.csv` to be in the **same folder** as `MultipleLinearReg.ipynb`.

---

## Dataset Expectations (`50_Startups.csv`)

The notebook assumes the dataset has **5 columns** where:

- **Columns 0–3** are features (inputs)
- **Column 4** is the target (output)

This is based on the code:

```python
X = df.iloc[:, :-1].values
y = df.iloc[:, 4].values