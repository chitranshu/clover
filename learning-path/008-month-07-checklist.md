# Month 7 (Day 1–Day 30) — NLP Fundamentals + Sequence Models

_Last updated: 23 Feb 2026_

## How to use this checklist
- Target: **2 to 3 hours/day**.
- Build two baselines: classical NLP and neural NLP.
- Keep dataset preprocessing reproducible and versioned.

---

## Week 1 (Days 1–7): Text Processing + Classical NLP

### Day 1
- [ ] Create `month-7-nlp-fundamentals/` structure
- [ ] Pick dataset (sentiment/spam/topic)
- [ ] Build text ingestion and label pipeline
- [ ] Notes: label quality and dataset caveats

### Day 2
- [ ] Text cleaning (lowercase, punctuation, normalization)
- [ ] Tokenization basics
- [ ] Explore sequence lengths and vocabulary size
- [ ] Save preprocessing config

### Day 3
- [ ] Feature extraction with Bag-of-Words
- [ ] Train logistic regression baseline
- [ ] Evaluate accuracy/F1/confusion matrix
- [ ] Document baseline limitations

### Day 4
- [ ] TF-IDF features and n-grams
- [ ] Compare vs Bag-of-Words baseline
- [ ] Tune regularization for logistic regression
- [ ] Save leaderboard update

### Day 5
- [ ] Error analysis on misclassified texts
- [ ] Inspect top tokens/weights
- [ ] Identify data cleaning improvements
- [ ] Write correction plan

### Day 6
- [ ] Build reusable classical NLP pipeline script
- [ ] Add train/eval CLI arguments
- [ ] Save model + vectorizer artifacts
- [ ] Write inference usage docs

### Day 7 (Review)
- [ ] Re-run classical baseline from clean setup
- [ ] Week summary (1 page)
- [ ] Push code + results
- [ ] Clean notebooks/scripts

**Week 1 Deliverable**
- [ ] Strong classical NLP baseline (TF-IDF + LR)

---

## Week 2 (Days 8–14): Embeddings + RNN/LSTM Basics

### Day 8
- [ ] Word embeddings intuition (static vs contextual)
- [ ] Train embedding + simple classifier baseline
- [ ] Compare against TF-IDF performance
- [ ] Notes: where embeddings help

### Day 9
- [ ] RNN fundamentals for sequence data
- [ ] Implement basic RNN text classifier in PyTorch
- [ ] Validate sequence padding/masking pipeline
- [ ] Log training behavior

### Day 10
- [ ] LSTM/GRU concepts and differences
- [ ] Replace RNN with LSTM model
- [ ] Compare stability and metrics
- [ ] Save model comparison table

### Day 11
- [ ] Tune sequence length, embedding dim, hidden size
- [ ] Add dropout and weight decay
- [ ] Track overfitting trends
- [ ] Document best configuration

### Day 12
- [ ] Add attention mechanism intuition (lightweight)
- [ ] Implement simple attention over LSTM outputs (optional)
- [ ] Evaluate impact on difficult samples
- [ ] Notes: interpretability gains

### Day 13
- [ ] Build standardized evaluation and prediction scripts
- [ ] Add class-wise performance and hard-example logging
- [ ] Save all artifacts and configs
- [ ] Update README usage

### Day 14 (Review)
- [ ] Reproduce best neural run end-to-end
- [ ] Week summary (1 page)
- [ ] Push milestone
- [ ] Consolidate notes

**Week 2 Deliverable**
- [ ] Neural sequence model pipeline with evaluation

---

## Week 3 (Days 15–21): Transformer Intuition + Practical Intro

### Day 15
- [ ] Study attention and transformer encoder intuition
- [ ] Review tokenization (WordPiece/BPE basics)
- [ ] Map concepts to existing NLP tasks
- [ ] Notes: why transformers scale well

### Day 16
- [ ] Use pretrained transformer for classification (Hugging Face)
- [ ] Fine-tune on your dataset
- [ ] Compare with LSTM and TF-IDF baselines
- [ ] Log runtime and accuracy tradeoff

### Day 17
- [ ] Tune learning rate, batch size, epochs
- [ ] Add early stopping/checkpointing
- [ ] Track validation behavior
- [ ] Save best run details

### Day 18
- [ ] Evaluate calibration/confidence on uncertain examples
- [ ] Inspect attention/attribution proxies (optional)
- [ ] Document error clusters
- [ ] Add practical improvement ideas

### Day 19
- [ ] Build lightweight inference script with tokenizer/model loading
- [ ] Batch inference on sample text file
- [ ] Save outputs with confidence scores
- [ ] Validate consistency across runs

### Day 20
- [ ] Final model comparison: TF-IDF vs LSTM vs Transformer
- [ ] Produce concise benchmark report
- [ ] Choose deployment candidate
- [ ] Justify model choice clearly

### Day 21 (Review)
- [ ] Re-run best transformer pipeline from clean env
- [ ] Week summary (1 page)
- [ ] Push scripts/reports
- [ ] Archive unused experiments

**Week 3 Deliverable**
- [ ] Transformer-based text classifier benchmarked against baselines

---

## Week 4 (Days 22–30): NLP Capstone

### Day 22
- [ ] Define final NLP capstone scope and success metric
- [ ] Lock dataset split and evaluation protocol
- [ ] Create report outline
- [ ] Freeze preprocessing config

### Day 23
- [ ] Train final baseline and candidate models
- [ ] Run standardized evaluations
- [ ] Save full metrics table
- [ ] Validate no leakage

### Day 24
- [ ] Perform deep error analysis by text category/length
- [ ] Add confusion slices and failure examples
- [ ] Draft mitigation strategy
- [ ] Update report

### Day 25
- [ ] Finalize best model and hyperparameters
- [ ] Save artifacts (model, tokenizer, config)
- [ ] Add inference CLI/API-style script
- [ ] Document usage examples

### Day 26
- [ ] Add robustness checks (typos/paraphrases/short text)
- [ ] Measure sensitivity to input variation
- [ ] Record practical limitations
- [ ] Add safety note section

### Day 27
- [ ] Complete final NLP project report
- [ ] Include methodology, metrics, errors, and risks
- [ ] Add plots/tables for clarity
- [ ] Polish README

### Day 28
- [ ] Reproducibility audit (fresh setup test)
- [ ] Confirm end-to-end training/inference works
- [ ] Fix dependency/documentation gaps
- [ ] Final code cleanup

### Day 29
- [ ] Prepare 5-minute capstone walkthrough
- [ ] Optional demo video recording
- [ ] Collect feedback and apply key improvements
- [ ] Tag release version

### Day 30 (Demo Day)
- [ ] Deliver Month 7 capstone:
  - [ ] End-to-end NLP pipeline
  - [ ] Baseline vs neural vs transformer comparison
  - [ ] Error and robustness analysis
  - [ ] Reproducible inference workflow
- [ ] Write Month 7 retrospective

**Month 7 Completion Criteria**
- [ ] Can build strong classical and neural NLP baselines
- [ ] Can fine-tune transformer for text classification
- [ ] Can evaluate model quality beyond accuracy
- [ ] Can ship an NLP inference-ready artifact

## Best Free Resources by Week
- **Week 1 (Classical NLP):**
  - Scikit-learn text feature extraction: https://scikit-learn.org/stable/modules/feature_extraction.html#text-feature-extraction
  - NLTK book (free online): https://www.nltk.org/book/
- **Week 2 (RNN/LSTM/GRU):**
  - PyTorch NLP sequence tutorial: https://pytorch.org/tutorials/beginner/nlp/sequence_models_tutorial.html
  - Colah LSTM article: https://colah.github.io/posts/2015-08-Understanding-LSTMs/
- **Week 3 (Transformers Intro):**
  - Hugging Face NLP course: https://huggingface.co/learn/nlp-course
  - Illustrated Transformer: https://jalammar.github.io/illustrated-transformer/
- **Week 4 (NLP Capstone + Evaluation):**
  - Evaluate library docs: https://huggingface.co/docs/evaluate/index
  - Kaggle NLP datasets/notebooks: https://www.kaggle.com/datasets?tags=13303-NLP

## After Month 7
Continue with Month 8 in [001-learning-path.md](001-learning-path.md): transformers/LLMs, prompting, and RAG basics.
