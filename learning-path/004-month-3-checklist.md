# Month 3 (Day 1–Day 30) — Intermediate ML + Experimentation Daily Checklist

_Last updated: 23 Feb 2026_

## How to use this checklist
- Target: **1.5 to 2.5 hours/day**.
- Daily pattern: learn → implement → evaluate → note.
- Mark progress: `[ ]` to `[x]`.

---

## Week 1 (Days 1–7): Feature Engineering + Leakage Control

### Day 1
- [ ] Set up `month-3-intermediate-ml/` project structure
- [ ] Define objective metric + business constraints
- [ ] Add experiment log template (`run_id`, params, metrics)
- [ ] Notes: baseline risks and leakage sources

### Day 2
- [ ] Create numeric feature transforms (log/binning/interactions)
- [ ] Compare transformed vs raw feature performance
- [ ] Save feature dictionary markdown
- [ ] Notes: explain each engineered feature intuition

### Day 3
- [ ] Build categorical encoding variants (one-hot/target/frequency)
- [ ] Validate encodings inside CV only (no leakage)
- [ ] Compare performance across encoders
- [ ] Record tradeoffs in log

### Day 4
- [ ] Time/date feature extraction (if applicable)
- [ ] Build robust train/validation split strategy
- [ ] Add leakage guard checklist to README
- [ ] Notes: what not to include before split

### Day 5
- [ ] Feature selection methods (filter/wrapper/model-based)
- [ ] Try permutation importance
- [ ] Remove low-value features and re-evaluate
- [ ] Save before/after metrics table

### Day 6
- [ ] Add pipeline tests for preprocessing consistency
- [ ] Ensure identical transforms in train and inference
- [ ] Run reproducibility check with fixed seeds
- [ ] Notes: top failure points found

### Day 7 (Review)
- [ ] Rebuild full feature pipeline from scratch
- [ ] Clean scripts/notebooks and folder naming
- [ ] Week summary (1 page)
- [ ] Push tagged milestone to GitHub

**Week 1 Deliverable**
- [ ] Robust feature engineering pipeline with leakage controls

---

## Week 2 (Days 8–14): Ensemble Methods + Better Evaluation

### Day 8
- [ ] Review random forest internals
- [ ] Tune depth, estimators, min samples
- [ ] Capture train vs validation gap
- [ ] Notes: variance reduction behavior

### Day 9
- [ ] Gradient boosting fundamentals
- [ ] Train `GradientBoosting` baseline
- [ ] Compare to random forest on same split/CV
- [ ] Log runtime and metric differences

### Day 10
- [ ] Introduce `XGBoost` or `LightGBM` (if available)
- [ ] Train with conservative default settings
- [ ] Evaluate calibration + robustness
- [ ] Notes: handling missing values behavior

### Day 11
- [ ] Advanced metrics: ROC-AUC, PR-AUC, balanced accuracy
- [ ] Pick metric aligned to objective
- [ ] Build unified metrics report generator
- [ ] Save leaderboard markdown

### Day 12
- [ ] Error analysis by slices (segment/category/time)
- [ ] Identify worst-performing cohorts
- [ ] Write mitigation actions
- [ ] Add fairness note section

### Day 13
- [ ] Model explainability with SHAP (or permutation fallback)
- [ ] Generate top feature explanation plots
- [ ] Validate explanations against domain intuition
- [ ] Notes: suspicious explanations to investigate

### Day 14 (Review)
- [ ] Re-run top 3 ensemble models from clean state
- [ ] Confirm deterministic results with fixed seeds
- [ ] Week summary (1 page)
- [ ] Publish updated leaderboard

**Week 2 Deliverable**
- [ ] Ensemble model benchmark + error analysis report

---

## Week 3 (Days 15–21): Hyperparameter Optimization + Experiment Tracking

### Day 15
- [ ] Define tuning search spaces carefully
- [ ] Use `RandomizedSearchCV` for fast exploration
- [ ] Log each run in experiment sheet
- [ ] Notes: why each range was chosen

### Day 16
- [ ] Use `Optuna` (or equivalent) for Bayesian-style search
- [ ] Compare efficiency vs random/grid search
- [ ] Keep search budget fixed for fairness
- [ ] Save best-trial summary

### Day 17
- [ ] Add early stopping where supported
- [ ] Track overfitting during tuning
- [ ] Plot metric vs trial number
- [ ] Notes: diminishing returns point

### Day 18
- [ ] Stress-test model on perturbed validation data
- [ ] Evaluate stability under feature noise
- [ ] Record robustness score
- [ ] Add recommendations section

### Day 19
- [ ] Build reusable training CLI/config file
- [ ] Externalize hyperparameters into config
- [ ] Save model + metadata artifacts
- [ ] Notes: reproducibility checklist

### Day 20
- [ ] Compare untuned vs tuned vs robust models
- [ ] Produce final selection rationale
- [ ] Update README with final chosen model
- [ ] Prepare charts for final presentation

### Day 21 (Review)
- [ ] Run full pipeline from fresh environment
- [ ] Verify artifact paths and versioning
- [ ] Week summary (1 page)
- [ ] Push release tag

**Week 3 Deliverable**
- [ ] Tuned, reproducible, and robust model package

---

## Week 4 (Days 22–30): Mini Capstone — Intermediate ML Production-Ready Baseline

### Day 22
- [ ] Select final dataset/problem for Month 3 capstone
- [ ] Define success criteria and non-goals
- [ ] Draft architecture flow (data → model → report)
- [ ] Create final README skeleton

### Day 23
- [ ] Implement clean data/preprocessing modules
- [ ] Add train/val/test orchestration scripts
- [ ] Save all artifacts under versioned folders
- [ ] Document dataset assumptions

### Day 24
- [ ] Train baselines + ensembles + tuned candidate
- [ ] Generate unified metrics dashboard notebook
- [ ] Validate against leakage checklist
- [ ] Update results section

### Day 25
- [ ] Complete explainability + slice analysis section
- [ ] Add model risk and limitation section
- [ ] Propose next improvements
- [ ] Finalize experiment logs

### Day 26
- [ ] Build inference script for single/batch prediction
- [ ] Add input validation and error messages
- [ ] Test with unseen examples
- [ ] Document usage examples

### Day 27
- [ ] Package project for reproducibility (`requirements`, config)
- [ ] Verify run instructions on clean clone
- [ ] Polish code style and folder hygiene
- [ ] Add architecture diagram (optional)

### Day 28
- [ ] Create final report (problem, methods, results, risks)
- [ ] Add key visualizations and insights
- [ ] Write lessons learned section
- [ ] Prepare short demo outline

### Day 29
- [ ] Record or rehearse 5-minute project walkthrough
- [ ] Gather feedback from one peer (optional)
- [ ] Incorporate critical fixes
- [ ] Final repo cleanup

### Day 30 (Demo Day)
- [ ] Deliver Month 3 capstone:
  - [ ] End-to-end reproducible ML pipeline
  - [ ] Strong evaluation + explainability
  - [ ] Inference-ready script
  - [ ] Documented limitations and next steps
- [ ] Write Month 3 retrospective

**Month 3 Completion Criteria**
- [ ] Strong feature engineering with leakage-safe validation
- [ ] Ensemble/tuned model selection with rationale
- [ ] Reproducible training + inference pipeline
- [ ] Structured experiment tracking and error analysis

## Best Free Resources by Week
- **Week 1 (Feature Engineering + Leakage):**
  - Kaggle Feature Engineering: https://www.kaggle.com/learn/feature-engineering
  - Scikit-learn common pitfalls (leakage): https://scikit-learn.org/stable/common_pitfalls.html
- **Week 2 (Ensembles + Evaluation):**
  - Scikit-learn ensembles: https://scikit-learn.org/stable/modules/ensemble.html
  - XGBoost docs: https://xgboost.readthedocs.io/en/stable/
- **Week 3 (Optimization + Tracking):**
  - Optuna docs: https://optuna.org/
  - MLflow docs: https://mlflow.org/docs/latest/index.html
- **Week 4 (Capstone Packaging):**
  - Cookiecutter Data Science: https://cookiecutter-data-science.drivendata.org/
  - Kaggle notebooks for reporting ideas: https://www.kaggle.com/code

## After Month 3
Continue with Month 4 in [learning-path/001-learning-path.md](learning-path/001-learning-path.md): neural networks from scratch + PyTorch basics.
