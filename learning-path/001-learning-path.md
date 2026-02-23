# AI Learning Path (12 Months) — Beginner to Advanced

_Last updated: 23 Feb 2026_

## How to use this plan
- Weekly time target: **8–12 hours/week** (can scale up/down).
- Pattern each week:
  - **Learn (40%)**: watch/read core concepts.
  - **Build (40%)**: implement from scratch + library version.
  - **Reflect (20%)**: notes, mistakes, and summary.
- Always keep one public repo with:
  - `/notes` for theory notes
  - `/projects` for code
  - `/experiments` for model runs and metrics

---

## Month 1 — Programming + Math Foundations

### Goals
- Become comfortable with Python and core math needed for AI.
- Build coding discipline and reproducibility habits.

### Week-by-week
- **Week 1:** Python basics (types, loops, functions), Git/GitHub basics.
- **Week 2:** Numpy, Pandas, Matplotlib; data loading and plotting.
- **Week 3:** Linear algebra essentials (vectors, matrices, dot product, matrix multiplication).
- **Week 4:** Probability/statistics + intro calculus for optimization.

### Project
- **Student Performance Analyzer**
  - Load CSV, clean missing values, do EDA, visualize trends.
  - Write a short report with observations.

### Free resources
- Python: Harvard CS50P (YouTube), freeCodeCamp Python
- Math: Khan Academy (Linear Algebra, Probability, Calculus)
- Practical math for ML: StatQuest (YouTube)

---

## Month 2 — Data Handling + Classical ML Basics

### Goals
- Understand end-to-end data pipeline and first ML models.

### Week-by-week
- **Week 5:** Data preprocessing (scaling, encoding, train/val/test split).
- **Week 6:** Linear regression, logistic regression, evaluation metrics.
- **Week 7:** Decision trees, random forests.
- **Week 8:** Cross-validation, overfitting/underfitting, regularization.

### Project
- **House Price Predictor**
  - Baseline linear model vs tree-based model.
  - Compare MAE/RMSE and explain tradeoffs.

### Free resources
- Scikit-learn official tutorials
- Google Machine Learning Crash Course (MLCC)
- Kaggle Intro to Machine Learning

---

## Month 3 — Intermediate ML + Competitions Mindset

### Goals
- Improve model quality and experimentation practices.

### Week-by-week
- **Week 9:** Gradient boosting (XGBoost/LightGBM concepts).
- **Week 10:** Feature engineering, feature importance, leakage prevention.
- **Week 11:** Unsupervised learning (KMeans, PCA).
- **Week 12:** Hyperparameter tuning (Grid/Random/Bayesian basics).

### Project
- **Customer Churn Prediction**
  - Full pipeline with preprocessing + model comparison.
  - Add confusion matrix, precision/recall, ROC-AUC.

### Free resources
- Kaggle Intermediate ML + Feature Engineering
- StatQuest (ensembles, PCA, bias-variance)
- Optuna docs/tutorials

---

## Month 4 — Neural Networks from Scratch + PyTorch Basics

### Goals
- Understand neural nets deeply (not only API usage).

### Week-by-week
- **Week 13:** Perceptron, MLP, activation/loss functions.
- **Week 14:** Backpropagation math + gradient descent.
- **Week 15:** Build MLP from scratch with Numpy.
- **Week 16:** Rebuild same model in PyTorch with training loop.

### Project
- **MNIST Digit Classifier (Scratch + PyTorch)**
  - Implement from scratch and then with PyTorch.
  - Compare performance and code simplicity.

### Free resources
- 3Blue1Brown neural network series
- PyTorch official tutorials
- Andrej Karpathy micrograd videos/repo

---

## Month 5 — Deep Learning Training Mastery

### Goals
- Learn to train stable and performant deep models.

### Week-by-week
- **Week 17:** Optimizers (SGD, Momentum, Adam), learning rates.
- **Week 18:** Initialization, normalization, dropout, regularization.
- **Week 19:** Experiment tracking and reproducibility.
- **Week 20:** Error analysis and ablation studies.

### Project
- **Image Classifier on CIFAR-10**
  - Build robust training pipeline with augmentations.
  - Track experiments and summarize best recipe.

### Free resources
- fast.ai Practical Deep Learning
- Weights & Biases free docs/tutorials
- Papers With Code (benchmark exploration)

---

## Month 6 — Computer Vision Core

### Goals
- Build practical CV systems and understand transfer learning.

### Week-by-week
- **Week 21:** CNN architecture fundamentals.
- **Week 22:** Transfer learning with pretrained models.
- **Week 23:** Object detection/segmentation concepts.
- **Week 24:** Vision model evaluation and deployment constraints.

### Project
- **Custom Image Classifier + Mini Detection Demo**
  - Fine-tune pretrained model on your own dataset.
  - Optional: use YOLO small model for detection demo.

### Free resources
- PyTorch vision tutorials
- Ultralytics YOLO docs
- Stanford CS231n lecture videos

---

## Month 7 — NLP Fundamentals

### Goals
- Move from bag-of-words to embeddings and sequence models.

### Week-by-week
- **Week 25:** Text cleaning, tokenization, TF-IDF, embeddings.
- **Week 26:** RNN/LSTM/GRU basics for sequence data.
- **Week 27:** Attention mechanism and intuition.
- **Week 28:** Build text classification pipeline.

### Project
- **Sentiment Analyzer**
  - Baseline: TF-IDF + Logistic Regression.
  - Neural: embedding + LSTM.

### Free resources
- Hugging Face NLP Course (free)
- Illustrated Transformer (Jay Alammar)
- NLP playlists by AssemblyAI/StatQuest

---

## Month 8 — Transformers + LLM Fundamentals

### Goals
- Understand modern LLM stack and practical usage patterns.

### Week-by-week
- **Week 29:** Transformer architecture deep dive.
- **Week 30:** Prompting techniques and evaluation.
- **Week 31:** Retrieval-Augmented Generation (RAG) basics.
- **Week 32:** Fine-tuning concepts (LoRA/PEFT overview).

### Project
- **Domain Q&A Assistant (RAG)**
  - Ingest docs, embed, retrieve, answer with citations.
  - Evaluate faithfulness and hallucination cases.

### Free resources
- Hugging Face Transformers course/docs
- LangChain or LlamaIndex docs (choose one)
- Open-source LLM guides (e.g., llama.cpp docs)

---

## Month 9 — Generative AI Beyond Text

### Goals
- Learn image/audio generation concepts and limitations.

### Week-by-week
- **Week 33:** GAN and VAE intuition.
- **Week 34:** Diffusion model basics.
- **Week 35:** Multimodal systems intro (text-image).
- **Week 36:** Safety, alignment, prompt/response filtering.

### Project
- **Image Generation Experiment Notebook**
  - Compare prompt settings and output quality.
  - Document safety checks and failure modes.

### Free resources
- Hugging Face Diffusers docs
- Lil’Log by OpenAI (conceptual deep dives)
- Two Minute Papers (concept overview)

---

## Month 10 — Reinforcement Learning + Sequential Decision Making

### Goals
- Understand agent learning from rewards.

### Week-by-week
- **Week 37:** Markov Decision Process, value functions.
- **Week 38:** Q-learning, DQN.
- **Week 39:** Policy gradients, actor-critic, PPO intuition.
- **Week 40:** Reward shaping and evaluation pitfalls.

### Project
- **RL Agent in Gymnasium Environment**
  - Train and compare DQN vs PPO on simple control task.
  - Plot reward curves and stability.

### Free resources
- Sutton & Barto (free draft)
- David Silver RL lectures (YouTube)
- CleanRL docs/examples

---

## Month 11 — MLOps + Production AI

### Goals
- Ship and maintain ML systems in real environments.

### Week-by-week
- **Week 41:** Model packaging, REST inference API.
- **Week 42:** Docker, CI basics, reproducible environments.
- **Week 43:** Monitoring: drift, latency, quality metrics.
- **Week 44:** Retraining pipeline and model registry concepts.

### Project
- **Model Serving Service**
  - Serve one trained model with FastAPI.
  - Add logging, health checks, simple monitoring dashboard.

### Free resources
- FastAPI docs
- Docker docs
- MLflow docs
- Evidently AI docs (monitoring)

---

## Month 12 — Capstone + Portfolio + Interview Readiness

### Goals
- Consolidate everything into one high-quality end-to-end project.

### Week-by-week
- **Week 45:** Pick problem + dataset + measurable success criteria.
- **Week 46:** Build v1 pipeline and baseline metrics.
- **Week 47:** Improve model + inference + monitoring.
- **Week 48:** Write documentation, architecture, and demo video.

### Capstone options (pick one)
- **AI Tutor** (RAG + feedback loop)
- **Medical/Legal Document Q&A** (if domain-safe data available)
- **Smart Vision Inspector** (defect detection)
- **Personalized Recommender**

### Deliverables
- Clean GitHub repo with README, architecture diagram, metrics table
- One blog post: problem, approach, lessons
- Short demo video (3–5 min)

---

## Ongoing Weekly Routine (All 12 Months)
- **1 day:** Theory and notes
- **2 days:** Implementation
- **1 day:** Experiments and debugging
- **1 day:** Review + write what you learned

## Skill Checklist by End of Year
- Can build, evaluate, and deploy ML/DL models.
- Can work with NLP/LLM and basic RAG pipelines.
- Can run experiments reproducibly and explain tradeoffs.
- Can ship one production-style AI application.
- Can discuss ethics, bias, and monitoring in AI systems.

---

## Optional Free Certifications / Milestones
- Kaggle micro-courses badges
- Google ML Crash Course completion
- DeepLearning.AI short courses (audit/free where available)
- Hugging Face course certificate (if offered at the time)

## Notes for your current workspace
You can align this with your current folder structure:
- `projects/ai/01-neural-network` → Months 4–5
- `projects/ai/02-character-level-language-model` → Months 7–8
- `services/ai/` → Months 11–12 for deployment practice

If you want, the next step is: I can generate a **Month 1 exact daily checklist** inside a second file so you can start immediately tomorrow.