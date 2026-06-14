# Cancer Survival Prediction

Machine Learning project for predicting cancer patient survival using classification models.

---

## Project Overview

This project focuses on predicting whether a cancer patient survives based on demographic, clinical, and lifestyle-related factors. The dataset contains approximately 890,000 records and 17 features, making it a large-scale binary classification problem.

One of the key challenges in this dataset was class imbalance, where only about 22% of patients belonged to the survival class. To address this issue, SMOTE (Synthetic Minority Oversampling Technique) was applied during preprocessing.

---

## Dataset

- Source: Kaggle
- Records: ~890,000
- Features: 17
- Target Variable: `survived`
- Problem Type: Binary Classification

### Target Classes

| Value | Meaning |
|---------|---------|
| 0 | Did Not Survive |
| 1 | Survived |

---

## Project Workflow

### 1. Data Exploration (EDA)

Performed exploratory data analysis to understand feature distributions and relationships.

Techniques used:

- Histograms
- Boxplots
- Correlation Heatmaps
- Class Distribution Analysis

### 2. Data Preprocessing

Data preparation included:

- Missing value handling
- Outlier detection and removal
- Feature engineering
- Feature scaling using StandardScaler
- Categorical feature encoding using OneHotEncoder

### 3. Class Balancing

The dataset was highly imbalanced.

To improve model performance on the minority class:

- SMOTE (Synthetic Minority Oversampling Technique) was applied
- Training data was balanced before model training

### 4. Model Training

The following machine learning models were trained and evaluated:

- Logistic Regression
- Random Forest Classifier
- XGBoost Classifier

### 5. Hyperparameter Tuning

Model optimization was performed using:

- GridSearchCV

### 6. Model Evaluation

Models were evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC Score
- Confusion Matrix

---

## Visualizations

### Class Distribution Before and After SMOTE

Shows how class imbalance was addressed before model training.

### Correlation Heatmap

Displays relationships between numerical features.

### Feature Distribution Analysis

Histograms and boxplots were used to analyze feature distributions and identify potential outliers.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)
- XGBoost
- Google Colab

---

## Repository Structure

```text
cancer-survival-prediction/
│
├── notebooks/
│   └── group_pipeline.ipynb
│
├── screenshots/
│   ├── class_distribution_smote.png
│   ├── correlation_heatmap.png
│   └── raw_data_histograms.png
│
└── README.md
```

---

## Future Improvements

- Feature selection optimization
- Additional ensemble models
- Explainable AI techniques (SHAP/LIME)
- Model deployment using Flask or Streamlit

---

## Academic Information

This project was developed as part of a university Machine Learning group project involving six team members.

---

## License

This repository is intended for educational and portfolio purposes.
