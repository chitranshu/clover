# Month 5 (Day 1–Day 30) — Deep Learning Training Mastery

_Last updated: 23 Feb 2026_

## How to use this checklist
- Target: **2 to 3 hours/day**.
- Focus this month: training stability, optimization, and experiment rigor.
- Keep strict run tracking for every experiment.

---

## Week 1 (Days 1–7): Optimization and Learning Dynamics

### Day 1
- [ ] Set up `month-5-dl-training/` project
- [ ] Define experiment naming/version rules
- [ ] Establish baseline CNN/MLP task (e.g., CIFAR-10)
- [ ] Notes: expected bottlenecks

### Day 2
- [ ] Compare optimizers: SGD, SGD+Momentum, Adam
- [ ] Fix all else equal and benchmark convergence
- [ ] Plot loss/accuracy curves per optimizer
- [ ] Summarize optimizer tradeoffs

### Day 3
- [ ] Learning rate sensitivity study
- [ ] Run LR range test
- [ ] Select initial LR candidate set
- [ ] Document unstable regions

### Day 4
- [ ] Add LR schedulers (step, cosine, one-cycle)
- [ ] Compare final validation metrics and speed
- [ ] Save scheduler vs performance table
- [ ] Notes: scheduler selection rule

### Day 5
- [ ] Gradient clipping and exploding gradient checks
- [ ] Track gradient norms during training
- [ ] Add safeguards in train loop
- [ ] Validate no degradation on stable runs

### Day 6
- [ ] Mixed precision basics (if hardware supports)
- [ ] Benchmark speed/memory vs full precision
- [ ] Validate metric parity
- [ ] Log deployment relevance

### Day 7 (Review)
- [ ] Re-run best optimization recipe from clean start
- [ ] Week summary (1 page)
- [ ] Push code + experiment report
- [ ] Update reproducibility instructions

**Week 1 Deliverable**
- [ ] Optimizer and LR strategy benchmark report

---

## Week 2 (Days 8–14): Regularization and Generalization

### Day 8
- [ ] Dropout experiments at multiple rates
- [ ] Compare train/val gap changes
- [ ] Select effective range
- [ ] Notes: under/over-regularization signals

### Day 9
- [ ] Weight decay study
- [ ] Tune weight decay with fixed LR
- [ ] Track generalization improvement
- [ ] Save best run params

### Day 10
- [ ] Data augmentation fundamentals
- [ ] Implement flips/crops/color jitter (as appropriate)
- [ ] Compare with non-augmented baseline
- [ ] Note augmentation failure cases

### Day 11
- [ ] Label smoothing and calibration checks
- [ ] Evaluate confidence quality
- [ ] Plot reliability-style summary (optional)
- [ ] Document effect on accuracy/F1

### Day 12
- [ ] Early stopping policy + checkpoint strategy
- [ ] Implement best-checkpoint restore logic
- [ ] Validate no accidental over-training
- [ ] Add run metadata capture

### Day 13
- [ ] Combine best regularization choices into one recipe
- [ ] Run ablation: remove one trick at a time
- [ ] Create ablation results table
- [ ] Summarize most impactful techniques

### Day 14 (Review)
- [ ] Reproduce best regularized run end-to-end
- [ ] Week summary (1 page)
- [ ] Push milestone
- [ ] Clean experiment artifacts

**Week 2 Deliverable**
- [ ] Generalization-focused training recipe + ablation analysis

---

## Week 3 (Days 15–21): Experiment Tracking and Error Analysis

### Day 15
- [ ] Set up experiment tracker (W&B/MLflow or markdown logs)
- [ ] Log hyperparams, metrics, artifacts
- [ ] Define mandatory fields for each run
- [ ] Notes: run hygiene checklist

### Day 16
- [ ] Implement reproducible seed + env capture
- [ ] Log package versions and hardware info
- [ ] Verify deterministic behavior where possible
- [ ] Document known nondeterminism sources

### Day 17
- [ ] Build standardized evaluation report generator
- [ ] Include class-wise metrics and confusion matrix
- [ ] Save reports per run automatically
- [ ] Validate report correctness

### Day 18
- [ ] Misclassification mining workflow
- [ ] Sample top failure categories
- [ ] Diagnose data-quality or model-blindspot causes
- [ ] Add corrective action list

### Day 19
- [ ] Perform robustness checks (noise, blur, shifts)
- [ ] Measure degradation under perturbations
- [ ] Record robustness scorecard
- [ ] Notes: practical resilience implications

### Day 20
- [ ] Package best model + inference benchmark
- [ ] Measure latency and memory footprint
- [ ] Compare against target constraints
- [ ] Draft optimization ideas

### Day 21 (Review)
- [ ] Re-run complete best experiment from config only
- [ ] Week summary (1 page)
- [ ] Push reports and scripts
- [ ] Confirm all artifacts resolve correctly

**Week 3 Deliverable**
- [ ] Full experiment tracking + deep error analysis setup

---

## Week 4 (Days 22–30): CIFAR-10 Capstone Pipeline

### Day 22
- [ ] Finalize capstone objective and acceptance criteria
- [ ] Freeze data/preprocessing pipeline
- [ ] Select 2–3 final model/training recipes
- [ ] Plan final comparison protocol

### Day 23
- [ ] Train baseline model with strict logging
- [ ] Generate full report and charts
- [ ] Validate baseline reproducibility
- [ ] Document baseline limitations

### Day 24
- [ ] Train improved recipe #1
- [ ] Compare with baseline on same protocol
- [ ] Save checkpoints and reports
- [ ] Record practical tradeoffs

### Day 25
- [ ] Train improved recipe #2 (if needed)
- [ ] Finalize best model selection
- [ ] Justify decision with metrics + constraints
- [ ] Update README results table

### Day 26
- [ ] Build inference script + batch evaluator
- [ ] Add CLI arguments and input validation
- [ ] Test on unseen sample folder
- [ ] Document usage

### Day 27
- [ ] Create end-to-end project report
- [ ] Include ablations, errors, robustness, and latency
- [ ] Add “what I’d improve next” section
- [ ] Polish visuals

### Day 28
- [ ] Reproducibility audit on clean environment
- [ ] Validate setup, training, and inference steps
- [ ] Fix docs and missing dependencies
- [ ] Final code cleanup

### Day 29
- [ ] Prepare short demo narrative (problem → approach → results)
- [ ] Optional: record 5-minute demo
- [ ] Gather one peer review
- [ ] Apply critical fixes

### Day 30 (Demo Day)
- [ ] Deliver Month 5 capstone:
  - [ ] Stable, optimized training pipeline
  - [ ] Reproducible experiments and ablations
  - [ ] Error/robustness analysis
  - [ ] Inference-ready model package
- [ ] Write Month 5 retrospective

**Month 5 Completion Criteria**
- [ ] Can tune optimization and LR schedules systematically
- [ ] Can improve generalization via regularization/augmentation
- [ ] Can run controlled ablations and error analysis
- [ ] Can produce reproducible, well-documented DL experiments

## Best Free Resources by Week
- **Week 1 (Optimization + LR):**
  - CS231n optimization: https://cs231n.github.io/neural-networks-3/
  - fast.ai course (free): https://course.fast.ai/
- **Week 2 (Regularization + Generalization):**
  - CS231n regularization notes: https://cs231n.github.io/neural-networks-2/
  - Albumentations docs: https://albumentations.ai/docs/
- **Week 3 (Experiment Tracking + Analysis):**
  - Weights & Biases docs: https://docs.wandb.ai/
  - MLflow tracking docs: https://mlflow.org/docs/latest/tracking.html
- **Week 4 (CIFAR Capstone):**
  - CIFAR dataset page: https://www.cs.toronto.edu/~kriz/cifar.html
  - Papers With Code CIFAR-10 leaderboard: https://paperswithcode.com/sota/image-classification-on-cifar-10

## After Month 5
Continue with Month 6 in [learning-path/001-learning-path.md](learning-path/001-learning-path.md): computer vision core and transfer learning.
