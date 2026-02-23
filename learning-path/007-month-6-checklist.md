# Month 6 (Day 1–Day 30) — Computer Vision Core + Transfer Learning

_Last updated: 23 Feb 2026_

## How to use this checklist
- Target: **2 to 3 hours/day**.
- Core balance: architecture understanding + practical fine-tuning.
- Keep all runs logged with dataset/version/model details.

---

## Week 1 (Days 1–7): CNN Foundations + Data Pipelines

### Day 1
- [ ] Create `month-6-computer-vision/` project setup
- [ ] Prepare image dataset folders and class labels
- [ ] Build data loader with train/val/test splits
- [ ] Notes: dataset quality and imbalance

### Day 2
- [ ] Review CNN layers: conv, pooling, stride, padding
- [ ] Visualize feature map intuition
- [ ] Implement small CNN from scratch in PyTorch
- [ ] Check tensor shape flow

### Day 3
- [ ] Train small CNN baseline on chosen dataset
- [ ] Track accuracy/loss per epoch
- [ ] Add confusion matrix report
- [ ] Log key failure classes

### Day 4
- [ ] Add augmentations (flip/crop/rotate/color jitter)
- [ ] Compare baseline vs augmented training
- [ ] Choose safe augmentations for your domain
- [ ] Notes: harmful augmentations

### Day 5
- [ ] Class imbalance handling (weights, sampling)
- [ ] Evaluate macro vs weighted metrics
- [ ] Improve minority-class performance
- [ ] Save metric comparison table

### Day 6
- [ ] Add robust evaluation script and report output
- [ ] Include per-class precision/recall/F1
- [ ] Automate result artifact saving
- [ ] Validate report consistency

### Day 7 (Review)
- [ ] Rebuild data pipeline and baseline from scratch
- [ ] Week summary (1 page)
- [ ] Push code + report
- [ ] Cleanup dataset and scripts

**Week 1 Deliverable**
- [ ] Working CV baseline with reliable evaluation

---

## Week 2 (Days 8–14): Transfer Learning for Image Classification

### Day 8
- [ ] Load pretrained model (ResNet/EfficientNet)
- [ ] Freeze backbone, train classifier head only
- [ ] Compare against custom CNN baseline
- [ ] Log speed and performance

### Day 9
- [ ] Unfreeze top layers for fine-tuning
- [ ] Use lower LR for pretrained layers
- [ ] Track gains vs overfitting risk
- [ ] Notes: when to unfreeze more

### Day 10
- [ ] Compare 2 pretrained architectures
- [ ] Benchmark accuracy vs latency tradeoff
- [ ] Pick best candidate for your constraints
- [ ] Save leaderboard

### Day 11
- [ ] Calibrate confidence and inspect misclassifications
- [ ] Add top-k accuracy (if multi-class)
- [ ] Review uncertainty on hard examples
- [ ] Document reliability concerns

### Day 12
- [ ] Add test-time augmentation (optional)
- [ ] Evaluate if it improves stability
- [ ] Keep only if consistent gains
- [ ] Update final pipeline config

### Day 13
- [ ] Build inference script for single and batch images
- [ ] Add preprocessing parity checks
- [ ] Save prediction outputs to CSV/JSON
- [ ] Write usage docs

### Day 14 (Review)
- [ ] Re-run full transfer-learning pipeline cleanly
- [ ] Week summary (1 page)
- [ ] Push milestone
- [ ] Finalize selected model recipe

**Week 2 Deliverable**
- [ ] Fine-tuned pretrained classifier with inference script

---

## Week 3 (Days 15–21): Detection/Segmentation Concepts + Practical Demo

### Day 15
- [ ] Study detection basics (boxes, IoU, mAP)
- [ ] Review segmentation basics (masks, IoU/Dice)
- [ ] Choose one track for practice demo
- [ ] Notes: task differences and use-cases

### Day 16
- [ ] Set up demo with YOLO (detection) or U-Net (segmentation)
- [ ] Prepare small labeled sample dataset
- [ ] Run baseline training/inference
- [ ] Capture initial metrics/examples

### Day 17
- [ ] Tune core hyperparameters for selected track
- [ ] Improve precision/recall balance
- [ ] Save visual outputs (predictions)
- [ ] Log failure patterns

### Day 18
- [ ] Add evaluation summary notebook
- [ ] Include qualitative and quantitative analysis
- [ ] Identify dominant error categories
- [ ] Propose next improvements

### Day 19
- [ ] Benchmark inference latency and memory usage
- [ ] Compare CPU/GPU behavior if available
- [ ] Record deployment feasibility notes
- [ ] Select practical configuration

### Day 20
- [ ] Build lightweight demo script for chosen task
- [ ] Validate input/output consistency
- [ ] Add basic error handling
- [ ] Document end-user steps

### Day 21 (Review)
- [ ] Re-run demo from scratch on clean setup
- [ ] Week summary (1 page)
- [ ] Push scripts/results
- [ ] Organize artifacts

**Week 3 Deliverable**
- [ ] Detection or segmentation mini-demo with evaluation

---

## Week 4 (Days 22–30): Vision Capstone

### Day 22
- [ ] Define final capstone scope (classification + optional detection)
- [ ] Set acceptance criteria (metric + latency target)
- [ ] Lock dataset and split strategy
- [ ] Draft final README structure

### Day 23
- [ ] Train and evaluate final classification pipeline
- [ ] Save best checkpoint and full metrics
- [ ] Create confusion matrix and class report
- [ ] Document limitations

### Day 24
- [ ] Integrate optional detection/segmentation demo
- [ ] Align output format and naming
- [ ] Add side-by-side result visuals
- [ ] Update report draft

### Day 25
- [ ] Run robustness checks (lighting/crop/blur/noise)
- [ ] Quantify degradation by perturbation type
- [ ] Record mitigation ideas
- [ ] Add reliability section

### Day 26
- [ ] Finalize inference CLI and batch processing
- [ ] Validate on unseen sample set
- [ ] Add reproducibility instructions
- [ ] Verify dependencies

### Day 27
- [ ] Complete project report (method, metrics, errors, risks)
- [ ] Add architecture flow diagram (optional)
- [ ] Include deployment notes
- [ ] Polish visuals and wording

### Day 28
- [ ] Reproducibility audit on clean environment
- [ ] Confirm setup/train/infer commands work
- [ ] Fix doc and path issues
- [ ] Final code cleanup

### Day 29
- [ ] Prepare 5-minute project walkthrough
- [ ] Optional: record demo video
- [ ] Incorporate one feedback pass
- [ ] Freeze release version

### Day 30 (Demo Day)
- [ ] Deliver Month 6 capstone:
  - [ ] Fine-tuned vision model with strong evaluation
  - [ ] Inference-ready script
  - [ ] Robustness observations
  - [ ] Clear documentation
- [ ] Write Month 6 retrospective

**Month 6 Completion Criteria**
- [ ] Can build and fine-tune CV models effectively
- [ ] Can evaluate per-class quality and failures
- [ ] Can deliver practical inference pipeline
- [ ] Understands latency/robustness tradeoffs

## Best Free Resources by Week
- **Week 1 (CNN + Data Pipelines):**
  - CS231n ConvNet notes: https://cs231n.github.io/convolutional-networks/
  - PyTorch data loading tutorial: https://pytorch.org/tutorials/beginner/data_loading_tutorial.html
- **Week 2 (Transfer Learning):**
  - PyTorch transfer learning tutorial: https://pytorch.org/tutorials/beginner/transfer_learning_tutorial.html
  - timm model library docs: https://huggingface.co/docs/timm/index
- **Week 3 (Detection/Segmentation):**
  - Ultralytics YOLO docs: https://docs.ultralytics.com/
  - TorchVision detection tutorial: https://pytorch.org/tutorials/intermediate/torchvision_tutorial.html
- **Week 4 (Capstone + Deployment):**
  - ONNX runtime docs: https://onnxruntime.ai/docs/
  - OpenCV docs: https://docs.opencv.org/

## After Month 6
Continue with Month 7 in [001-learning-path.md](001-learning-path.md): NLP fundamentals and sequence modeling.
