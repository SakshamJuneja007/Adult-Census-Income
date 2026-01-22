# Adult-Census-Income
Adult Census Income Dataset – Data Preprocessing for Machine Learning (Level 1)

📌 Project Overview

This project focuses on preprocessing a real-world raw dataset to make it suitable for machine learning models.  
The Adult Census Income dataset is used to demonstrate essential data cleaning and preprocessing techniques commonly applied in machine learning pipelines.

---

📊 Dataset Information

Dataset Name: Adult Census Income Dataset  
Source: UCI Machine Learning Repository / Kaggle  
Records: 32,561  
Features: 14 (before preprocessing)  
Target Variable: Income  

---

🎯 Objectives

The main objectives of this task are:

- Handle missing values in the dataset  
- Encode categorical variables into numerical form  
- Normalize / standardize numerical features  
- Split the dataset into training and testing sets  

---

🔧 Data Preprocessing Steps

### 1️⃣ Handling Missing Values

- Missing values were present in categorical columns as special symbols (`?`)
- These values were first converted to NaN
- Missing values were handled using **mode imputation** for categorical features:

Columns handled:
- workclass  
- occupation  
- native.country  

✔ Result: Dataset with no missing values

---

### 2️⃣ Encoding Categorical Variables

- Categorical columns were converted into numerical form using **One-Hot Encoding**
- This ensures compatibility with machine learning algorithms

✔ Result: All categorical features encoded into machine-readable format

---

### 3️⃣ Feature Scaling

- **StandardScaler** was applied to numerical features:
  - age  
  - fnlwgt  
  - capital.gain  
  - capital.loss  
  - hours.per.week  

This ensures:
- Mean = 0  
- Standard Deviation = 1  

✔ Result: Numerical features standardized for ML readiness

---

### 4️⃣ Train-Test Split

- Dataset split into:
  - Training Set: 80%
  - Testing Set: 20%
- `random_state = 42` used for reproducibility

✔ Result: Dataset prepared for machine learning workflows

---

🛠️ Tools & Technologies Used

- Python  
- pandas  
- NumPy  
- scikit-learn  
- matplotlib  
- seaborn  
- Google Colab 

---

📈 Final Outcome

✅ Missing values handled  
✅ Categorical encoding completed  
✅ Feature scaling applied  
✅ Train-test split performed  

The cleaned dataset is now fully prepared for use in machine learning models.

---

📌 Note

This task focuses only on **data preprocessing**.  
Model training and evaluation will be performed in subsequent tasks.
