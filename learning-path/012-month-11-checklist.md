# Month 11 (Day 1–Day 30) — MLOps + Production AI

_Last updated: 23 Feb 2026_

## How to use this checklist
- Target: **2 to 3 hours/day**.
- Focus: ship, monitor, and maintain AI systems reliably.
- Treat every model as a production service, not only a notebook.

---

## Week 1 (Days 1–7): Serving and API Foundations

### Day 1
- [ ] Create `month-11-mlops/` project with `app`, `models`, `tests`, `infra`
- [ ] Select one previously trained model as production candidate
- [ ] Define service API contract (inputs/outputs/errors)
- [ ] Notes: SLA assumptions and constraints

### Day 2
- [ ] Build FastAPI inference endpoint (`/predict`)
- [ ] Add request/response schema validation
- [ ] Load model artifact safely at startup
- [ ] Return structured error messages

### Day 3
- [ ] Add batch inference endpoint (`/predict-batch`)
- [ ] Validate throughput and payload limits
- [ ] Add response metadata (model version, latency)
- [ ] Save API examples

### Day 4
- [ ] Add unit tests for API and inference logic
- [ ] Add integration smoke test with sample payloads
- [ ] Ensure deterministic output checks where possible
- [ ] Document test strategy

### Day 5
- [ ] Add logging (request id, latency, status)
- [ ] Add basic health checks (`/health`, `/ready`)
- [ ] Include model and dependency version in readiness output
- [ ] Notes: observability essentials

### Day 6
- [ ] Add configuration management (`env`/config file)
- [ ] Separate dev and production config defaults
- [ ] Validate startup with missing/invalid config
- [ ] Update README setup instructions

### Day 7 (Review)
- [ ] Rebuild and run API from clean environment
- [ ] Week summary (1 page)
- [ ] Push code + tests
- [ ] Clean project structure

**Week 1 Deliverable**
- [ ] Production-style inference API with tests and health checks

---

## Week 2 (Days 8–14): Containerization + CI Basics

### Day 8
- [ ] Write Dockerfile for the inference service
- [ ] Build local image and run container
- [ ] Validate API endpoints in container
- [ ] Log image size and startup time

### Day 9
- [ ] Add `.dockerignore` and optimize layers
- [ ] Improve build speed and image footprint
- [ ] Re-test functionality after optimization
- [ ] Document container run command

### Day 10
- [ ] Add docker-compose for local service dependencies (if needed)
- [ ] Define environment variables cleanly
- [ ] Validate multi-service startup
- [ ] Notes: local parity with production

### Day 11
- [ ] Set up CI workflow (lint + tests + build)
- [ ] Trigger CI on PR/push events
- [ ] Add status badges to README
- [ ] Ensure failing tests block merge

### Day 12
- [ ] Add API contract checks in CI (schema/response shape)
- [ ] Add smoke test step for built container
- [ ] Validate CI reproducibility
- [ ] Save CI troubleshooting notes

### Day 13
- [ ] Add semantic versioning for model/service releases
- [ ] Tag release candidate and changelog entry
- [ ] Verify rollback plan basics
- [ ] Document release process

### Day 14 (Review)
- [ ] Run full CI pipeline and address blockers
- [ ] Week summary (1 page)
- [ ] Push milestone
- [ ] Confirm Docker + CI docs are clear

**Week 2 Deliverable**
- [ ] Containerized service with working CI pipeline

---

## Week 3 (Days 15–21): Monitoring, Drift, and Retraining Concepts

### Day 15
- [ ] Define monitoring metrics (latency, error rate, data quality)
- [ ] Add request/response telemetry capture
- [ ] Build simple dashboard notebook/script
- [ ] Notes: alert thresholds rationale

### Day 16
- [ ] Add prediction distribution tracking
- [ ] Track input feature statistics over time
- [ ] Compare live vs training baseline distributions
- [ ] Flag potential drift conditions

### Day 17
- [ ] Implement basic drift checks (statistical proxy)
- [ ] Generate drift report artifact
- [ ] Add automated periodic check script
- [ ] Document interpretation limits

### Day 18
- [ ] Add data quality checks (missing/null/range anomalies)
- [ ] Define failure-handling policy for bad inputs
- [ ] Log quality incidents
- [ ] Add remediation actions

### Day 19
- [ ] Design retraining trigger policy (time-based or drift-based)
- [ ] Sketch retraining pipeline steps
- [ ] Add model validation gate before promotion
- [ ] Write model promotion checklist

### Day 20
- [ ] Add model registry-style metadata file
- [ ] Track model lineage (data/code/version)
- [ ] Save evaluation reports per model version
- [ ] Update operational README

### Day 21 (Review)
- [ ] Run monitoring/drift scripts on sample data stream
- [ ] Week summary (1 page)
- [ ] Push scripts and docs
- [ ] Consolidate operational artifacts

**Week 3 Deliverable**
- [ ] Monitoring and drift-aware operations baseline

---

## Week 4 (Days 22–30): MLOps Capstone

### Day 22
- [ ] Define final MLOps capstone acceptance criteria
- [ ] Freeze service API and model version
- [ ] Draft final architecture diagram
- [ ] Create capstone report template

### Day 23
- [ ] Finalize API + container deployment workflow
- [ ] Run end-to-end local deployment test
- [ ] Capture latency and reliability metrics
- [ ] Document deployment steps

### Day 24
- [ ] Finalize CI workflow and quality gates
- [ ] Add release checklist and rollback notes
- [ ] Validate all checks pass on clean branch
- [ ] Save CI evidence screenshots/logs

### Day 25
- [ ] Integrate monitoring and drift reports into routine
- [ ] Simulate drift/anomaly scenario
- [ ] Validate alerting and investigation flow
- [ ] Record incident response notes

### Day 26
- [ ] Build retraining pipeline skeleton/script
- [ ] Add placeholder for scheduled execution
- [ ] Validate model validation gate logic
- [ ] Document handoff process

### Day 27
- [ ] Complete final MLOps report
- [ ] Include architecture, reliability, and maintenance strategy
- [ ] Add known limitations and future improvements
- [ ] Polish docs and diagrams

### Day 28
- [ ] Reproducibility audit from clean environment
- [ ] Verify setup → test → run → monitor workflow
- [ ] Fix final issues
- [ ] Final cleanup

### Day 29
- [ ] Prepare 5-minute operations-focused walkthrough
- [ ] Optional demo recording
- [ ] Collect one feedback pass
- [ ] Apply critical fixes

### Day 30 (Demo Day)
- [ ] Deliver Month 11 capstone:
  - [ ] Inference API with tests and health checks
  - [ ] Containerized deployment + CI
  - [ ] Monitoring/drift pipeline basics
  - [ ] Retraining and release process documentation
- [ ] Write Month 11 retrospective

**Month 11 Completion Criteria**
- [ ] Can deploy and serve an ML model as an API
- [ ] Can containerize and validate via CI
- [ ] Can monitor quality/performance and detect drift
- [ ] Can document retraining and release lifecycle

## Best Free Resources by Week
- **Week 1 (API Serving):**
  - FastAPI docs: https://fastapi.tiangolo.com/
  - Pydantic docs: https://docs.pydantic.dev/
- **Week 2 (Docker + CI):**
  - Docker docs: https://docs.docker.com/
  - GitHub Actions docs: https://docs.github.com/en/actions
- **Week 3 (Monitoring + Drift):**
  - Evidently docs: https://docs.evidentlyai.com/
  - Prometheus docs: https://prometheus.io/docs/introduction/overview/
- **Week 4 (MLOps Capstone):**
  - MLflow docs: https://mlflow.org/docs/latest/index.html
  - Great Expectations docs: https://docs.greatexpectations.io/

## After Month 11
Continue with Month 12 in [learning-path/001-learning-path.md](learning-path/001-learning-path.md): final capstone, portfolio, and interview readiness.
