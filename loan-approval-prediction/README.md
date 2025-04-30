# 🧠 Loan Approval Prediction – Mini Classification Model

## 📌 Overview

This project is a simple yet powerful demonstration of supervised machine learning using a **Decision Tree Classifier** to predict whether a loan should be approved based on applicant data. It walks through the complete ML pipeline from scratch, built using Python and Jupyter Notebook.

---

## ✅ Problem Statement

Lenders often need to assess whether a loan applicant is likely to repay their loan. This model helps automate that process by predicting loan approval using features like income, credit score, employment history, and loan amount.

---

## 🔧 Tools & Libraries

- Python
- Jupyter Notebook
- `pandas`, `numpy`, `matplotlib`, `seaborn`
- `scikit-learn` (DecisionTreeClassifier, train_test_split, evaluation metrics)

---

## 📂 Workflow

1. **Data Creation** – Built a small, fake dataset of loan applicants
2. **EDA** – Explored feature distributions, correlations, and patterns
3. **Preprocessing** – Split data into features (`X`) and target (`y`), then into train/test sets
4. **Modeling** – Trained a Decision Tree classifier
5. **Evaluation** – Assessed performance using accuracy, precision, recall, F1-score, and a confusion matrix
6. **Real-World Prediction** – Used the trained model to predict approval for new applicants

---

## 🔍 Key Insights

- Income, Credit Score, and Years Employed were highly correlated with loan approval
- Decision Trees don't require feature scaling or normalization
- Accuracy and F1-score were both 1.00 on a small, clean dataset

---

## 🧪 Sample Prediction

```python
new_applicant = pd.DataFrame({
    'Age': [33],
    'Income': [75000],
    'CreditScore': [705],
    'YearsEmployed': [5],
    'LoanAmount': [25000]
})

prediction = model.predict(new_applicant)
print("Loan Approved?", "✅ Yes" if prediction[0] == 1 else "❌ No")
```

## 💡 What I Learned

Full ML workflow: from raw data to deployment-ready prediction
How to evaluate models with confidence
Why feature selection, ordering, and cleaning matter
How to visually interpret decision logic using correlation heatmaps and tree diagrams

## 🚀 Next Steps

Try more complex models like RandomForestClassifier or XGBoost
Introduce noise or imbalanced classes for more realism
Build a simple web app or API around this model
