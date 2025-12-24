# Awesome Learning from Experience (LfE)

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of research papers and resources dedicated to **Learning from Experience** in AI. This list is organized by the **evolutionary stage** of the agent: from managing memory to abstracting skills, then reinforcement learning, continual learning, and finally to real-world applications.

![learn_from_experience](learn_from_experience.png)

## Contents

- [0. Foundations & Surveys](#0-foundations--surveys)
- [1. Dynamic Memory & Context](#1-dynamic-memory--context)
  - *The base layer: How agents store and refine their history.*
- [2. Experience-Driven Reasoning](#2-experience-driven-reasoning)
  - *The inference layer: Using the past to guide current thinking.*
- [3. Skill Acquisition & Abstraction](#3-skill-acquisition--abstraction)
  - *The abstraction layer: Turning traces into reusable tools/APIs.*
- [4. Reinforcement Learning & Optimization](#5-reinforcement-learning--optimization)
  - *The training layer: Hardening experience into policy/weights.*
- [5. Systemic Self-Evolution](#4-systemic-self-evolution)
  - *The lifecycle layer: Closed-loop agents that improve over time.*
- [6. Real-World Applications](#6-embodied--world-agents)
  - *The physical layer: Learning from interaction with environments.*
- [Benchmarks](#benchmarks)

---

## 0. Foundations & Surveys

* [![](https://img.shields.io/badge/2025-Note-blue)](https://storage.googleapis.com/deepmind-media/Era-of-Experience%20/The%20Era%20of%20Experience%20Paper.pdf) **Welcome to the Era of Experience** - *David Silver, Richard S. Sutton*
  * A visionary note proposing that agents will acquire superhuman capabilities predominantly by learning from experience.
* [![arXiv](https://img.shields.io/badge/2025.11-arXiv-b31b1b.svg)](https://arxiv.org/abs/2511.16660) **Cognitive Foundations for Reasoning and Their Manifestation in LLMs**
  * Synthesizes cognitive science into a taxonomy of 28 elements, highlighting the lack of meta-cognitive controls in current models.
* [![arXiv](https://img.shields.io/badge/2025.04-arXiv-b31b1b.svg)](https://arxiv.org/abs/2504.06943v2) **Review of Case-Based Reasoning for LLM Agents: Theoretical Foundations, Architectural Components, and Cognitive Integration**
  * A systematic review exploring how Case-Based Reasoning (CBR) integrates with LLMs.

## 1. Dynamic Memory & Context
*Focus: moving beyond static storage to memory that evolves, corrects itself, and adapts.*

* [![arXiv](https://img.shields.io/badge/2025.12-arXiv-b31b1b.svg)](http://arxiv.org/abs/2512.10696) **Remember Me, Refine Me: A Dynamic Procedural Memory Framework for Experience-Driven Agent Evolution**
  * Distills and refines procedural memory via utility-based pruning, allowing smaller models to outperform larger ones.
* [![arXiv](https://img.shields.io/badge/2025.08-arXiv-b31b1b.svg)](https://arxiv.org/abs/2508.06433v2) **Memp: Exploring Agent Procedural Memory**
  * Endows agents with a learnable, updatable procedural memory that evolves with new experiences.
* [![arXiv](https://img.shields.io/badge/2025.12-arXiv-b31b1b.svg)](http://arxiv.org/abs/2512.18746) **MemEvolve: Meta-Evolution of Agent Memory Systems**
  * A framework that evolves not just the content but the **memory architecture** itself to adapt to diverse task contexts.
* [![arXiv](https://img.shields.io/badge/2025.12-arXiv-b31b1b.svg)](http://arxiv.org/abs/2512.11485) **Mistake Notebook Learning: Selective Batch-Wise Context Optimization for In-Context Learning**
  * A training-free framework that abstracts error patterns from batch failures into a "notebook" to avoid repeating mistakes.
* [![arXiv](https://img.shields.io/badge/2025.10-arXiv-b31b1b.svg)](http://arxiv.org/abs/2510.08191) **Training-Free Group Relative Policy Optimization**
  * Learns experiential knowledge as a "token prior" to guide model behavior without parameter updates.

## 2. Experience-Driven Reasoning
*Focus: utilizing retrieved experience to optimize the reasoning path (CoT) at test time.*

* [![arXiv](https://img.shields.io/badge/2025.02-arXiv-b31b1b.svg)](http://arxiv.org/abs/2502.06772) **ReasonFlux: Hierarchical LLM Reasoning via Scaling Thought Templates**
  * Uses hierarchical RL and a library of thought templates to optimize reasoning paths, achieving SOTA on MATH.
* [![arXiv](https://img.shields.io/badge/2025.09-arXiv-b31b1b.svg)](http://arxiv.org/abs/2509.13237) **Metacognitive Reuse: Turning Recurring LLM Reasoning Into Concise Behaviors**
  * Converts recurring reasoning fragments into concise "behaviors" to reduce token usage and improve efficiency.
* [![arXiv](https://img.shields.io/badge/2025.12-arXiv-b31b1b.svg)](http://arxiv.org/abs/2512.17260) **Seed-Prover 1.5: Mastering Undergraduate-Level Theorem Proving via Learning from Experience**
  * Accumulates experience from interactions with Lean to master undergraduate-level theorem proving.
* [![arXiv](https://img.shields.io/badge/2025.12-arXiv-b31b1b.svg)](http://arxiv.org/abs/2512.10739) **Long-horizon Reasoning Agent for Olympiad-Level Mathematical Problem Solving**
  * Uses lemma-based memory to conduct multi-round hierarchical reasoning for IMO-level problems.
* [![arXiv](https://img.shields.io/badge/2025.12-arXiv-b31b1b.svg)](http://arxiv.org/abs/2512.06751) **Becoming Experienced Judges: Selective Test-Time Learning for Evaluators**
  * Allows evaluators to improve sequentially at inference time by maintaining an evolving meta-prompt.

## 3. Skill Acquisition & Abstraction
*Focus: the cognitive leap from "remembering what happened" to "learning a new skill/tool".*

* [![arXiv](https://img.shields.io/badge/2025.04-arXiv-b31b1b.svg)](https://arxiv.org/abs/2504.07079v1) **SkillWeaver: Web Agents can Self-Improve by Discovering and Honing Skills**
  * Agents autonomously synthesize reusable skills as APIs from exploration and practice.
* [![arXiv](https://img.shields.io/badge/2024.09-arXiv-b31b1b.svg)](http://arxiv.org/abs/2409.07429) **Agent Workflow Memory**
  * Induces commonly reused routines (workflows) from past experiences to guide future actions.
* [![arXiv](https://img.shields.io/badge/2025.04-arXiv-b31b1b.svg)](https://arxiv.org/abs/2504.06821v2) **Inducing Programmatic Skills for Agentic Tasks**
  * Demonstrates that programs are an effective representation for skills, allowing online verification.
* [![arXiv](https://img.shields.io/badge/2025.12-arXiv-b31b1b.svg)](http://arxiv.org/abs/2512.11303) **SMITH: Unifying Dynamic Tool Creation and Cross-Task Experience Sharing through Cognitive Memory Architecture**
  * Unifies dynamic tool creation with cross-task experience sharing through hierarchical memory.

## 4. Reinforcement Learning & Optimization
*Focus: The mathematical hardening of experience — RL, Gradients, and Policy Updates.*

* [![arXiv](https://img.shields.io/badge/2025.07-arXiv-b31b1b.svg)](http://arxiv.org/abs/2507.07451) **RLEP: Reinforcement Learning with Experience Replay for LLM Reasoning**
  * Blends newly generated rollouts with verified "success" trajectories during RL training to stabilize learning.
* [![arXiv](https://img.shields.io/badge/2025.11-arXiv-b31b1b.svg)](http://arxiv.org/abs/2511.03773) **Scaling Agent Learning via Experience Synthesis**
  * Introduces **DreamGym** to synthesize diverse experiences, enabling scalable online RL training without expensive rollouts.
* [![arXiv](https://img.shields.io/badge/2025.10-arXiv-b31b1b.svg)](http://arxiv.org/abs/2510.10304) **Sample-Efficient Online Learning in LM Agents via Hindsight Trajectory Rewriting**
  * Introduces **ECHO**, which uses hindsight experience replay to create synthetic positive examples from failed attempts.
* [![arXiv](https://img.shields.io/badge/2025.12-arXiv-b31b1b.svg)](http://arxiv.org/abs/2512.17102) **Reinforcement Learning for Self-Improving Agent with Skill Library**
  * Proposes **SAGE**, an RL framework that incorporates a skill library via sequential rollouts.
* [![arXiv](https://img.shields.io/badge/2025.11-arXiv-b31b1b.svg)](http://arxiv.org/abs/2511.19399) **DR Tulu: Reinforcement Learning with Evolving Rubrics for Deep Research**
  * Uses "Evolving Rubrics" that co-evolve with the policy to provide feedback for long-form research.
* [![arXiv](https://img.shields.io/badge/2025.10-arXiv-b31b1b.svg)](http://arxiv.org/abs/2510.08558) **Agent Learning via Early Experience**
  * Proposes using "early experience" (interaction data without rewards) for implicit world modeling.

## 5. Systemic Self-Evolution
*Focus: The "Agentic Lifecycle" — continuous loops of exploration, reflection, and self-update.*

* [![arXiv](https://img.shields.io/badge/2025.09-arXiv-b31b1b.svg)](http://arxiv.org/abs/2509.25140) **ReasoningBank: Scaling Agent Self-Evolving with Reasoning Memory**
  * Distills strategies from success and failure to guide "test-time scaling" for continuous improvement.
* [![arXiv](https://img.shields.io/badge/2025.10-arXiv-b31b1b.svg)](http://arxiv.org/abs/2510.16079) **EvolveR: Self-Evolving LLM Agents through an Experience-Driven Lifecycle**
  * Implements a closed-loop lifecycle of offline self-distillation and online interaction to refine strategies.
* [![arXiv](https://img.shields.io/badge/2025.11-arXiv-b31b1b.svg)](http://arxiv.org/abs/2511.10395) **AgentEvolver: Towards Efficient Self-Evolving Agent System**
  * Features self-questioning and self-navigating mechanisms to drive autonomous learning and reduce data costs.
* [![arXiv](https://img.shields.io/badge/2025.11-arXiv-b31b1b.svg)](http://arxiv.org/abs/2511.06449) **FLEX: Continuous Agent Evolution via Forward Learning from Experience**
  * A gradient-free paradigm that builds a structured experience library through continual reflection.
* [![arXiv](https://img.shields.io/badge/2025.11-arXiv-b31b1b.svg)](http://arxiv.org/abs/2511.23473) **ThetaEvolve: Test-time Learning on Open Problems**
  * Scales both in-context learning and RL at test time for open mathematical problems.
* [![arXiv](https://img.shields.io/badge/2025.12-arXiv-b31b1b.svg)](http://arxiv.org/abs/2512.15374) **SCOPE: Prompt Evolution for Enhancing Agent Effectiveness**
  * Frames context management as an online optimization problem, automatically evolving the agent's prompt.

## 6. Real-World Applications
*Focus: Applying LfE in environments where interaction is costly or complex.*

* [![arXiv](https://img.shields.io/badge/2025.11-arXiv-b31b1b.svg)](http://arxiv.org/abs/2511.14759) **$π^{*}_{0.6}$: a VLA That Learns From Experience**
  * Trains Vision-Language-Action models via RL by combining demonstrations, on-policy data, and corrections.
* [![arXiv](https://img.shields.io/badge/2025.11-arXiv-b31b1b.svg)](http://arxiv.org/abs/2511.09516) **MAP-VLA: Memory-Augmented Prompting for Vision-Language-Action Model in Robotic Manipulation**
  * Augments VLA models with a memory library derived from demonstrations using prompt tuning.
* [![arXiv](https://img.shields.io/badge/2025.12-arXiv-b31b1b.svg)](http://arxiv.org/abs/2512.19396) **EchoTrail-GUI: Building Actionable Memory for GUI Agents via Critic-Guided Self-Exploration**
  * Agents autonomously build a database of successful GUI interaction trajectories.
* [![arXiv](https://img.shields.io/badge/2025.11-arXiv-b31b1b.svg)](http://arxiv.org/abs/2511.21678) **Agentic Learner with Grow-and-Refine Multimodal Semantic Memory**
  * Introduces **ViLoMem**, a dual-stream memory (visual distraction vs. logical errors) for multimodal agents.
* [![arXiv](https://img.shields.io/badge/2025.11-arXiv-b31b1b.svg)](http://arxiv.org/abs/2511.19033) **ReEXplore: Improving MLLMs for Embodied Exploration with Contextualized Retrospective Experience Replay**
  * Uses retrospective experience replay and hierarchical frontier selection for embodied exploration.

## Benchmarks

* [![arXiv](https://img.shields.io/badge/2025.11-arXiv-b31b1b.svg)](http://arxiv.org/abs/2511.20857) **Evo-Memory: Benchmarking LLM Agent Test-time Learning with Self-Evolving Memory**
  * A streaming benchmark evaluating how well agents search, adapt, and evolve memory across sequential task streams.

---

## Contributing

Contributions are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details.
