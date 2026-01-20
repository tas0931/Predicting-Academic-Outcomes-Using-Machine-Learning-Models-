**📘 Project Summary: Predicting Academic Outcomes [CSE422: Artificial Intelligence]**
**Problem Focus:** Educational data mining aims to predict student outcomes (graduation, dropout, continuous enrollment) to identify at-risk students early and improve retention programs.

**Objective:** Build and evaluate machine learning models to classify students into three groups: enrolled, graduate, and dropout, based on social, economic, academic, and cultural factors.

**Dataset:** 

link--https://drive.google.com/drive/folders/1bD49bV95E4OAmyI5TXnW-stWcZvtvCtP?usp=sharing

4,424 samples, 24 features (7 quantitative, 17 categorical).

Target variable: categorical (Graduate, Dropout, Enrolled).

Issues: class imbalance (Graduate > Dropout > Enrolled), missing values (~10%).

**Preprocessing:**

Dropped rows with missing target labels.

Removed redundant features (e.g., parental occupation/qualification).

**Imputation:** median for numeric, mode for categorical.

One-hot encoding for categorical variables.

Standardization of numeric features.

**Models Used:**

Neural Network: Best performance (62% accuracy), but weak recall for Enrolled class.

Logistic Regression: Balanced performance, strong micro/weighted averages.

Decision Tree: Underperformed (52% accuracy), sensitive to imbalance and high-dimensional data.

K-Means Clustering: Applied as unsupervised learning, but lower performance compared to supervised models.

**Evaluation Metrics:** Accuracy, precision, recall, F1-score, ROC curves.

**Key Findings:**

Severe class imbalance hindered detection of Enrolled students.

Neural networks outperformed others but struggled with minority classes.

Logistic regression captured linear relationships effectively.

Decision trees were unstable due to noise and imbalance.

**Conclusion:** Neural networks provided the best overall results, though improvements are needed for minority class detection (e.g., oversampling, advanced loss functions).
