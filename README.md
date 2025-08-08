# 🩺 Breast Cancer Classification using Logistic Regression

## 📌 Overview
This project applies **Logistic Regression** to classify breast tumors as **Malignant (M)** or **Benign (B)** using the Breast Cancer dataset.  
The workflow covers:
1. Data preprocessing
2. Train-test split & feature scaling
3. Logistic Regression model training
4. Model evaluation using confusion matrix, precision, recall, and ROC-AUC
5. Threshold tuning and explanation of the **Sigmoid function**

---

## 📂 Dataset
The dataset used is **Breast Cancer Wisconsin (Diagnostic) Data Set**:
- **Features:** 30 numerical attributes (e.g., radius, texture, smoothness)
- **Target:** `diagnosis` (M = malignant, B = benign)

**Source:** Commonly available in `sklearn.datasets` or CSV format.

---

## ⚙️ Steps in the Project
1. **Load Dataset**  
   Remove irrelevant columns (`id`, unnamed) and encode target (`M`=1, `B`=0).

2. **Preprocessing**  
   - Train/test split (80%-20%)
   - Standardize features using `StandardScaler`

3. **Model Training**  
   Logistic Regression with `max_iter=1000`.

4. **Evaluation**  
   - Confusion Matrix
   - Precision & Recall
   - ROC Curve & AUC Score

5. **Threshold Tuning**  
   - Explore thresholds from 0 to 1
   - Plot **Precision vs Threshold** and **Recall vs Threshold**
   - Understand trade-offs between false positives and false negatives

6. **Sigmoid Function Explanation**  
   - Formula:  
     \[
     \sigma(z) = \frac{1}{1 + e^{-z}}
     \]  
   - Converts model score into a probability (0–1 range).

---

## 📊 Results 
- **Precision:** 97.5%  
- **Recall:** 92.86%  
- **ROC-AUC:** 0.996  

**Confusion Matrix (Threshold=0.5):**
