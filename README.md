# CodeAlpha_DiseasePrediction

Machine Learning Internship at CodeAlpha, Task 4: Disease Prediction from Medical Data.

## Objective
Predict whether a tumor is **Malignant** or **Benign** from patient medical measurements using classification algorithms.

## Dataset
Breast Cancer Wisconsin (Diagnostic) dataset from the UCI ML Repository, loaded via scikit-learn.
- 569 patients
- 30 numeric features (radius, texture, perimeter, area, etc.)
- Target: 0 = Malignant, 1 = Benign

## Approach
1. Load and explore the dataset
2. Train-test split (80% / 20%, stratified)
3. Feature scaling with StandardScaler
4. Train and compare three models: Logistic Regression, SVM, Random Forest
5. Evaluate using Accuracy, Precision, Recall, F1-Score and ROC-AUC
6. Plot ROC curve, confusion matrix and feature importance

## Results

| Model               | Accuracy | Precision | Recall | F1     | ROC-AUC |
|---------------------|----------|-----------|--------|--------|---------|
| Logistic Regression | 0.9825   | 0.9861    | 0.9861 | 0.9861 | 0.9954  |
| SVM                 | 0.9825   | 0.9861    | 0.9861 | 0.9861 | 0.9950  |
| Random Forest       | 0.9561   | 0.9589    | 0.9722 | 0.9655 | 0.9932  |

**Best model: Logistic Regression** (Accuracy 98.25%, ROC-AUC 0.9954).

## Conclusion
- Logistic Regression and SVM performed best and almost identically.
- Random Forest scored slightly lower overall but had the highest Recall.
- High Recall matters in medical problems, since missing a real case is costly.

## Tech Stack
Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, Jupyter Notebook

## How to Run
1. Install the libraries: `pip install scikit-learn pandas matplotlib seaborn jupyter`
2. Open the notebook: `jupyter notebook CodeAlpha_Task4_DiseasePrediction.ipynb`
3. Run all cells (Kernel, then Restart & Run All)

## Author
Parmar Sejal, Machine Learning Intern at CodeAlpha
