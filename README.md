# Breast_Cancer_Detection_with_Logistic_Regression_XAI

Objective:
Developed a high-performance machine learning model to classify breast cancer tumors as Benign or Malignant, emphasizing both accuracy and explainability for clinical trust.

Key Steps & Methods:

->Data: 569 samples, 33 features from data.csv.

->Preprocessing: Mapped diagnosis (‘M’→1, ‘B’→0) and applied StandardScaler for normalization.

->Model: Logistic Regression selected for its interpretability and efficiency.

Results:

Accuracy: 98.25% on test data
Confusion Matrix: TN = 70, TP = 42, FP = 1, FN = 1
ROC-AUC: 0.997 (near-perfect discrimination)
Precision/Recall: 0.99 (Benign), 0.98 (Malignant)

Explainable AI Implementation:
LIME (Local): Explained individual predictions; for one case, 95.15% probability of Benign influenced mainly by area_worst ≤ -0.63.
SHAP (Global): Identified top contributing features — concave points_mean, area_worst, and radius_worst — via beeswarm and summary plots.



