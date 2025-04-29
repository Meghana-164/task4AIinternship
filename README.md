# Task 4: Logistic Regression on Breast Cancer Diagnosis Dataset

##  Objective
To apply logistic regression to predict whether a tumor is **Benign (B)** or **Malignant (M)** using the Breast Cancer Wisconsin dataset. Focus was on visualizing the **sigmoid function**, evaluating performance via **confusion matrix**, **ROC curve**, and **classification report**.

---

## 📈Sigmoid Curve Visualization

The following plot shows the sigmoid output from logistic regression using the standardized `radius_mean` feature. As the value of radius increases, the predicted probability of malignancy rises smoothly, forming the characteristic **S-shaped sigmoid curve**.



- **X-axis**: Standardized `radius_mean`
- **Y-axis**: Predicted Probability (Malignant)
- The model uses a threshold of 0.5 to classify tumors.

---

##  Confusion Matrix

|              | Predicted Benign | Predicted Malignant |
|--------------|------------------|----------------------|
| **Actual Benign**    | 70               | 1                    |
| **Actual Malignant** | 2                | 41                   |

- **True Negatives (TN)**: 70
- **False Positives (FP)**: 1
- **False Negatives (FN)**: 2
- **True Positives (TP)**: 41

---

##  Classification Report

| Class        | Precision | Recall | F1-Score | Support |
|--------------|-----------|--------|----------|---------|
| Benign (0)   | 0.97      | 0.99   | 0.98     | 71      |
| Malignant (1)| 0.98      | 0.95   | 0.96     | 43      |

- **Accuracy**: `0.97`
- **Macro Avg**: Precision = 0.97, Recall = 0.97, F1 = 0.97
- **Weighted Avg**: Precision = 0.97, Recall = 0.97, F1 = 0.97

---

## 📉 ROC Curve and AUC Score

The ROC curve shows an excellent model with high separability between classes.


- **AUC Score**: `0.997`

---

##  Conclusion

- The model achieved **97% accuracy** with **very high precision and recall** for both classes.
- **False negatives** were minimal (only 2), which is crucial in cancer diagnosis.
- The sigmoid curve provides an interpretable decision boundary for classification.
- The **ROC AUC of 0.997** indicates near-perfect classification capability.

---

## Files

- `logistic_model.ipynb` – Notebook containing code for model training and evaluation
- `README.md` – Summary of results (this file)
- `sigmoidal curve.png` – Sigmoid visualization
- `ROC curve.png` – ROC Curve visualization

---

