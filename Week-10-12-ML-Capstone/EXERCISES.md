# Week 10-12 Machine Learning & Capstone - Exercises & Solutions

## Exercise Set 1: Linear Regression

### Problems

**1.1 Simple Linear Regression**
```python
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_squared_error, r2_score
import numpy as np
import pandas as pd

# TODO: Create and train model:
# - X: [1, 2, 3, 4, 5] (reshaped)
# - y: [2, 4, 6, 8, 10]
# - Train LinearRegression
# - Make predictions
# - Calculate MSE and R²
# - Plot actual vs predicted
```

**1.2 Multiple Regression**
```python
# TODO: Use dataset with:
# - Multiple features (X)
# - Single target (y)
# - Split: 80/20 train/test
# - Train model
# - Evaluate on both sets
# - Check for overfitting
# - Print coefficients
```

**1.3 Polynomial Regression**
```python
from sklearn.preprocessing import PolynomialFeatures

# TODO:
# - Create X with one feature
# - Create polynomial features (degree 2, 3)
# - Train models with each
# - Compare performance
# - Plot results
# - Choose best degree
```

**1.4 Regularization**
```python
from sklearn.linear_model import Ridge, Lasso

# TODO:
# - Train Ridge regression with different alpha
# - Train Lasso regression with different alpha
# - Compare to regular LinearRegression
# - Plot coefficients vs alpha
# - Evaluate on test set
# - Explain when to use each
```

---

## Exercise Set 2: Logistic Regression & Classification

### Problems

**2.1 Binary Classification**
```python
from sklearn.linear_model import LogisticRegression
from sklearn.metrics import confusion_matrix, classification_report, accuracy_score

# TODO:
# - Create binary classification dataset
# - Split: 80/20
# - Train LogisticRegression
# - Make predictions
# - Calculate accuracy
# - Print confusion matrix
# - Print classification report
```

**2.2 Multi-class Classification**
```python
# TODO:
# - Use 3-class classification dataset
# - Train LogisticRegression
# - Make predictions
# - Confusion matrix
# - Macro and weighted F1 scores
# - Precision/recall per class
```

**2.3 Probability Predictions**
```python
# TODO:
# - Train logistic regression
# - Get probability predictions
# - Plot decision boundary
# - Show probability regions
# - Vary decision threshold
# - Evaluate at different thresholds
```

**2.4 ROC Curve**
```python
from sklearn.metrics import roc_curve, auc

# TODO:
# - Train classifier
# - Get probability predictions
# - Calculate ROC curve
# - Plot ROC curve
# - Calculate AUC
# - Interpret curve
```

---

## Exercise Set 3: K-Nearest Neighbors

### Problems

**3.1 Basic KNN**
```python
from sklearn.neighbors import KNeighborsClassifier

# TODO:
# - Train KNN with k=3, 5, 7
# - Evaluate each
# - Find optimal k
# - Plot accuracy vs k
# - Test on unseen data
```

**3.2 Distance Metrics**
```python
# TODO:
# - Compare distance metrics:
#   - Euclidean
#   - Manhattan
#   - Minkowski
# - Train models with each
# - Compare performance
# - Which performs best?
```

**3.3 Scaling Importance**
```python
from sklearn.preprocessing import StandardScaler

# TODO:
# - Create dataset with different scales
# - Train KNN without scaling
# - Train KNN with StandardScaler
# - Compare results
# - Explain importance
```

**3.4 KNN Regression**
```python
from sklearn.neighbors import KNeighborsRegressor

# TODO:
# - Use regression dataset
# - Train KNNRegressor with different k
# - Evaluate with MSE, MAE, R²
# - Find optimal k
# - Compare to LinearRegression
```

---

## Exercise Set 4: Decision Trees & Random Forests

### Problems

**4.1 Decision Tree**
```python
from sklearn.tree import DecisionTreeClassifier
from sklearn import tree

# TODO:
# - Train tree with different max_depth
# - Visualize tree
# - Get feature importance
# - Evaluate performance
# - Check for overfitting
# - Prune if needed
```

**4.2 Random Forest**
```python
from sklearn.ensemble import RandomForestClassifier

# TODO:
# - Train RandomForest with n_estimators: 10, 50, 100
# - Evaluate each
# - Get feature importance
# - Compare to single tree
# - Plot importance
# - Identify key features
```

**4.3 Feature Importance Analysis**
```python
# TODO:
# - Train forest on dataset
# - Calculate feature importance
# - Create importance dataframe
# - Plot top features
# - Drop unimportant features
# - Retrain and compare
```

**4.4 Ensemble Methods**
```python
from sklearn.ensemble import GradientBoostingClassifier, AdaBoostClassifier

# TODO:
# - Train GradientBoosting
# - Train AdaBoost
# - Train RandomForest
# - Compare all three
# - Evaluate metrics
# - Which is best for your data?
```

---

## Exercise Set 5: Support Vector Machines

### Problems

**5.1 Linear SVM**
```python
from sklearn.svm import SVC

# TODO:
# - Create linearly separable data
# - Train linear SVM
# - Visualize decision boundary
# - Vary C parameter
# - Evaluate performance
# - Show support vectors
```

**5.2 Non-linear SVM (Kernels)**
```python
# TODO:
# - Create non-linear data
# - Train SVM with different kernels:
#   - Linear
#   - Polynomial
#   - RBF
#   - Sigmoid
# - Compare visualizations
# - Which kernel fits best?
```

**5.3 Hyperparameter Tuning**
```python
from sklearn.model_selection import GridSearchCV

# TODO:
# - Define parameter grid (C, kernel, gamma)
# - Use GridSearchCV
# - Find best parameters
# - Print best score
# - Train with best params
# - Evaluate on test set
```

**5.4 SVM Regression**
```python
from sklearn.svm import SVR

# TODO:
# - Use regression dataset
# - Train SVR with different kernels
# - Tune hyperparameters
# - Evaluate with MSE, MAE, R²
# - Compare to LinearRegression
```

---

## Exercise Set 6: Clustering

### Problems

**6.1 K-Means**
```python
from sklearn.cluster import KMeans

# TODO:
# - Create dataset with multiple clusters
# - Train KMeans with k=2, 3, 4, 5
# - Calculate inertia for each
# - Plot elbow curve
# - Find optimal k
# - Visualize clusters
```

**6.2 Elbow Method**
```python
# TODO:
# - Train KMeans for k=1 to 10
# - Record inertia
# - Plot elbow curve
# - Find elbow point
# - Interpret results
# - Choose optimal k
```

**6.3 Silhouette Score**
```python
from sklearn.metrics import silhouette_score

# TODO:
# - Train KMeans with different k
# - Calculate silhouette score for each
# - Compare to inertia
# - Which metric better?
# - Visualize silhouette plots
```

**6.4 Hierarchical Clustering**
```python
from scipy.cluster.hierarchy import dendrogram, linkage

# TODO:
# - Use hierarchical clustering
# - Create dendrogram
# - Try different linkage methods
# - Compare to KMeans
# - Visualize results
```

---

## Exercise Set 7: Dimensionality Reduction

### Problems

**7.1 PCA Basics**
```python
from sklearn.decomposition import PCA

# TODO:
# - Load dataset with multiple features
# - Apply PCA with all components
# - Check explained variance ratio
# - Create scree plot
# - Determine components needed
# - Retain 95% variance
```

**7.2 PCA Visualization**
```python
# TODO:
# - Apply PCA(n_components=2)
# - Project data to 2D
# - Visualize in 2D space
# - Color by class/cluster
# - Compare original vs reduced
# - Evaluate information loss
```

**7.3 Feature Importance from PCA**
```python
# TODO:
# - Apply PCA
# - Get loading matrix
# - Identify important original features
# - Visualize loadings
# - Interpret results
```

**7.4 t-SNE**
```python
from sklearn.manifold import TSNE

# TODO:
# - Apply t-SNE with different perplexity
# - Visualize in 2D
# - Compare to PCA
# - Note: slower, better local structure
# - Good for visualization
```

---

## Exercise Set 8: Model Evaluation & Selection

### Problems

**8.1 Cross-Validation**
```python
from sklearn.model_selection import cross_val_score

# TODO:
# - Train multiple models
# - Use 5-fold cross-validation
# - Get cross-validation scores
# - Calculate mean and std
# - Compare models
# - Choose best model
```

**8.2 Train/Test/Validation Split**
```python
# TODO:
# - Split data: 60% train, 20% validation, 20% test
# - Train on training set
# - Tune hyperparameters on validation set
# - Evaluate on test set
# - Report all three metrics
```

**8.3 Hyperparameter Tuning**
```python
from sklearn.model_selection import GridSearchCV, RandomizedSearchCV

# TODO:
# - Define parameter grid
# - Use GridSearchCV
# - Use RandomizedSearchCV
# - Compare speed vs accuracy
# - Train final model
# - Evaluate on test set
```

**8.4 Learning Curves**
```python
from sklearn.model_selection import learning_curve

# TODO:
# - Plot learning curves
# - Analyze bias-variance
# - Identify overfitting/underfitting
# - Suggest improvements
# - Retrain with improvements
```

---

## Capstone Project (Week 12)

### Project Requirements

**Phase 1: Problem Definition & Exploration (Days 1-2)**

```python
# TODO:
# 1. Select dataset or topic
# 2. Define problem statement
# 3. Identify target variable
# 4. Determine problem type:
#    - Regression, Classification, Clustering
# 5. Exploratory Data Analysis:
#    - Data shape, types, missing values
#    - Descriptive statistics
#    - Visualizations
#    - Correlations
#    - Distributions
# 6. Document findings
```

**Phase 2: Data Preprocessing (Days 2-3)**

```python
# TODO:
# 1. Handle missing values
# 2. Deal with outliers
# 3. Encode categorical variables
# 4. Feature scaling/normalization
# 5. Feature engineering
# 6. Create train/test split
# 7. Document all preprocessing steps
```

**Phase 3: Model Development (Days 3-4)**

```python
# TODO:
# 1. Try multiple algorithms:
#    - For regression: LinearReg, Ridge, SVR, RandomForest
#    - For classification: LogisticReg, SVM, RF, GradientBoosting
# 2. Baseline model
# 3. Cross-validation
# 4. Hyperparameter tuning
# 5. Train final models
# 6. Compare performance
```

**Phase 4: Model Evaluation (Days 4-5)**

```python
# TODO:
# 1. For regression:
#    - MSE, RMSE, MAE, R²
#    - Residual analysis
#    - Prediction plots
# 2. For classification:
#    - Accuracy, Precision, Recall, F1
#    - Confusion matrix
#    - ROC-AUC curves
# 3. Feature importance
# 4. Error analysis
# 5. Compare to baseline
```

**Phase 5: Visualization & Reporting (Days 5-6)**

```python
# TODO:
# 1. Key findings visualization
# 2. Model comparison plots
# 3. Feature importance charts
# 4. Prediction examples
# 5. Business impact quantification
# 6. Professional report/presentation
```

**Phase 6: Documentation & Presentation (Day 6)**

```python
# TODO:
# 1. Jupyter notebook with narrative
# 2. README.md with project overview
# 3. Clean, commented code
# 4. 5-10 minute presentation
# 5. Handle questions
# 6. Discuss learnings
```

### Capstone Project Ideas

**Beginner-Friendly**
1. House Price Prediction (Regression)
2. Iris Classification (Classification)
3. Customer Segmentation (Clustering)
4. Titanic Survival (Classification)
5. Boston Housing (Regression)

**Intermediate**
1. Customer Churn Prediction (Binary Classification)
2. Stock Price Forecasting (Time Series)
3. Movie Recommendation (Recommender)
4. Sentiment Analysis (Text + Classification)
5. Credit Card Fraud Detection (Imbalanced Classification)

**Advanced**
1. Multi-class Problem with Custom Metrics
2. Real-world Imbalanced Dataset
3. Multiple Data Sources Integration
4. Natural Language Processing Task
5. Time Series with External Features

---

## Challenge Exercises

**C1: Model Comparison**
```python
# TODO:
# - Implement 5 different algorithms
# - Evaluate all comprehensively
# - Create comparison table
# - Visualize performance
# - Recommend best model
# - Document pros/cons of each
```

**C2: Hyperparameter Sensitivity**
```python
# TODO:
# - Train model with different hyperparameters
# - Plot performance vs each parameter
# - Identify sensitivity
# - Find optimal ranges
# - Explain why parameter matters
```

**C3: Error Analysis**
```python
# TODO:
# - Make predictions
# - Identify errors
# - Categorize error types
# - Visualize error patterns
# - Suggest improvements
# - Retrain with improvements
```

---

## Solution Hints

### Regression
```python
# Train
model = LinearRegression()
model.fit(X_train, y_train)

# Evaluate
y_pred = model.predict(X_test)
mse = mean_squared_error(y_test, y_pred)
rmse = np.sqrt(mse)
r2 = r2_score(y_test, y_pred)
```

### Classification
```python
# Train
model = LogisticRegression()
model.fit(X_train, y_train)

# Evaluate
y_pred = model.predict(X_test)
accuracy = accuracy_score(y_test, y_pred)
cm = confusion_matrix(y_test, y_pred)
print(classification_report(y_test, y_pred))
```

### Model Selection
```python
# GridSearchCV
from sklearn.model_selection import GridSearchCV

param_grid = {'C': [0.1, 1, 10], 'kernel': ['linear', 'rbf']}
grid = GridSearchCV(SVC(), param_grid, cv=5)
grid.fit(X_train, y_train)
print(grid.best_params_)
```

### Evaluation
```python
# Cross-validation
scores = cross_val_score(model, X, y, cv=5)
print(f"Mean: {scores.mean()}, Std: {scores.std()}")

# Learning curves
from sklearn.model_selection import learning_curve
train_sizes, train_scores, test_scores = learning_curve(...)
```

---

## Review Checklist

- [ ] All ML algorithm exercises completed
- [ ] Comfortable with scikit-learn
- [ ] Understand model evaluation
- [ ] Can tune hyperparameters
- [ ] Capstone project planned
- [ ] Capstone project implemented
- [ ] All phases documented
- [ ] Presentation prepared
- [ ] Ready to present!

---

## Post-Internship Resources

- Kaggle Competitions: https://www.kaggle.com/competitions
- Fast.ai: https://www.fast.ai/
- Andrew Ng's ML Course: https://www.coursera.org/learn/machine-learning
- Papers with Code: https://paperswithcode.com/
- Towards Data Science: https://towardsdatascience.com/

Congratulations on completing the internship! You're now a data scientist! 🎓🚀
