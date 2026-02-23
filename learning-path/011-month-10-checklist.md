# Month 10 (Day 1–Day 30) — Reinforcement Learning Fundamentals

_Last updated: 23 Feb 2026_

## How to use this checklist
- Target: **2 to 3 hours/day**.
- Focus: RL intuition + reproducible experiments.
- Keep reward curves and configs for every run.

---

## Week 1 (Days 1–7): MDPs and Value-Based Basics

### Day 1
- [ ] Create `month-10-reinforcement-learning/` structure
- [ ] Set up Gymnasium and plotting utilities
- [ ] Choose initial simple environment (e.g., CartPole)
- [ ] Notes: state/action/reward definitions

### Day 2
- [ ] Study Markov Decision Process components
- [ ] Implement random policy baseline
- [ ] Run multiple episodes and log rewards
- [ ] Interpret baseline behavior

### Day 3
- [ ] Bellman equation intuition
- [ ] Implement tabular value iteration on toy gridworld
- [ ] Visualize value table updates
- [ ] Notes: convergence understanding

### Day 4
- [ ] Q-learning algorithm fundamentals
- [ ] Implement tabular Q-learning on simple env
- [ ] Tune epsilon-greedy exploration schedule
- [ ] Save reward curve

### Day 5
- [ ] Compare exploration strategies (epsilon schedules)
- [ ] Evaluate sample efficiency differences
- [ ] Add moving-average reward plots
- [ ] Document best setup

### Day 6
- [ ] Evaluate policy stability over seeds
- [ ] Report mean ± std return across runs
- [ ] Analyze variance sources
- [ ] Notes: reproducibility in RL

### Day 7 (Review)
- [ ] Rebuild tabular RL pipeline from scratch
- [ ] Week summary (1 page)
- [ ] Push code + plots
- [ ] Clean experiment outputs

**Week 1 Deliverable**
- [ ] Working tabular RL benchmark with Q-learning

---

## Week 2 (Days 8–14): Deep Q-Networks (DQN)

### Day 8
- [ ] Understand DQN architecture and replay buffer
- [ ] Implement DQN scaffold in PyTorch
- [ ] Validate action selection and buffer logic
- [ ] Notes: why replay helps

### Day 9
- [ ] Add target network mechanism
- [ ] Implement periodic target updates
- [ ] Train first DQN baseline
- [ ] Save reward/loss curves

### Day 10
- [ ] Tune core hyperparameters (LR, gamma, epsilon decay)
- [ ] Compare 3 controlled configurations
- [ ] Log stability and sample efficiency
- [ ] Update benchmark table

### Day 11
- [ ] Add gradient clipping and training safeguards
- [ ] Diagnose divergence cases
- [ ] Improve training reliability
- [ ] Document practical defaults

### Day 12
- [ ] Evaluate learned policy over multiple seeds
- [ ] Save evaluation protocol script
- [ ] Report confidence interval style summary
- [ ] Notes: avoiding overclaiming single-run results

### Day 13
- [ ] Optional DQN extensions (double DQN/dueling)
- [ ] Benchmark against baseline DQN
- [ ] Keep only if measurable gains
- [ ] Summarize complexity tradeoff

### Day 14 (Review)
- [ ] Reproduce best DQN run from clean config
- [ ] Week summary (1 page)
- [ ] Push milestone
- [ ] Organize model checkpoints

**Week 2 Deliverable**
- [ ] Stable DQN training pipeline with evaluation protocol

---

## Week 3 (Days 15–21): Policy Gradient and Actor-Critic (PPO Intuition)

### Day 15
- [ ] Study policy gradient intuition and objective
- [ ] Implement REINFORCE baseline on simple env
- [ ] Track variance and instability
- [ ] Notes: why baselines matter

### Day 16
- [ ] Add value baseline to reduce variance
- [ ] Compare with plain REINFORCE
- [ ] Save learning curves
- [ ] Record key improvements

### Day 17
- [ ] Understand actor-critic structure
- [ ] Implement simple actor-critic scaffold
- [ ] Validate policy/value losses
- [ ] Debug gradient flow

### Day 18
- [ ] Study PPO clipping intuition
- [ ] Run PPO using a trusted implementation or minimal version
- [ ] Compare with DQN on compatible task
- [ ] Log sample efficiency tradeoffs

### Day 19
- [ ] Tune PPO essentials (clip, LR, rollout length)
- [ ] Compare returns and stability over seeds
- [ ] Save best PPO config
- [ ] Notes: over-optimization warning signs

### Day 20
- [ ] Evaluate policy robustness to env variation (if feasible)
- [ ] Record degradation under changed settings
- [ ] Add practical reliability notes
- [ ] Update comparison table

### Day 21 (Review)
- [ ] Re-run best PPO setup cleanly
- [ ] Week summary (1 page)
- [ ] Push scripts/reports
- [ ] Consolidate figures

**Week 3 Deliverable**
- [ ] Policy-gradient/actor-critic benchmark with PPO reference

---

## Week 4 (Days 22–30): RL Capstone

### Day 22
- [ ] Define final capstone environment and success criteria
- [ ] Freeze evaluation protocol (episodes, seeds, metrics)
- [ ] Draft report structure
- [ ] Lock config templates

### Day 23
- [ ] Train value-based candidate (DQN family)
- [ ] Train policy-based candidate (PPO/actor-critic)
- [ ] Capture full learning curves
- [ ] Save checkpoints and configs

### Day 24
- [ ] Tune both candidates under fixed budget
- [ ] Run fair comparison with same evaluation standard
- [ ] Record sample efficiency and final return
- [ ] Update result tables

### Day 25
- [ ] Analyze failure modes (instability, variance, poor exploration)
- [ ] Add mitigation strategies
- [ ] Re-test with top fixes
- [ ] Capture deltas

### Day 26
- [ ] Build evaluation/inference script for trained policy
- [ ] Add deterministic and stochastic rollout modes
- [ ] Validate reproducibility across seeds
- [ ] Document usage

### Day 27
- [ ] Complete final RL report
- [ ] Include methods, tuning, comparisons, and risks
- [ ] Add caveats on environment generalization
- [ ] Polish plots and explanations

### Day 28
- [ ] Reproducibility audit on clean environment
- [ ] Verify training/evaluation commands end-to-end
- [ ] Fix docs/dependency issues
- [ ] Final code cleanup

### Day 29
- [ ] Prepare 5-minute capstone walkthrough
- [ ] Optional demo video
- [ ] Incorporate one feedback pass
- [ ] Tag final release

### Day 30 (Demo Day)
- [ ] Deliver Month 10 capstone:
  - [ ] Value-based vs policy-based RL comparison
  - [ ] Reproducible training and evaluation
  - [ ] Stability and variance analysis
  - [ ] Practical deployment notes
- [ ] Write Month 10 retrospective

**Month 10 Completion Criteria**
- [ ] Can explain MDP, value, policy, and exploration fundamentals
- [ ] Can train/evaluate DQN and PPO-style agents
- [ ] Can compare RL methods with fair protocols
- [ ] Can report RL uncertainty and limitations honestly

## Best Free Resources by Week
- **Week 1 (MDP + Q-Learning Basics):**
  - Sutton & Barto RL book (free): http://incompleteideas.net/book/the-book-2nd.html
  - David Silver RL course: https://www.davidsilver.uk/teaching/
- **Week 2 (DQN):**
  - DeepMind DQN paper: https://www.nature.com/articles/nature14236
  - CleanRL docs: https://docs.cleanrl.dev/
- **Week 3 (Policy Gradient + PPO):**
  - OpenAI Spinning Up PPO: https://spinningup.openai.com/en/latest/algorithms/ppo.html
  - Stable-Baselines3 docs: https://stable-baselines3.readthedocs.io/en/master/
- **Week 4 (RL Capstone):**
  - RL Baselines3 Zoo: https://github.com/DLR-RM/rl-baselines3-zoo
  - Gymnasium docs: https://gymnasium.farama.org/

## After Month 10
Continue with Month 11 in [learning-path/001-learning-path.md](learning-path/001-learning-path.md): MLOps and production AI systems.
