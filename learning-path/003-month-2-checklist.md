# Month 2 (Day 1–Day 30) — Classical Machine Learning Daily Checklist

_Last updated: 23 Feb 2026_

## How to use this checklist
- Target: **1.5 to 2.5 hours/day**.
- Daily structure:
  - **45–60 min** concept learning
  - **45–60 min** coding/experiments
  - **15–30 min** notes + recap
- Mark tasks as done: `[ ]` → `[x]`.

---

## Week 1 (Days 1–7): Data Preprocessing + Pipeline Basics

### Day 1
- [ ] Set up `month-2-ml/` project folder with `data`, `notebooks`, `src`
- [ ] Install and verify `scikit-learn`, `pandas`, `numpy`, `matplotlib`, `seaborn`
- [ ] Pick one tabular dataset (e.g., Titanic, housing, churn)
- [ ] Load dataset and inspect shape, columns, dtypes
- [ ] Notes: define target variable and problem type

### Day 2
- [ ] Handle missing values (`SimpleImputer`, `fillna`, `dropna`)
- [ ] Identify numerical vs categorical columns
- [ ] Build preprocessing baseline notebook
- [ ] Document assumptions for missing-data strategy

### Day 3
- [ ] Encode categorical features (OneHotEncoder, ordinal encoding basics)
- [ ] Compare manual encoding vs sklearn transformers
- [ ] Save a clean feature table artifact (`processed_v1.csv`)
- [ ] Notes: when one-hot is not ideal

### Day 4
- [ ] Feature scaling (StandardScaler, MinMaxScaler)
- [ ] Compare model behavior with and without scaling
- [ ] Visualize distribution changes before/after scaling
- [ ] Notes: which models need scaling most

### Day 5
- [ ] Train/validation/test split strategy
- [ ] Stratified split for classification datasets
- [ ] Explain and detect data leakage with examples
- [ ] Write a checklist: “No leakage” rules

### Day 6
- [ ] Build first reusable sklearn `Pipeline`
- [ ] Add `ColumnTransformer` for mixed feature types
- [ ] Fit baseline model (logistic or linear regression)
- [ ] Save metrics in `results/baseline_metrics.md`

### Day 7 (Review Day)
- [ ] Rebuild preprocessing + baseline from scratch
- [ ] Clean project structure and file naming
- [ ] Week summary (1 page)
- [ ] Push progress to GitHub

**Week 1 Deliverable**
- [ ] One clean preprocessing pipeline with baseline model

---

## Week 2 (Days 8–14): Regression + Classification Fundamentals

### Day 8
- [ ] Linear regression intuition and assumptions
- [ ] Train baseline linear model on regression dataset
- [ ] Evaluate with MAE, MSE, RMSE, $R^2$
- [ ] Notes: metric interpretation in plain language

### Day 9
- [ ] Logistic regression intuition (classification)
- [ ] Train logistic regression on classification dataset
- [ ] Evaluate accuracy, precision, recall, F1
- [ ] Plot confusion matrix

### Day 10
- [ ] Decision tree concepts (splits, depth, impurity)
- [ ] Train decision tree classifier/regressor
- [ ] Compare performance vs linear/logistic model
- [ ] Notes: overfitting signs in trees

### Day 11
- [ ] Random forest intuition and bagging
- [ ] Train random forest with basic hyperparameters
- [ ] Analyze feature importances
- [ ] Save side-by-side model comparison table

### Day 12
- [ ] Intro gradient boosting concepts
- [ ] Train `GradientBoosting` or `XGBoost` (if available)
- [ ] Compare with random forest results
- [ ] Notes: when boosting usually wins

### Day 13
- [ ] Build unified evaluation function for all models
- [ ] Standardize metric logging format
- [ ] Create model leaderboard markdown
- [ ] Add quick error analysis section

### Day 14 (Review Day)
- [ ] Repeat training of 3 models end-to-end
- [ ] Verify reproducibility with fixed random seeds
- [ ] Week summary (1 page)
- [ ] Publish model comparison chart

**Week 2 Deliverable**
- [ ] Model leaderboard with at least 4 algorithms

---

## Week 3 (Days 15–21): Validation, Regularization, and Tuning

### Day 15
- [ ] Cross-validation fundamentals (`KFold`, `StratifiedKFold`)
- [ ] Replace single split evaluation with CV
- [ ] Report mean ± std of key metrics
- [ ] Notes: why single split can mislead

### Day 16
- [ ] Bias-variance tradeoff intuition
- [ ] Diagnose underfitting vs overfitting from learning curves
- [ ] Plot training vs validation performance
- [ ] Write model improvement hypotheses

### Day 17
- [ ] Regularization basics (L1/L2)
- [ ] Try ridge/lasso (or regularized logistic regression)
- [ ] Compare coefficient shrinkage behavior
- [ ] Notes: sparse features and L1

### Day 18
- [ ] Hyperparameter tuning with `GridSearchCV`
- [ ] Tune one baseline model carefully
- [ ] Save best parameters and CV score
- [ ] Track search space and runtime

### Day 19
- [ ] Hyperparameter tuning with `RandomizedSearchCV`
- [ ] Compare search efficiency vs grid search
- [ ] Add runtime/performance tradeoff notes
- [ ] Update leaderboard with tuned models

### Day 20
- [ ] Calibration and threshold tuning (classification)
- [ ] Plot ROC curve and PR curve
- [ ] Choose threshold based on precision/recall needs
- [ ] Notes: business impact of threshold changes

### Day 21 (Review Day)
- [ ] Re-run best tuned pipeline from clean start
- [ ] Validate no leakage/no target contamination
- [ ] Week summary (1 page)
- [ ] Push polished notebooks/scripts

**Week 3 Deliverable**
- [ ] Tuned model pipeline with CV-based evaluation

---

## Week 4 (Days 22–30): Mini Capstone — End-to-End ML Project

### Day 22
- [ ] Select final Month 2 dataset/problem statement
- [ ] Define objective metric and acceptance target
- [ ] Draft project plan (scope, risks, assumptions)
- [ ] Create `README` skeleton for capstone

### Day 23
- [ ] Build data ingestion + preprocessing module (`src/data.py`)
- [ ] Add reproducible random state config
- [ ] Save processed train/val/test artifacts
- [ ] Notes: dataset quality issues encountered

### Day 24
- [ ] Implement baseline models (`src/train_baselines.py`)
- [ ] Run and log all baseline metrics
- [ ] Identify top 2 candidates for tuning
- [ ] Update project README with early results

### Day 25
- [ ] Tune top models with CV search
- [ ] Add feature importance/permutation importance analysis
- [ ] Document which features drive outcomes
- [ ] Save best model artifact (`models/best.pkl`)

### Day 26
- [ ] Error analysis deep dive
- [ ] Slice-based analysis (where model fails most)
- [ ] Add practical mitigation ideas
- [ ] Document ethical/bias risks in your dataset

### Day 27
- [ ] Build simple inference script (`src/predict.py`)
- [ ] Test on unseen examples
- [ ] Add usage instructions to README
- [ ] Confirm reproducibility from fresh environment

### Day 28
- [ ] Create visual report: metrics, confusion matrix/curves, key charts
- [ ] Finalize experiment log table
- [ ] Add “lessons learned” section
- [ ] Review code quality and folder hygiene

### Day 29
- [ ] Prepare final presentation summary (1–2 pages)
- [ ] Record short walkthrough (optional)
- [ ] Publish final repo updates
- [ ] Ask for one peer review (optional)

### Day 30 (Month-End Demo Day)
- [ ] Deliver **End-to-End Classical ML Project**
  - [ ] Clean data pipeline
  - [ ] Baseline + tuned model comparison
  - [ ] Proper validation and metrics
  - [ ] Inference script + reproducibility instructions
- [ ] Write Month 2 retrospective (wins, gaps, next focus)

**Week 4 Deliverable**
- [ ] Completed capstone-quality classical ML project

---

## Month 2 Completion Criteria
- [ ] You trained and compared at least 4 ML algorithms.
- [ ] You implemented a sklearn preprocessing pipeline.
- [ ] You used cross-validation and at least one tuning strategy.
- [ ] You produced a reproducible end-to-end ML project.
- [ ] You can explain metric tradeoffs and model selection rationale.

## Best Free Resources by Week
- **Week 1 (Preprocessing + Pipelines):**
  - Scikit-learn preprocessing: https://scikit-learn.org/stable/modules/preprocessing.html
  - Scikit-learn pipelines: https://scikit-learn.org/stable/modules/compose.html
- **Week 2 (Regression + Classification):**
  - Scikit-learn supervised learning: https://scikit-learn.org/stable/supervised_learning.html
  - Google ML Crash Course: https://developers.google.com/machine-learning/crash-course
- **Week 3 (Validation + Tuning):**
  - Model selection and CV: https://scikit-learn.org/stable/modules/cross_validation.html
  - Hyperparameter tuning: https://scikit-learn.org/stable/modules/grid_search.html
- **Week 4 (End-to-End Mini Capstone):**
  - Kaggle Learn (free micro-courses): https://www.kaggle.com/learn
  - Cookiecutter Data Science (project structure): https://cookiecutter-data-science.drivendata.org/

## After Month 2
Move to Month 3 in [learning-path/001-learning-path.md](learning-path/001-learning-path.md) and focus on intermediate ML, feature engineering, and stronger experimentation discipline.