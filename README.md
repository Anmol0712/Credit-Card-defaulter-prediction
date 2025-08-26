# Credit Card Default Prediction  

This project predicts whether a credit card client will **default on their payment next month** using machine learning models.  
The dataset is the **Default of Credit Card Clients in Taiwan** from the UCI Machine Learning Repository.  

---

## 📊 Dataset  

- **Source:** Kaggle
- **Size:** 30,000 clients  
- **Features:** 23 predictors + 1 target  
- **Key Variables:**  
  - Demographics → `SEX`, `EDUCATION`, `MARRIAGE`, `AGE`  
  - Credit & Billing → `LIMIT_BAL`, `BILL_AMT1-6`, `PAY_AMT1-6`  
  - Repayment History → `PAY_0` to `PAY_6`  
- **Target:** `default.payment.next.month` (1 = default, 0 = no default)  

---

## ⚙️ Models Implemented  

- Logistic Regression  
- K-Nearest Neighbors (KNN)  
- Decision Tree  
- Random Forest  
- Support Vector Machine (SVM)  

---

## 📈 Results  

| Model              | Accuracy | Notes |
|---------------------|----------|-------|
| Logistic Regression | ~81%     | Good baseline, linear relationships only |
| KNN                 | ~79%     | Lower recall, struggles with imbalance |
| Decision Tree       | ~71%     | Overfits easily |
| Random Forest       | ~82%     | Best balance between accuracy & interpretability |
| SVM                 | ~82%     | High accuracy, less interpretable |

👉 **Random Forest was chosen as the final model** due to its robustness, interpretability, and feature importance insights.  
