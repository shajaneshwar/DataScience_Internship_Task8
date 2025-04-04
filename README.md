# 🛡️ Fraud Detection using Decision Trees

This project focuses on detecting fraudulent financial transactions using a Decision Tree Classifier. The dataset is synthetically generated and demonstrates how feature engineering and hyperparameter tuning can improve fraud detection performance.

---

## 📁 Dataset

**Filename:** `fraud_detection.csv`  
**Columns:**
- `Transaction ID`: Unique transaction identifier
- `Amount`: Amount of transaction
- `Type`: Transaction type (credit/debit)
- `Is Fraud`: Label (1 = Fraud, 0 = Legitimate)

---

## 🧠 Objectives

- Detect fraudulent transactions using decision tree models.
- Enhance model performance through feature engineering.
- Tune hyperparameters using GridSearchCV.

---

## 📊 Project Workflow

### ✅ 1. Data Preprocessing
- Loaded the dataset
- Checked for null values
- Encoded categorical feature (`Type`)
- Removed unnecessary columns (`Transaction ID`)

### ✅ 2. Feature Engineering
- Created new features:
  - `HighAmount`: Flag for transactions > 2000
  - `Amount_log`: Log-transformed version of amount

### ✅ 3. Model Training
- Split data into train/test sets (80/20)
- Trained a `DecisionTreeClassifier`

### ✅ 4. Model Evaluation
- Evaluated using:
  - Confusion Matrix
  - Precision, Recall, F1-score

### ✅ 5. Hyperparameter Tuning
- Used `GridSearchCV` to tune parameters like:
  - `max_depth`
  - `min_samples_split`
  - `criterion`

---

## 📈 Results

After tuning, the Decision Tree model showed improved performance, especially in identifying fraudulent transactions (F1-score for class `1`).

---

## 📌 Tools Used

- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn


