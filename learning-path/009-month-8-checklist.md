# Month 8 (Day 1–Day 30) — Transformers, LLMs, Prompting, and RAG

_Last updated: 23 Feb 2026_

## How to use this checklist
- Target: **2 to 3 hours/day**.
- Goal: move from NLP models to practical LLM application building.
- Track prompt versions and retrieval settings rigorously.

---

## Week 1 (Days 1–7): Transformer + LLM Practical Basics

### Day 1
- [ ] Create `month-8-llm-rag/` project structure
- [ ] Set up API/local-model access and environment variables
- [ ] Define task scope (Q&A, summarization, extraction)
- [ ] Notes: success and failure criteria

### Day 2
- [ ] Review transformer blocks and token limits
- [ ] Explore tokenizer behavior and context windows
- [ ] Run first simple prompts on sample data
- [ ] Save baseline prompt set

### Day 3
- [ ] Prompt engineering basics: role, task, constraints, format
- [ ] Test 10 prompt variants on same inputs
- [ ] Score outputs manually on quality dimensions
- [ ] Document best prompt patterns

### Day 4
- [ ] Structured outputs (JSON schema style)
- [ ] Add output validation checks
- [ ] Handle malformed responses safely
- [ ] Notes: prompt strategies for reliability

### Day 5
- [ ] Cost/latency awareness and token optimization
- [ ] Benchmark prompt lengths and response quality
- [ ] Choose practical default prompt template
- [ ] Save prompt cookbook

### Day 6
- [ ] Build minimal LLM wrapper module
- [ ] Add retry/timeouts/basic error handling
- [ ] Add run logging (input/prompt/output metadata)
- [ ] Write usage examples

### Day 7 (Review)
- [ ] Re-run core prompt benchmark from clean start
- [ ] Week summary (1 page)
- [ ] Push code + prompt logs
- [ ] Refine prompt templates

**Week 1 Deliverable**
- [ ] Stable prompting baseline with structured output handling

---

## Week 2 (Days 8–14): Retrieval-Augmented Generation (RAG) Foundations

### Day 8
- [ ] Choose domain documents and ingestion format
- [ ] Build document chunking strategy
- [ ] Compare chunk sizes/overlap choices
- [ ] Notes: retrieval granularity tradeoffs

### Day 9
- [ ] Generate embeddings and index vectors
- [ ] Implement top-k retrieval
- [ ] Inspect retrieval quality manually
- [ ] Save retrieval debug notebook

### Day 10
- [ ] Build first RAG chain (retrieve → prompt → answer)
- [ ] Include citation/source references in output
- [ ] Validate grounding on test questions
- [ ] Log hallucination cases

### Day 11
- [ ] Tune retriever settings (k, similarity threshold)
- [ ] Evaluate precision of retrieved chunks
- [ ] Improve prompt with context instructions
- [ ] Update quality score table

### Day 12
- [ ] Add query rewriting or multi-query retrieval (optional)
- [ ] Compare single-query vs enhanced retrieval
- [ ] Keep only if measurable gains
- [ ] Document complexity vs benefit

### Day 13
- [ ] Build eval set for RAG (20–50 curated questions)
- [ ] Score answers on correctness + citation faithfulness
- [ ] Track common failure categories
- [ ] Draft mitigation plan

### Day 14 (Review)
- [ ] Re-run full RAG pipeline on eval set
- [ ] Week summary (1 page)
- [ ] Push scripts/reports
- [ ] Freeze retriever baseline config

**Week 2 Deliverable**
- [ ] Working RAG system with initial evaluation set

---

## Week 3 (Days 15–21): LLM App Quality, Safety, and Reliability

### Day 15
- [ ] Build evaluation rubric (helpfulness, correctness, groundedness)
- [ ] Implement automatic scoring where possible
- [ ] Add manual review checklist
- [ ] Notes: evaluation blind spots

### Day 16
- [ ] Add guardrails for unsafe/off-topic/PII-sensitive prompts
- [ ] Implement basic input/output filters
- [ ] Test on adversarial prompt examples
- [ ] Document false positive/negative cases

### Day 17
- [ ] Add fallback behavior when retrieval is weak
- [ ] Use “insufficient context” response policy
- [ ] Measure hallucination reduction
- [ ] Save before/after comparison

### Day 18
- [ ] Improve answer format consistency
- [ ] Add citation formatting and source ranking
- [ ] Validate citation traceability
- [ ] Notes: confidence reporting policy

### Day 19
- [ ] Add telemetry logging for latency/token usage/errors
- [ ] Build simple quality dashboard notebook
- [ ] Identify performance bottlenecks
- [ ] Plan optimization actions

### Day 20
- [ ] Package RAG app as script/API skeleton
- [ ] Add config-driven model/retriever settings
- [ ] Verify reproducibility with sample dataset
- [ ] Update README setup guide

### Day 21 (Review)
- [ ] Re-test full pipeline on eval + stress prompts
- [ ] Week summary (1 page)
- [ ] Push milestone release
- [ ] Clean artifacts

**Week 3 Deliverable**
- [ ] Reliable RAG pipeline with guardrails and evaluation

---

## Week 4 (Days 22–30): LLM/RAG Capstone

### Day 22
- [ ] Define final capstone domain and user stories
- [ ] Freeze dataset and eval questions
- [ ] Set measurable acceptance criteria
- [ ] Draft final report structure

### Day 23
- [ ] Build final ingestion/indexing pipeline
- [ ] Validate chunking and retrieval quality
- [ ] Save retriever metrics
- [ ] Document indexing assumptions

### Day 24
- [ ] Integrate best prompting strategy
- [ ] Integrate citation and fallback policies
- [ ] Run full eval benchmark
- [ ] Capture key metrics

### Day 25
- [ ] Perform error analysis (hallucinations, missed context, formatting)
- [ ] Implement top 2–3 fixes
- [ ] Re-run eval and compare deltas
- [ ] Finalize quality table

### Day 26
- [ ] Build user-facing demo script/API endpoint
- [ ] Add example queries and expected behaviors
- [ ] Validate with unseen questions
- [ ] Add operational notes

### Day 27
- [ ] Complete final report with methodology + results
- [ ] Include safety and limitation section
- [ ] Add future improvement roadmap
- [ ] Polish documentation

### Day 28
- [ ] Reproducibility audit from clean environment
- [ ] Verify setup/index/query flow works end-to-end
- [ ] Fix config/path/dependency issues
- [ ] Final code cleanup

### Day 29
- [ ] Prepare 5-minute capstone walkthrough
- [ ] Optional demo video recording
- [ ] Gather one feedback pass
- [ ] Apply critical fixes

### Day 30 (Demo Day)
- [ ] Deliver Month 8 capstone:
  - [ ] Domain RAG assistant with citations
  - [ ] Eval set with quality metrics
  - [ ] Safety/fallback handling
  - [ ] Reproducible setup and usage docs
- [ ] Write Month 8 retrospective

**Month 8 Completion Criteria**
- [ ] Can design and tune prompts systematically
- [ ] Can build and evaluate a grounded RAG workflow
- [ ] Can implement practical guardrails
- [ ] Can package an LLM app for reproducible use

## Best Free Resources by Week
- **Week 1 (Prompting + LLM Basics):**
  - Prompt Engineering Guide: https://www.promptingguide.ai/
  - Hugging Face Transformers docs: https://huggingface.co/docs/transformers/index
- **Week 2 (RAG Foundations):**
  - LangChain RAG docs: https://python.langchain.com/docs/concepts/rag/
  - LlamaIndex docs: https://docs.llamaindex.ai/
- **Week 3 (Evaluation + Safety):**
  - RAGAS docs: https://docs.ragas.io/
  - OWASP LLM Top 10: https://owasp.org/www-project-top-10-for-large-language-model-applications/
- **Week 4 (Capstone Packaging):**
  - FastAPI docs: https://fastapi.tiangolo.com/
  - Gradio docs: https://www.gradio.app/docs

## After Month 8
Continue with Month 9 in [001-learning-path.md](001-learning-path.md): generative AI beyond text (GAN/VAE/diffusion basics).
