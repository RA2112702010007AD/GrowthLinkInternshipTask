#**GrowthLinkInternshipTask**

Machine Learning Project

**Task 3: Customer Churn Prediction**

• The objective is to predict whether a customer will discontinue a subscription-based service. • Historical customer data should be analyzed, considering factors like usage patterns,       demographic details,subscription duration, etc. 

• Customer data may have missing values, appropriate imputation strategies must be applied. 

• Expected Outcome: A model that effectively identifies customers likely to leave, along with insights into the mostsignificant factors contributing to churn. 

Ah, the journey begins! 🚀 Here's your **step-by-step guide** to running the **Bank Customer Churn Prediction project** in Google Colab—from setting the stage to reading the final act. Ready? Let's roll:

---

## ✅ Steps to Run the Project on Google Colab

---

###**🌱 Step 1: Open Google Colab**
- Go to [https://colab.research.google.com](https://colab.research.google.com)
- Click on **New Notebook** or upload one later if you save this script as `.ipynb`

---

###**📦 Step 2: Install kagglehub**
```python
!pip install kagglehub -q
```

- This package lets us download datasets directly from [KaggleHub](https://www.kagglehub.com/).

---

###**📁 Step 3: Download the Dataset**
```python
import kagglehub

path = kagglehub.dataset_download("shantanudhakadd/bank-customer-churn-prediction")
print("Path to dataset files:", path)
```

> ⚠️ If you run into issues, make sure you're logged in to KaggleHub via browser once.

---

###**📊 Step 4: Load and Explore the Data**
```python
import pandas as pd
df = pd.read_csv(path + '/Bank Customer Churn Prediction.csv')  # Adjust filename if needed
df.head()
```

---

###**🧼 Step 5: Clean the Data**
- Handle missing values using imputation
- Encode categorical columns (like `Gender`, `Geography`)
- Scale numerical data

---

###**🤖 Step 6: Build and Train the Model**
- Use **Random Forest Classifier** (or any other model)
- Split into training and test sets
- Fit the model and make predictions

---

###**📈 Step 7: Evaluate the Model**
- Print the **classification report**
- Plot a **confusion matrix**
- Visualize **feature importances**

---

###**🔍 Step 8: Understand the Results**
- Check top features that influence customer churn (like `Tenure`, `Balance`, `Age`)
- Use this for actionable insights into why customers are leaving

---



