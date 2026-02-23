# Month 4 (Day 1–Day 30) — Neural Networks from Scratch + PyTorch Basics

_Last updated: 23 Feb 2026_

## How to use this checklist
- Target: **1.5 to 3 hours/day**.
- Focus split: **50% concepts + 50% implementation**.
- Keep one notebook for derivations and one script folder for clean code.

---

## Week 1 (Days 1–7): Perceptron, MLP, and Core Building Blocks

### Day 1
- [ ] Create `month-4-neural-nets/` project structure
- [ ] Review neuron/perceptron intuition
- [ ] Implement single perceptron for AND/OR gates
- [ ] Notes: linear separability intuition

### Day 2
- [ ] Activation functions (sigmoid, tanh, ReLU)
- [ ] Plot activation and gradient curves
- [ ] Compare vanishing gradient tendencies
- [ ] Notes: when to use ReLU variants

### Day 3
- [ ] Loss functions (MSE, BCE, Cross-Entropy)
- [ ] Implement each loss from scratch in Numpy
- [ ] Validate loss values on toy predictions
- [ ] Write formula cheatsheet

### Day 4
- [ ] Build 2-layer MLP forward pass in Numpy
- [ ] Verify tensor dimensions at each step
- [ ] Add unit tests for shape consistency
- [ ] Notes: common shape bugs

### Day 5
- [ ] Introduce parameter initialization strategies
- [ ] Compare random vs Xavier/He init behavior
- [ ] Run quick convergence experiments
- [ ] Log observations

### Day 6
- [ ] Implement mini-batch processing logic
- [ ] Shuffle data and iterate batches correctly
- [ ] Track batch vs epoch metrics
- [ ] Notes: batch size effect

### Day 7 (Review)
- [ ] Rebuild forward-only MLP from scratch
- [ ] Consolidate Week 1 notes and formulas
- [ ] Push code + notebook updates
- [ ] Week summary (1 page)

**Week 1 Deliverable**
- [ ] Working Numpy forward-pass MLP scaffold

---

## Week 2 (Days 8–14): Backpropagation + Training Loop from Scratch

### Day 8
- [ ] Derive backprop for one linear layer
- [ ] Implement manual gradients in Numpy
- [ ] Numerical gradient check for correctness
- [ ] Notes: chain rule in code terms

### Day 9
- [ ] Extend backprop to two-layer MLP
- [ ] Validate gradients layer by layer
- [ ] Fix gradient sign/magnitude issues
- [ ] Add gradient debug prints/plots

### Day 10
- [ ] Implement SGD optimizer from scratch
- [ ] Add learning rate parameterization
- [ ] Train on toy dataset and monitor loss
- [ ] Save training curve plot

### Day 11
- [ ] Add momentum and compare with plain SGD
- [ ] Track convergence speed differences
- [ ] Evaluate stability across learning rates
- [ ] Notes: optimizer behavior patterns

### Day 12
- [ ] Add regularization (L2) and observe generalization
- [ ] Split train/val and monitor both losses
- [ ] Document overfitting symptoms
- [ ] Save best checkpoint by val loss

### Day 13
- [ ] Build clean reusable training loop API
- [ ] Add metric logger and checkpoint saver
- [ ] Refactor code into modular files
- [ ] Improve docstrings/README

### Day 14 (Review)
- [ ] Train MLP end-to-end from scratch on simple dataset
- [ ] Verify reproducibility with fixed seed
- [ ] Week summary (1 page)
- [ ] Push milestone tag

**Week 2 Deliverable**
- [ ] End-to-end Numpy MLP with backprop + optimizer

---

## Week 3 (Days 15–21): PyTorch Fundamentals

### Day 15
- [ ] PyTorch tensor basics and autograd
- [ ] Recreate small Numpy ops in PyTorch
- [ ] Inspect computation graph behavior
- [ ] Notes: what autograd automates

### Day 16
- [ ] Build same MLP in `torch.nn.Module`
- [ ] Implement forward method cleanly
- [ ] Use `DataLoader` for batching
- [ ] Validate outputs and shapes

### Day 17
- [ ] Write standard train/val loop in PyTorch
- [ ] Add optimizer + scheduler basics
- [ ] Track loss and accuracy per epoch
- [ ] Save best model checkpoint

### Day 18
- [ ] Add dropout and batch normalization
- [ ] Compare with/without regularization
- [ ] Plot train/val curves for each variant
- [ ] Notes: generalization impact

### Day 19
- [ ] Build evaluation script with confusion matrix
- [ ] Add precision/recall/F1 reporting
- [ ] Handle model loading for inference
- [ ] Write usage examples

### Day 20
- [ ] Compare Numpy vs PyTorch implementation quality
- [ ] Document speed, clarity, and maintenance differences
- [ ] Finalize PyTorch project structure
- [ ] Update README

### Day 21 (Review)
- [ ] Re-run PyTorch training from clean environment
- [ ] Confirm reproducibility + artifact paths
- [ ] Week summary (1 page)
- [ ] Push polished code

**Week 3 Deliverable**
- [ ] Reproducible PyTorch MLP training project

---

## Week 4 (Days 22–30): MNIST Capstone (Scratch + PyTorch)

### Day 22
- [ ] Prepare MNIST pipeline (download/load/split)
- [ ] Define baseline metrics and success target
- [ ] Implement simple preprocessing
- [ ] Add run configuration file

### Day 23
- [ ] Train Numpy MLP baseline on reduced subset
- [ ] Record performance + runtime
- [ ] Identify bottlenecks and failure cases
- [ ] Log observations

### Day 24
- [ ] Train PyTorch MLP on full dataset
- [ ] Tune hidden size, LR, batch size
- [ ] Save best model + metrics
- [ ] Plot learning curves

### Day 25
- [ ] Evaluate on test set and per-class performance
- [ ] Generate confusion matrix
- [ ] Compare errors across classes
- [ ] Document top confusion pairs

### Day 26
- [ ] Add simple inference script for image prediction
- [ ] Validate on random test samples
- [ ] Add input preprocessing checks
- [ ] Write command usage in README

### Day 27
- [ ] Create side-by-side report: Scratch vs PyTorch
- [ ] Compare code complexity and performance
- [ ] List what you now understand deeply
- [ ] Add visuals

### Day 28
- [ ] Refactor and clean all code paths
- [ ] Ensure project reproducibility instructions work
- [ ] Organize artifacts and checkpoints
- [ ] Final QA pass

### Day 29
- [ ] Prepare 5-minute project demo summary
- [ ] Optional: record quick walkthrough video
- [ ] Gather one feedback round
- [ ] Apply final fixes

### Day 30 (Demo Day)
- [ ] Deliver Month 4 capstone:
  - [ ] MLP from scratch (core understanding)
  - [ ] PyTorch MLP (practical implementation)
  - [ ] MNIST results and error analysis
  - [ ] Reproducible training/inference pipeline
- [ ] Write Month 4 retrospective

**Month 4 Completion Criteria**
- [ ] Can explain forward pass and backprop intuitively
- [ ] Can implement MLP from scratch and in PyTorch
- [ ] Can train/evaluate/save/load neural models
- [ ] Can diagnose basic training issues

## Best Free Resources by Week
- **Week 1 (NN Building Blocks):**
  - 3Blue1Brown Neural Networks: https://www.3blue1brown.com/topics/neural-networks
  - CS231n notes (NN basics): https://cs231n.github.io/neural-networks-1/
- **Week 2 (Backprop + Training from Scratch):**
  - Karpathy micrograd: https://github.com/karpathy/micrograd
  - CS231n backprop/optimization notes: https://cs231n.github.io/optimization-2/
- **Week 3 (PyTorch Fundamentals):**
  - PyTorch tutorials: https://pytorch.org/tutorials/
  - 60-minute blitz: https://pytorch.org/tutorials/beginner/deep_learning_60min_blitz.html
- **Week 4 (MNIST Capstone):**
  - Official MNIST docs: http://yann.lecun.com/exdb/mnist/
  - PyTorch examples repo: https://github.com/pytorch/examples

## After Month 4
Continue with Month 5 in [documents/001-learning-path.md](documents/001-learning-path.md): deep learning training mastery and optimization.
