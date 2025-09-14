# Heart Disease Prediction using Machine Learning

This project focuses on predicting the presence of heart disease using the **UCI Heart Disease Dataset**. The dataset contains various medical attributes such as age, sex, chest pain type, resting blood pressure, cholesterol level, and more, which are used to determine the likelihood of heart disease.

---

## Project Workflow

### 1. Data Loading and Preprocessing
- Loaded the dataset and inspected basic information.
- Handled missing values and performed data cleaning.
- Encoded categorical variables and scaled numerical features for model training.

---

### 2. Exploratory Data Analysis (EDA)
- **Distribution Analysis:** Count plots of the target variable (`num`) to understand class distribution.
- **Correlation Heatmap:** Explored relationships between features and target variable.
- **Boxplots & Histograms:** Visualized feature distributions and their effect on target labels.
- **Feature Importance (Random Forest):** Identified most influential features contributing to prediction.

---

### 3. Modeling

#### Multi-class Classification
- **Logistic Regression**
  - Accuracy: ~59%
  - Struggled with minority classes.
- **Random Forest**
  - Accuracy: ~57%
  - Improved performance on majority classes, but minority classes remained challenging.

#### Binary Classification (Presence vs. Absence of Heart Disease)
- **Logistic Regression**
  - Accuracy: ~83%
  - Balanced precision and recall.
- **Random Forest**
  - Accuracy: ~85%
  - Slightly better performance, higher recall for positive cases.

---

### 4. Results
- Multi-class classification performed moderately well but suffered due to class imbalance.
- Binary classification achieved strong performance, with Random Forest slightly outperforming Logistic Regression.
- Feature importance analysis revealed that attributes like **thalach (maximum heart rate achieved), cp (chest pain type), oldpeak, and ca (number of vessels colored by fluoroscopy)** are significant indicators of heart disease.

---

## Conclusion
- **Binary classification** is more reliable for this dataset compared to multi-class classification.
- Random Forest delivered the best results with an **accuracy of 85%**.
- Future improvements could include:
  - Hyperparameter tuning with GridSearchCV.
  - Applying advanced ensemble methods (XGBoost, LightGBM).
  - Addressing class imbalance using resampling techniques (SMOTE).

---

## Tech Stack
- **Programming Language:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn  
