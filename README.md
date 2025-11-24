# Credit Card Fraud Detection using Logistic Regression

A machine learning project that detects fraudulent credit card transactions using **Logistic Regression**.  
Due to the rarity of fraud cases, two datasets were **combined** to increase the number of fraud samples and improve model performance.

---

## 📘 Overview

This project includes:

- Loading and combining two credit card transaction datasets  
- Basic data exploration and cleaning  
- Feature/target selection  
- Train–test split  
- Logistic Regression model training  
- Model evaluation (accuracy)

All steps are performed in a Google Colab environment.

---

## 📊 Dataset Information

To address the lack of fraudulent samples, **two datasets were concatenated**, resulting in:

- **Anonymized features**: `V1` to `V28`  
- **Amount**: Transaction amount  
- **Class**:  
  - `0` → Genuine Transaction  
  - `1` → Fraudulent Transaction  

### ❗ Why SMOTE Was Not Used
SMOTE was avoided because:

- The dataset is **high-dimensional and anonymized**, making synthetic fraud points unreliable.  
- Artificial fraud samples can introduce noise and reduce generalizability.  
- Real-world fraud detection performs better with actual fraud patterns.

---

## 🚀 Steps Performed

### 1. Import Libraries
Used:
- `numpy`  
- `pandas`  
- `scikit-learn`  

### 2. Load & Combine Data
Both CSV files are loaded with `pandas` and concatenated to increase fraud cases.

### 3. Initial Exploration
- View first rows  
- Check null values  
- Analyze fraud distribution  

### 4. Data Cleaning
- Dropped irrelevant `id` column  

### 5. Feature Selection
- **Features** → All columns except `Class`  
- **Target** → `Class`

### 6. Train–Test Split
Dataset split into training and testing sets.

### 7. Model Training
Trained a **Logistic Regression** classifier.

### 8. Evaluation
Generated predictions and computed **accuracy score**.

---

## 🧪 Requirements

Install packages:

```
bash
pip install numpy pandas scikit-learn
```

---

## 📝 Notes

* Dataset remained imbalanced even after concatenation — accuracy should be interpreted carefully.
* For deeper evaluation, consider additional metrics such as **precision**, **recall**, **F1-score**, and **confusion matrix**.
* Further improvements could include advanced models or feature engineering.

---

## 📂 Files Included

* `credit_fraud.ipynb` → Full project notebook
* `README.md` → Project documentation

---

## 📄 License

This project is open-source and available for educational purposes.

---

If you want, I can also:

✅ Add dataset links  
✅ Add visualizations/badges  
✅ Add a sample confusion matrix  
✅ Format your `.ipynb` title section to match this README

Just tell me!
```
