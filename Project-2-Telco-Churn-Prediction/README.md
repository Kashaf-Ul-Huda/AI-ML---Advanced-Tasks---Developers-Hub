
---

## 📌 **Task 2 – Customer Churn Prediction Pipeline**
```markdown
# 📞 Customer Churn Prediction – End-to-End ML Pipeline

## 📍 Objective
Develop a **production-ready ML pipeline** to predict customer churn using **Telco Customer Churn Dataset**.  
Pipeline includes preprocessing, model training, hyperparameter tuning, and export.

---

## 📊 Dataset
- **Telco Customer Churn Dataset**  
- Features: Demographics, services, billing info  
- Target: `Churn` (Yes/No → 1/0)

---

## ⚙️ Methodology
1. **Data Preprocessing**
   - Drop `customerID`  
   - Convert `TotalCharges` to numeric  
   - Impute missing values  
   - One-hot encode categorical features  
   - Scale numeric features  

2. **Pipeline Construction**
   - `ColumnTransformer` for preprocessing  
   - Integrated with ML models via `Pipeline`  

3. **Models & Hyperparameter Tuning**
   - **Logistic Regression**  
   - **Random Forest**  
   - Tuned with `GridSearchCV` (3-fold CV, F1 scoring)  

4. **Evaluation**
   - Accuracy, F1, Confusion Matrix, Classification Report  

5. **Export**
   - Save trained pipeline using `joblib`  

---

## ✅ Results
- **Best model selected via GridSearch**  
- Achieved **Accuracy ~80–85%**  
- Macro **F1-score ~0.78–0.82**  

---
