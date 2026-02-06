# Week 10-12: Machine Learning & Capstone Project

## Overview
The final three weeks focus on machine learning algorithms, model evaluation, and building a comprehensive capstone project. You'll apply all previous knowledge to solve real-world problems and build a portfolio-worthy project.

## Learning Objectives
By the end of these weeks, you should be able to:
- [ ] Understand regression problems and solutions
- [ ] Apply logistic regression for classification
- [ ] Use ensemble methods (Random Forests, etc.)
- [ ] Implement clustering algorithms
- [ ] Apply dimensionality reduction techniques
- [ ] Build recommender systems
- [ ] Perform natural language processing
- [ ] Evaluate models comprehensively
- [ ] Build end-to-end ML pipelines
- [ ] Present and defend your capstone project

## Weekly Schedule

### Week 10: Regression & Classification

**Monday - Linear Regression Fundamentals**
- Study: Linear regression theory
- Study: Cost functions and optimization
- Study: Multiple and polynomial regression
- Practice: Regression exercises
- Time: 3 hours

**Tuesday - Linear Regression Advanced**
- Study: Feature scaling and normalization
- Study: Regularization (Ridge, Lasso)
- Study: Model evaluation metrics
- Practice: Advanced regression
- Time: 3 hours

**Wednesday - Logistic Regression**
- Study: Classification fundamentals
- Study: Logistic regression theory
- Study: Decision boundaries
- Study: Classification metrics (precision, recall, F1)
- Practice: Classification exercises
- Time: 3 hours

**Thursday - K-Nearest Neighbors**
- Study: KNN algorithm
- Study: Distance metrics
- Study: Finding optimal K
- Practice: KNN exercises
- Time: 3 hours

**Friday - Model Comparison & Integration**
- Review regression and classification
- Compare models and metrics
- Integration exercises
- Prepare for Week 11
- Time: 2 hours

### Week 11: Ensemble Methods & Unsupervised Learning

**Monday - Decision Trees & Random Forests**
- Study: Decision tree fundamentals
- Study: Splitting criteria and pruning
- Study: Random forests and bagging
- Study: Feature importance
- Practice: Tree-based models exercises
- Time: 3 hours

**Tuesday - Support Vector Machines**
- Study: SVM fundamentals
- Study: Kernel tricks
- Study: Hyperparameter tuning
- Practice: SVM exercises
- Time: 3 hours

**Wednesday - K-Means Clustering**
- Study: Unsupervised learning concepts
- Study: K-Means algorithm
- Study: Finding optimal K
- Study: Clustering evaluation
- Practice: Clustering exercises
- Time: 3 hours

**Thursday - Principal Component Analysis & Advanced Topics**
- Study: PCA fundamentals
- Study: Dimensionality reduction
- Study: Feature selection
- Study: Model selection and hyperparameter tuning
- Practice: PCA and feature selection
- Time: 3 hours

**Friday - Advanced Techniques**
- Study: Recommender systems basics
- Study: NLP fundamentals
- Study: Text preprocessing
- Integration exercises
- Time: 2 hours

### Week 12: Capstone Project & Presentation

**Monday-Wednesday - Capstone Project Development**
- Finalize project topic and dataset
- Perform exploratory data analysis
- Preprocess and clean data
- Begin model development
- Time: 4-5 hours/day

**Thursday - Model Refinement & Evaluation**
- Compare multiple models
- Tune hyperparameters
- Evaluate comprehensively
- Document findings
- Time: 4 hours

**Friday - Project Presentation & Reflection**
- Create presentation and visualizations
- Practice presentation
- Present to team/mentor
- Reflection and feedback
- Time: 3 hours

## Key Concepts to Master

### Linear Regression
```python
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_squared_error, r2_score

# Create and train model
model = LinearRegression()
model.fit(X_train, y_train)

# Predict and evaluate
y_pred = model.predict(X_test)
rmse = np.sqrt(mean_squared_error(y_test, y_pred))
r2 = r2_score(y_test, y_pred)
```

### Logistic Regression
```python
from sklearn.linear_model import LogisticRegression
from sklearn.metrics import confusion_matrix, classification_report

# Create and train
model = LogisticRegression()
model.fit(X_train, y_train)

# Evaluate
y_pred = model.predict(X_test)
print(classification_report(y_test, y_pred))
```

### Random Forests
```python
from sklearn.ensemble import RandomForestClassifier

# Create and train
rf = RandomForestClassifier(n_estimators=100, max_depth=10)
rf.fit(X_train, y_train)

# Feature importance
importances = rf.feature_importances_
feature_importance_df = pd.DataFrame({
    'Feature': X.columns,
    'Importance': importances
}).sort_values('Importance', ascending=False)
```

### K-Means Clustering
```python
from sklearn.cluster import KMeans
from sklearn.preprocessing import StandardScaler

# Scale and cluster
scaler = StandardScaler()
X_scaled = scaler.fit_transform(X)

kmeans = KMeans(n_clusters=3, random_state=42)
clusters = kmeans.fit_predict(X_scaled)

# Find elbow point
inertias = []
for k in range(1, 11):
    kmeans = KMeans(n_clusters=k)
    kmeans.fit(X_scaled)
    inertias.append(kmeans.inertia_)
```

### PCA
```python
from sklearn.decomposition import PCA

# Apply PCA
pca = PCA(n_components=2)
X_pca = pca.fit_transform(X_scaled)

# Explained variance
print(f"Explained variance: {pca.explained_variance_ratio_}")
print(f"Total: {pca.explained_variance_ratio_.sum()}")
```

## Study Materials

### Primary Resources
1. `11-Linear-Regression/` - Regression notebooks
2. `13-Logistic-Regression/` - Classification notebooks
3. `14-K-Nearest-Neighbors/` - KNN notebooks
4. `15-Decision-Trees-and-Random-Forests/` - Tree-based models
5. `16-Support-Vector-Machines/` - SVM notebooks
6. `17-K-Means-Clustering/` - Clustering notebooks
7. `18-Principal-Component-Analysis/` - PCA notebooks
8. `19-Recommender-Systems/` - Recommender systems
9. `20-Natural-Language-Processing/` - NLP notebooks
10. `10-Data-Capstone-Projects/` - Capstone examples

## Daily Practice Routine (Weeks 10-11)

```
Morning (1.5 hours):
- Review algorithm theory
- Study mathematical foundations

Active Study (2.5 hours):
- Read notebook examples
- Code along with implementations
- Understand hyperparameters

Afternoon (2 hours):
- Complete exercises
- Experiment with different parameters
- Compare models

Evening (30 min):
- Summarize algorithm
- Create reference sheet
- Note advantages/disadvantages
```

## Daily Routine (Week 12 - Capstone)

```
Morning (2 hours):
- Project work on assigned task
- Data exploration/processing

Midday (2 hours):
- Model development
- Testing and refinement

Afternoon (1.5 hours):
- Documentation
- Visualization creation
- Results analysis

Evening (1 hour):
- Plan next day
- Update project progress
- Organize findings
```

## Exercises to Complete

### Week 10 Exercises
- [ ] Linear regression on multiple datasets
- [ ] Polynomial regression comparison
- [ ] Regularization parameter tuning
- [ ] Logistic regression classification
- [ ] Classification metrics interpretation
- [ ] KNN with different K values
- [ ] Model comparison exercise

### Week 11 Exercises
- [ ] Decision tree visualization
- [ ] Random forest feature importance
- [ ] SVM with different kernels
- [ ] K-Means with elbow method
- [ ] PCA variance analysis
- [ ] Recommender system basics
- [ ] NLP text preprocessing

### Week 12 Project
- [ ] Exploratory data analysis
- [ ] Data preprocessing
- [ ] Feature engineering
- [ ] Model selection and training
- [ ] Hyperparameter optimization
- [ ] Model evaluation
- [ ] Results visualization
- [ ] Documentation and presentation

## Machine Learning Algorithm Selection Guide

| Problem Type | Algorithms to Consider |
|-------------|------------------------|
| **Regression** | Linear Regression, Polynomial Regression, Ridge/Lasso, Random Forest, SVM |
| **Classification** | Logistic Regression, KNN, Decision Trees, Random Forests, SVM, Naive Bayes |
| **Clustering** | K-Means, Hierarchical, DBSCAN, Gaussian Mixture Models |
| **Dimensionality Reduction** | PCA, t-SNE, Autoencoders |
| **Recommendation** | Collaborative Filtering, Content-based, Hybrid |
| **Text Analysis** | TF-IDF, Word2Vec, LSTM, BERT |

## Capstone Project Requirements

Your capstone project should include:

### 1. Problem Definition
- [ ] Clear problem statement
- [ ] Business context
- [ ] Success metrics defined

### 2. Data Exploration
- [ ] Dataset overview (shape, types)
- [ ] Statistical summaries
- [ ] Missing value analysis
- [ ] Distribution visualizations
- [ ] Correlation analysis

### 3. Data Preprocessing
- [ ] Missing value handling
- [ ] Outlier treatment
- [ ] Feature scaling/normalization
- [ ] Encoding categorical variables
- [ ] Feature engineering

### 4. Model Development
- [ ] Train/test split (or cross-validation)
- [ ] Try multiple algorithms
- [ ] Hyperparameter tuning
- [ ] Handle class imbalance (if applicable)
- [ ] Cross-validation strategy

### 5. Model Evaluation
- [ ] Multiple metrics relevant to problem
- [ ] Confusion matrix (for classification)
- [ ] ROC-AUC curves (for classification)
- [ ] Feature importance analysis
- [ ] Error analysis

### 6. Results & Visualization
- [ ] Key findings visualization
- [ ] Model comparison plots
- [ ] Prediction examples
- [ ] Feature importance charts
- [ ] Business impact quantification

### 7. Documentation & Presentation
- [ ] Clear README
- [ ] Jupyter notebook with narrative
- [ ] Professional visualizations
- [ ] 5-10 minute presentation
- [ ] Recommendations and next steps

## Example Capstone Topics

### Structured Data
- **House Price Prediction** - Regression on real estate data
- **Customer Churn Prediction** - Classification with business impact
- **Loan Default Detection** - Classification with cost considerations
- **Sales Forecasting** - Time series forecasting
- **Customer Segmentation** - Clustering for marketing

### Text Data
- **Sentiment Analysis** - Classify reviews as positive/negative
- **Topic Modeling** - Discover topics in documents
- **Text Classification** - Categorize documents
- **Named Entity Recognition** - Extract entities from text

### Mixed Data
- **Movie Recommendation System** - Recommender with ratings
- **Credit Card Fraud Detection** - Imbalanced classification
- **Restaurant Recommendation** - Content-based recommendation
- **Job Recommendation** - Collaborative filtering

## Model Evaluation Checklist

### Regression Models
- [ ] Mean Squared Error (MSE)
- [ ] Root Mean Squared Error (RMSE)
- [ ] Mean Absolute Error (MAE)
- [ ] R² Score
- [ ] Residual analysis
- [ ] Predictions vs. Actual plot

### Classification Models
- [ ] Accuracy
- [ ] Precision
- [ ] Recall
- [ ] F1 Score
- [ ] Confusion Matrix
- [ ] ROC-AUC Curve
- [ ] Precision-Recall Curve
- [ ] Cross-validation scores

### General
- [ ] Train vs. Test performance
- [ ] Evidence of overfitting/underfitting
- [ ] Feature importance
- [ ] Model interpretability
- [ ] Computational efficiency

## Common ML Pitfalls

1. **Data Leakage** - Features contain info about target
2. **Overfitting** - Model memorizes training data
3. **Underfitting** - Model too simple for data
4. **Class Imbalance** - Not enough minority class examples
5. **Feature Scaling** - Forgetting to scale for distance-based models
6. **Train/Test Contamination** - Fitting scaler on all data
7. **Hyperparameter Tuning on Test Set** - Use validation set instead
8. **Ignoring Baseline** - Compare to simple baseline model

## Resources

### Documentation
- Scikit-learn: https://scikit-learn.org/stable/
- TensorFlow/Keras: https://www.tensorflow.org/
- XGBoost: https://xgboost.readthedocs.io/

### Learning Resources
- Fast.ai: https://www.fast.ai/
- Andrew Ng's ML Course: https://www.coursera.org/learn/machine-learning
- Kaggle Competitions: https://www.kaggle.com/competitions
- Machine Learning Mastery: https://machinelearningmastery.com/

## Presentation Tips

### Structure
1. **Problem** (1-2 min) - What problem are you solving?
2. **Data** (1 min) - What data did you use?
3. **Methods** (2 min) - What approaches did you try?
4. **Results** (3-4 min) - What did you find?
5. **Conclusions** (1 min) - What are recommendations?

### Visuals
- Use consistent color schemes
- Include relevant plots/charts
- Show model performance comparisons
- Highlight key insights
- Keep slides uncluttered

### Practice
- Time your presentation
- Practice with an audience
- Anticipate questions
- Have backup slides with details
- Know your project deeply

## Checklist Before Graduation

- [ ] Completed all ML algorithm exercises
- [ ] Comfortable with scikit-learn
- [ ] Understand model evaluation thoroughly
- [ ] Completed comprehensive capstone project
- [ ] Can explain ML concepts clearly
- [ ] Built portfolio with capstone project
- [ ] Presented findings professionally
- [ ] Documented code well

## Tips for Success in Week 12

1. **Start Early** - Don't wait until Friday
2. **Keep It Focused** - Solve one problem well
3. **Iterate** - Try multiple approaches
4. **Document Process** - Show your thinking
5. **Tell Story** - Connect data to insights
6. **Get Feedback** - Present to others early
7. **Polish** - Make presentation professional

## Post-Internship Next Steps

After completing this internship:
1. **Build Portfolio** - Add capstone to GitHub
2. **Learn Advanced Topics** - Deep learning, advanced NLP
3. **Practice Continuously** - Kaggle competitions
4. **Read Research** - Stay current with techniques
5. **Teach Others** - Blog about learnings
6. **Network** - Connect with data science community

Congratulations on completing the 12-week internship! You've built strong foundations in data science and are ready for real-world projects! 🎊

---

## Internship Completion Certificate

By completing this internship, you have demonstrated:
- ✅ Python programming proficiency
- ✅ NumPy array manipulation skills
- ✅ Pandas data wrangling expertise
- ✅ Data visualization capabilities
- ✅ Machine learning model building
- ✅ Project management and documentation
- ✅ Professional communication skills

**You are now prepared for:**
- Entry-level Data Science roles
- Data Analysis positions
- ML Engineer positions
- Advanced coursework in AI/ML
- Specialized domain applications

Good luck on your data science journey! 🚀
