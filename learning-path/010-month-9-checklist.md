# Month 9 (Day 1–Day 30) — Generative AI Beyond Text (GAN, VAE, Diffusion)

_Last updated: 23 Feb 2026_

## How to use this checklist
- Target: **2 to 3 hours/day**.
- Focus: concept clarity + controlled experiments.
- Keep visual results organized by run and settings.

---

## Week 1 (Days 1–7): Generative Modeling Foundations + VAE

### Day 1
- [ ] Create `month-9-generative-ai/` structure
- [ ] Prepare image dataset and baseline preprocessing
- [ ] Define evaluation approach (qualitative + simple quantitative)
- [ ] Notes: generation quality criteria

### Day 2
- [ ] Study likelihood/latent-space intuition
- [ ] Understand VAE encoder/decoder structure
- [ ] Implement toy VAE architecture in PyTorch
- [ ] Validate shape flow and reconstruction path

### Day 3
- [ ] Implement VAE loss (reconstruction + KL)
- [ ] Train VAE on small dataset subset
- [ ] Visualize reconstructions across epochs
- [ ] Document training stability behavior

### Day 4
- [ ] Latent space exploration (interpolation)
- [ ] Generate interpolation grids
- [ ] Analyze smoothness and semantic transitions
- [ ] Notes: latent collapse signs

### Day 5
- [ ] Tune latent dimension and KL weighting
- [ ] Compare sample quality across configs
- [ ] Save side-by-side outputs
- [ ] Record best settings

### Day 6
- [ ] Build script for sampling/generation from trained VAE
- [ ] Add reproducible seed options
- [ ] Save outputs with metadata
- [ ] Write usage notes

### Day 7 (Review)
- [ ] Re-run best VAE training from clean setup
- [ ] Week summary (1 page)
- [ ] Push code + sample gallery
- [ ] Clean artifacts

**Week 1 Deliverable**
- [ ] Working VAE with latent exploration report

---

## Week 2 (Days 8–14): GAN Basics + Stability Techniques

### Day 8
- [ ] Review GAN min-max objective intuition
- [ ] Implement simple GAN (MLP/CNN-based)
- [ ] Validate generator/discriminator step logic
- [ ] Notes: training instability patterns

### Day 9
- [ ] Train baseline GAN and track losses
- [ ] Save generated samples by epoch
- [ ] Diagnose mode collapse indicators
- [ ] Log observations

### Day 10
- [ ] Add stabilization tricks (label smoothing, noise, update ratio)
- [ ] Compare with baseline training stability
- [ ] Keep best strategy only
- [ ] Update experiment table

### Day 11
- [ ] Implement DCGAN-style architecture improvement
- [ ] Compare quality vs baseline GAN
- [ ] Save curated comparison outputs
- [ ] Document architecture impact

### Day 12
- [ ] Add lightweight quantitative proxy (e.g., FID-like or classifier proxy)
- [ ] Track metric trend with sample quality
- [ ] Note mismatch between metric and perception
- [ ] Refine evaluation rubric

### Day 13
- [ ] Build generation CLI for GAN checkpoints
- [ ] Add model selection by run id
- [ ] Ensure deterministic seeds where possible
- [ ] Write README usage section

### Day 14 (Review)
- [ ] Reproduce best GAN run from config
- [ ] Week summary (1 page)
- [ ] Push milestone
- [ ] Organize sample outputs

**Week 2 Deliverable**
- [ ] Stable GAN pipeline with comparative analysis

---

## Week 3 (Days 15–21): Diffusion Model Concepts + Practical Usage

### Day 15
- [ ] Study diffusion forward/reverse process intuition
- [ ] Understand noise schedules and denoising steps
- [ ] Map concepts to practical tools
- [ ] Notes: why diffusion is stable/high quality

### Day 16
- [ ] Set up diffusion workflow (library-based)
- [ ] Generate baseline outputs from prompts/settings
- [ ] Record seeds, guidance scale, steps
- [ ] Save run metadata

### Day 17
- [ ] Prompt and parameter sweep experiments
- [ ] Compare quality/diversity tradeoffs
- [ ] Build best-practice defaults table
- [ ] Document failure cases

### Day 18
- [ ] Optional fine-tuning concept review (LoRA at high level)
- [ ] Run small adaptation experiment if feasible
- [ ] Compare base vs adapted outputs
- [ ] Notes: compute/data constraints

### Day 19
- [ ] Safety considerations in image generation
- [ ] Add content filtering policy for outputs
- [ ] Test unsafe/ambiguous prompt handling
- [ ] Document guardrail decisions

### Day 20
- [ ] Build small notebook/app for generation demo
- [ ] Add reproducible controls (seed/settings)
- [ ] Export result gallery
- [ ] Add usage guide

### Day 21 (Review)
- [ ] Re-run best diffusion settings from clean config
- [ ] Week summary (1 page)
- [ ] Push scripts/notebooks
- [ ] Consolidate visuals

**Week 3 Deliverable**
- [ ] Diffusion experiment pack with parameter insights

---

## Week 4 (Days 22–30): Generative AI Capstone

### Day 22
- [ ] Define capstone scope (VAE/GAN/Diffusion comparison)
- [ ] Set quality and reliability criteria
- [ ] Build report template
- [ ] Freeze dataset/settings for fairness

### Day 23
- [ ] Run final VAE experiments and collect artifacts
- [ ] Run final GAN experiments and collect artifacts
- [ ] Compile qualitative gallery
- [ ] Save metric summaries

### Day 24
- [ ] Run final diffusion experiments on same prompt set
- [ ] Compare quality/diversity/control
- [ ] Build side-by-side comparison board
- [ ] Draft key findings

### Day 25
- [ ] Perform deep failure analysis (artifacts, collapse, incoherence)
- [ ] Add mitigation recommendations
- [ ] Update methodology and limitations
- [ ] Finalize comparison tables

### Day 26
- [ ] Build unified generation script interface
- [ ] Add model/mode selection + output naming
- [ ] Validate reproducibility commands
- [ ] Improve docs

### Day 27
- [ ] Complete final capstone report
- [ ] Include architecture intuition and practical takeaways
- [ ] Add safety and ethics notes
- [ ] Polish visuals

### Day 28
- [ ] Reproducibility audit on clean environment
- [ ] Verify all scripts and paths
- [ ] Fix dependency/config issues
- [ ] Final code cleanup

### Day 29
- [ ] Prepare 5-minute walkthrough
- [ ] Optional demo video
- [ ] Collect feedback and apply key fixes
- [ ] Freeze final release

### Day 30 (Demo Day)
- [ ] Deliver Month 9 capstone:
  - [ ] Comparative generative AI project
  - [ ] Controlled experiments and outputs
  - [ ] Safety considerations and limitations
  - [ ] Reproducible generation workflows
- [ ] Write Month 9 retrospective

**Month 9 Completion Criteria**
- [ ] Understands VAE, GAN, and diffusion tradeoffs
- [ ] Can run structured generation experiments
- [ ] Can evaluate quality with clear rubric
- [ ] Can document safety and practical constraints

## Best Free Resources by Week
- **Week 1 (VAE Foundations):**
  - Lilian Weng VAE explainer: https://lilianweng.github.io/posts/2018-08-12-vae/
  - PyTorch VAE example: https://github.com/pytorch/examples/tree/main/vae
- **Week 2 (GAN Basics + Stability):**
  - PyTorch DCGAN tutorial: https://pytorch.org/tutorials/beginner/dcgan_faces_tutorial.html
  - GAN Hacks (practical tips): https://github.com/soumith/ganhacks
- **Week 3 (Diffusion Models):**
  - Hugging Face Diffusers docs: https://huggingface.co/docs/diffusers/index
  - Annotated Diffusion blog: https://huggingface.co/blog/annotated-diffusion
- **Week 4 (Capstone + Comparison):**
  - Papers With Code image generation tasks: https://paperswithcode.com/task/image-generation
  - Weights & Biases reports/examples: https://wandb.ai/site/articles

## After Month 9
Continue with Month 10 in [learning-path/001-learning-path.md](learning-path/001-learning-path.md): reinforcement learning fundamentals and agents.
