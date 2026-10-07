# Bank Marketing Prediction with Decision Trees 🏦

A machine learning project that predicts whether a customer will subscribe to a term deposit, built as Task 3 of my Prodigy InfoTech internship. It covers exploring the data, cleaning it, and training Decision Tree classifiers.

## 🛠️ Technologies
- **Python**
- **Pandas** and **NumPy** for data handling
- **Matplotlib** and **Seaborn** for charts
- **Scikit-learn** for encoding, modelling, and evaluation
- **Google Colab / Jupyter Notebook**

## ✨ Features
- Data checks: shape, data types, duplicates, and missing values
- Histograms of numeric columns and count plots of categorical columns
- Boxplots to spot outliers, with IQR-based outlier handling
- Correlation heatmap to find highly correlated features
- Label encoding of categorical columns
- Two Decision Tree models, one using Gini and one using Entropy
- Evaluation with accuracy, confusion matrix, and classification report
- Tree diagrams to show how the model makes decisions

## 🔄 The Process
1. Loaded `bank-additional.csv` and renamed the target column `y` to `deposit`
2. Checked structure, duplicates, and missing values
3. Visualised numeric and categorical features
4. Handled outliers in `age`, `campaign`, and `duration` using the IQR method
5. Checked correlations and found highly related features (`emp.var.rate`, `euribor3m`, `nr.employed`)
6. Encoded categorical data and split it into 75% training and 25% testing
7. Trained two Decision Trees and compared their scores
8. Evaluated the results and plotted the trees

## 📚 What I Learned
- **EDA First:** Looking at distributions, outliers, and correlations before building any model.
- **Outliers:** Using the IQR rule and boxplots to find and handle extreme values.
- **Encoding:** Turning text categories into numbers with `LabelEncoder` so models can use them.
- **Decision Trees:** How `criterion`, `max_depth`, and `min_samples_split` change the tree.
- **Overfitting:** Comparing training and testing scores to see if a model memorises the data.
- **Evaluation:** Reading a confusion matrix and classification report instead of relying on accuracy alone.

## 📁 Files
- `bank-additional.csv`: the dataset
- `prodigy_3.py`: the analysis and model script

## ▶️ How to Run
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
python prodigy_3.py
```
