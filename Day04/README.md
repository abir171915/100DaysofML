\# Logistic Regression Classification — `LogesticReg.ipynb`



This project demonstrates a complete \*\*binary classification workflow\*\* using \*\*Logistic Regression\*\* with \*\*Scikit-learn\*\* in Jupyter Notebook.



The notebook uses the \*\*Social\_Network\_Ads.csv\*\* dataset and walks through the standard machine learning pipeline:



\- Importing libraries

\- Loading the dataset

\- Selecting features and target

\- Splitting data into training and test sets

\- Feature scaling using `StandardScaler`

\- Training a Logistic Regression model

\- Making predictions on test data

\- Evaluating results using a confusion matrix



---



\## Files



\- `LogesticReg.ipynb` — main notebook containing the classification workflow

\- `Social\_Network\_Ads.csv` — dataset used in the notebook



> \*\*Important:\*\* The notebook expects `Social\_Network\_Ads.csv` to be in the \*\*same folder\*\* as the notebook.



---



\## Project Overview



Logistic Regression is a supervised machine learning algorithm used for \*\*classification problems\*\*, especially when the target variable has \*\*two classes\*\* such as:



\- Yes / No

\- 0 / 1

\- Purchased / Not Purchased



In this notebook, the model is trained to predict whether a user will make a purchase based on selected features from the dataset.



---



\## Dataset Information



The notebook reads the dataset using:



```python

df = pd.read\_csv('Social\_Network\_Ads.csv')

