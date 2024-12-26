# 🍷 Wine Quality Analysis and Classification

## 📖 Description
This project involves the analysis and classification of wine quality based on chemical and physical properties. Using the **Wine Quality Dataset** from the UCI Machine Learning Repository, the project implements data cleaning, exploratory data analysis, and predictive modeling to classify wine quality into binary categories (Good vs. Bad).

---

## 🚀 Objectives
- Perform data cleaning and preprocessing to handle duplicates, missing values, and type conversions.
- Analyze patterns and correlations in wine properties using visualizations and statistical summaries.
- Build and evaluate classification models:
  - **Logistic Regression**
  - **K-Nearest Neighbors (KNN)**
  - Additional models using LazyPredict for comparative analysis.

---

## 📊 Key Steps
1. **Data Cleaning**:
   - Removed duplicates from the dataset.
   - Ensured proper data types and handled missing values.

2. **Exploratory Data Analysis**:
   - Visualized distributions (e.g., histograms, boxplots) of features like acidity, alcohol, and sugar.
   - Analyzed correlations using heatmaps, highlighting relationships between variables like `alcohol` and `quality`.

3. **Modeling and Evaluation**:
   - Converted the target variable `quality` into a binary class: 0 (Bad) for scores ≤5 and 1 (Good) for scores >5.
   - Built pipelines for Logistic Regression and KNN models with preprocessing steps (scaling, imputing).
   - Evaluated models using metrics such as accuracy, precision, recall, and F1-score.

4. **Optimization**:
   - Tuned the hyperparameter `k` for KNN using cross-validation to achieve optimal performance.
   - Compared performance using LazyPredict, identifying `ExtraTreesClassifier` as the best model with 84% accuracy.

---

## 📈 Results
- Logistic Regression: Achieved ~74% accuracy on red wine and ~75% on white wine datasets.
- KNN: Outperformed Logistic Regression after optimization, with accuracy of ~76% on red wine and ~77% on white wine datasets.
- Best-performing model across all datasets: `ExtraTreesClassifier` with an accuracy of 84%.

---

## 🛠️ Tools and Technologies
- **Python**: Core programming language.
- **Jupyter Notebook**: For interactive exploration and analysis.
- **Libraries**:
  - Pandas & NumPy: Data manipulation.
  - Scikit-learn: Modeling and evaluation.
  - Matplotlib & Seaborn: Data visualization.
  - LazyPredict: Comparative model analysis.

---

## 📈 Insights
- Alcohol content is positively correlated with wine quality.
- Red wines tend to exhibit more variability in quality compared to white wines.
- The choice of classification model and its optimization greatly impacts prediction accuracy.
