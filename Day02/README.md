# Simple Linear Regression (Scikit-learn) — `SimpleLinearReg.ipynb`

This project demonstrates an end-to-end **Simple Linear Regression** workflow in a Jupyter Notebook using **Pandas, NumPy, Matplotlib, and Scikit-learn**.

The notebook covers the typical steps you need to train and visualize a simple regression model:

- Load a CSV dataset
- Split data into features (`X`) and target (`y`)
- Train/test split (80/20)
- Fit a `LinearRegression` model on the training set
- Predict on the test set
- Visualize regression line + scatter plots for train and test sets

---

## Files

- `SimpleLinearReg.ipynb` — main notebook (training + prediction + visualization)
- `studentscores.csv` — dataset file (you must include this in the repo or update the path in the notebook)

> The notebook expects the CSV file name to be exactly: `studentscores.csv`

---

## Dataset Assumptions

The notebook reads:

```python
df = pd.read_csv('studentscores.csv')
X = df.iloc[:, :1].values
y = df.iloc[:, 1].values