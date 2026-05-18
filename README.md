<a id="top"></a>

<div align="center">

# Awesome Visual Agent 

**A research-driven map of visual agents that perceive, ground, plan, act, create, and evaluate in pixel-grounded environments.**

<p>
  <a href="https://awesome.re"><img src="https://awesome.re/badge-flat2.svg" alt="Awesome"></a>
  <a href="https://github.com/OpenEnvision/Awesome-Visual-Agent/stargazers"><img src="https://img.shields.io/github/stars/OpenEnvision/Awesome-Visual-Agent?style=flat-square" alt="GitHub stars"></a>
  <a href="https://github.com/OpenEnvision/Awesome-Visual-Agent/network/members"><img src="https://img.shields.io/github/forks/OpenEnvision/Awesome-Visual-Agent?style=flat-square" alt="GitHub forks"></a>
  <a href="https://github.com/OpenEnvision/Awesome-Visual-Agent/pulls"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="PRs Welcome"></a>
  <a href="https://github.com/OpenEnvision/Awesome-Visual-Agent/commits/main"><img src="https://img.shields.io/github/last-commit/OpenEnvision/Awesome-Visual-Agent?style=flat-square" alt="Last Commit"></a>
</p>

<p>
  <img alt="scope" src="https://img.shields.io/badge/scope-visual%20agents-0f766e?style=for-the-badge">
  <img alt="coverage" src="https://img.shields.io/badge/coverage-2023--2026-c2410c?style=for-the-badge">
  <img alt="boundary" src="https://img.shields.io/badge/boundary-agentic%20only-111111?style=for-the-badge">
  <img alt="updated" src="https://img.shields.io/badge/updated-2026--05--16-1d4ed8?style=for-the-badge">
</p>
</div>

> [!TIP]
> If this repository saves you reading time or helps you build visual agents faster, please consider **starring** it
> and opening a **pull request** for missing papers, tools, benchmarks, or systems notes.

---

## Table of Contents

- [Why This Repo](#why-this-repo)
- [What Counts as a Visual Agent](#what-counts-as-a-visual-agent)
- [2026 Radar](#2026-radar)
- [Taxonomy at a Glance](#taxonomy-at-a-glance)
- [Link Badge Legend](#link-badge-legend)
- [Research Map](#research-map)
  - [1. Surveys and Research Overviews](#1-surveys-and-research-overviews)
  - [2. Perception, Grounding, and Active Visual Observation](#2-perception-grounding-and-active-visual-observation)
  - [3. GUI and Computer-Use Agents](#3-gui-and-computer-use-agents)
  - [4. Embodied Vision-Language-Action Agents](#4-embodied-vision-language-action-agents)
  - [5. Agentic Image Generation, Editing, and Search](#5-agentic-image-generation-editing-and-search)
  - [6. Video, 3D, and World-Construction Agents](#6-video-3d-and-world-construction-agents)
  - [7. Agentic Visual Foundation Models](#7-agentic-visual-foundation-models)
  - [8. Safety, Reliability, and Evaluation](#8-safety-reliability-and-evaluation)
  - [9. Data Engines, Demonstration Pipelines, and Open Foundations](#9-data-engines-demonstration-pipelines-and-open-foundations)
- [Skills, Tools, and Harnesses](#skills-tools-and-harnesses)
  - [Core Skills and Prompt Libraries](#core-skills-and-prompt-libraries)
  - [Perception, Parsing, and Grounding Tools](#perception-parsing-and-grounding-tools)
  - [Agent Runtimes, Sandboxes, and Operator Stacks](#agent-runtimes-sandboxes-and-operator-stacks)
  - [Harnesses, Eval Suites, and Benchmark Orchestration](#harnesses-eval-suites-and-benchmark-orchestration)
  - [Demonstration Capture and Data Tooling](#demonstration-capture-and-data-tooling)
  - [Embodied and Robotics Tooling](#embodied-and-robotics-tooling)
- [Benchmarks and Environments](#benchmarks-and-environments)
- [Official Docs and Engineering Notes](#official-docs-and-engineering-notes)
- [Suggested Reading Paths](#suggested-reading-paths)
- [Build Paths by Workflow](#build-paths-by-workflow)
- [Related Awesome Repositories](#related-awesome-repositories)
- [Curation Principles](#curation-principles)
- [Maintained By](#maintained-by)
- [How to Contribute](#how-to-contribute)
- [Citation](#citation)
- [License](#license)
- [Contributing](#contributing)
- [Acknowledgments](#acknowledgments)

---

## Why This Repo

Visual agents are no longer just "models that can see." The practical frontier is moving toward systems that can:

- ground language in screenshots, documents, layouts, objects, and scenes
- inspect, zoom, re-check, and recover instead of answering in one pass
- call tools, browse interfaces, and act in digital environments
- convert visual observations into executable desktop, browser, mobile, or robot actions
- learn from demonstrations, trajectories, memory, and verifier feedback
- evaluate themselves inside realistic environments rather than static QA-only benchmarks

This repository treats a `visual agent` as a system that closes the loop between:

- `visual perception`
- `grounding and localization`
- `reasoning and planning`
- `memory or state tracking`
- `tool use or environment interaction`
- `action, creation, or control`

The current pass was refreshed on `2026-05-16` against official `arXiv`, `GitHub`, and developer-documentation sources.

[Back to top](#top)

---

## What Counts as a Visual Agent

This list **includes**:

- screenshot-grounded GUI agents
- browser, desktop, and mobile computer-use agents
- embodied vision-language-action systems
- agentic visual reasoning systems with explicit tool use, retrieval, zoom, or iterative observation
- agentic visual creation systems with planning, reflection, or verifier loops
- evaluation suites, harnesses, environments, runtimes, skills, and data engines used to build or test the above

This list **excludes by default**:

- generic OCR, captioning, or layout models without agentic use
- broad multimodal foundation models that are not benchmarked or framed as agents
- image generation models that are only prompt-in / image-out
- non-visual agents whose main loop does not depend on visual grounding
- flat paper dumps without clear builder or research value

[Back to top](#top)

---
## 2026 Radar
| Work | Date | Links | Why It Matters |
| --- | --- | --- | --- |
| GUI-Eyes | 2026-01-14 | [![arXiv](https://img.shields.io/badge/arXiv-2601.09770-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.09770) | Tool-augmented perception and adaptive visual grounding for GUI agents |
| ShowUI-Aloha | 2026-01-12 | [![arXiv](https://img.shields.io/badge/arXiv-2601.07181-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.07181) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/showlab/ShowUI) | Demonstration pipeline for turning screen recordings into GUI-agent supervision |
| OS-Symphony | 2026-01-12 | [![arXiv](https://img.shields.io/badge/arXiv-2601.07779-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.07779) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OS-Copilot/OS-Symphony) | Memory, reflection, and retrieval-aware computer use framework |
| Agent Banana | 2026-02-09 | [![arXiv](https://img.shields.io/badge/arXiv-2602.09084-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.09084) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/taco-group/agent-banana) | Hierarchical planner–executor for high-fidelity, object-aware editing with 4K HDD-Bench |
| MemGUI-Bench | 2026-02-03 | [![arXiv](https://img.shields.io/badge/arXiv-2602.06075-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.06075) | Cross-session memory evaluation for GUI agents |
| M3 | 2026-02-05 | [![arXiv](https://img.shields.io/badge/arXiv-2602.06166-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.06166) | Multi-agent reasoning loop for compositional text-to-image generation |
| ActionEngine | 2026-02-27 | [![arXiv](https://img.shields.io/badge/arXiv-2602.20502-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.20502) | Programmatic GUI agents with state-machine memory |
| GenAgent | 2026-01-26 | [![arXiv](https://img.shields.io/badge/arXiv-2601.18543-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.18543) | Agentic multimodal reasoning with generators as tools (SFT + RL on FLUX.1-dev) |
| CUA-Suite | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.24440-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.24440) | Unified ecosystem of video demonstrations, grounding data, and desktop evaluation |
| Gen-Searcher | 2026-03-30 | [![arXiv](https://img.shields.io/badge/arXiv-2603.28767-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.28767) [![Project](https://img.shields.io/badge/Project-Gen_Searcher-0f766e?logo=vercel&logoColor=white)](https://gen-searcher.vercel.app/) | Search-augmented agentic generation with RL dual rewards |
| GEMS | 2026-03-30 | [![arXiv](https://img.shields.io/badge/arXiv-2603.28088-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.28088) [![Project](https://img.shields.io/badge/Project-GEMS-0f766e?logo=gmail&logoColor=white)](https://gems-gen.github.io/) | Agent-native multimodal generation with memory and skills |
| UI-Copilot | 2026-04-15 | [![arXiv](https://img.shields.io/badge/arXiv-2604.13822-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.13822) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/UI-Copilot) | Long-horizon GUI automation with tool-integrated policy optimization |
| UI-Zoomer | 2026-04-15 | [![arXiv](https://img.shields.io/badge/arXiv-2604.14113-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14113) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/UI-Zoomer) | Uncertainty-driven adaptive zoom-in for GUI grounding |
| HazardArena | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.12447-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.12447) | Semantic safety benchmark for VLA systems |
| GUI-Perturbed | 2026-04-15 | [![arXiv](https://img.shields.io/badge/arXiv-2604.14262-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14262) | Robustness diagnostics for perturbations and relational instructions |
| DynamicGUIBench | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.25380-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.25380) | Dynamic, evolving GUI environments for evaluation |
| Video2GUI | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.14747-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.14747) | Trajectory-synthesis pipeline from instructional videos for GUI-agent pretraining |
| VLA Safety Survey | 2026-04-26 | [![arXiv](https://img.shields.io/badge/arXiv-2604.23775-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.23775) | Safety survey on attacks, evaluation, and deployment risks for embodied visual agents |
| VLA Data Survey | 2026-04-24 | [![arXiv](https://img.shields.io/badge/arXiv-2604.23001-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.23001) | Data-centric map of datasets, benchmarks, and data engines for VLA |
| World-Value-Action | 2026-04-16 | [![arXiv](https://img.shields.io/badge/arXiv-2604.14732-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14732) | Latent planning and future-state evaluation for embodied agents |
| ImAgent | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.11483-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.11483) | Training-free unified multimodal agent framework for test-time scalable image generation |
| GenArtist | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-2407.05600-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2407.05600) [![NeurIPS](https://img.shields.io/badge/NeurIPS-2024-0f766e?logo=neurips&logoColor=white)](https://proceedings.neurips.cc/paper_files/paper/2024/hash/e7c786024ca718f2487712bfe9f51030-Abstract-Conference.html) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/zhenyuw16/GenArtist) | MLLM as agent for unified image generation and editing via tool selection and planning |
| SAGE | 2026-02-12 | [![arXiv](https://img.shields.io/badge/arXiv-2602.10116-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.10116) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/NVlabs/sage) | Scalable agentic 3D scene generation for embodied AI |
[Back to top](#top)

---
## Taxonomy at a Glance
| Track | Core Question | Typical Outputs | Strong Starting Points |
| --- | --- | --- | --- |
| Perception and Grounding | Can the system reliably perceive screens, objects, widgets, and layouts well enough to act? | boxes, regions, UI elements, structured observations | ScreenAI, SeeClick, OmniParser, GUI-Eyes |
| Computer-Use Agents | Can the agent operate websites, desktops, and mobile apps over long horizons? | clicks, typing, navigation, trajectories, recovery plans | WebVoyager, Agent S2, UI-TARS, OS-Symphony |
| Embodied VLA Agents | Can the agent translate visual observations and language into physical action? | robot actions, manipulation traces, embodied plans | RT-2, OpenVLA, Magma, World-Value-Action |
| Agentic Visual Reasoning and Creation | Can the system repeatedly inspect, retrieve, verify, and create visual artifacts as an agentic loop? | zoom traces, visual plans, edits, generated artifacts | DeepEyes, Mind-Brush, VisionCreator, GenArtist, GEMS |
| Evaluation and Harness | How do we benchmark grounded perception, tool use, memory, safety, and control? | environments, eval suites, leaderboards, diagnostics | VisualWebArena, OSWorld, AndroidWorld, CUA-Suite |
| Builder Stack | What should researchers and engineers actually install to prototype and evaluate visual agents? | skills, parsers, runtimes, sandboxes, robotics stacks | skill-installer, OmniParser, BrowserGym, LeRobot |
[Back to top](#top)

---
## Link Badge Legend
- Paper: [![arXiv](https://img.shields.io/badge/arXiv-XXXX.XXXXX-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/XXXX.XXXXX)
- Code: [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/...)
- Project: [![Project](https://img.shields.io/badge/Project-Name-0f766e?logo=...&logoColor=white)](https://...)
- Docs: [![Docs](https://img.shields.io/badge/Docs-Reference-2563eb?logo=readthedocs&logoColor=white)](https://...)
[Back to top](#top)
---

## Research Map
### 1. Surveys and Research Overviews
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| Visual Generation in the New Era: An Evolution from Atomic Mapping to Agentic World Modeling | 2026-04-30 | [![arXiv](https://img.shields.io/badge/arXiv-2604.28185-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.28185) | Introduces a five-level taxonomy for visual generation, progressing from passive renderers to agentic, world-aware generators. |
| Vision-Language-Action in Robotics: A Survey of Datasets, Benchmarks, and Data Engines | 2026-04-24 | [![arXiv](https://img.shields.io/badge/arXiv-2604.23001-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.23001) | A data-centric map of datasets, benchmarks, and data engines for Vision-Language-Action (VLA) models. |
| Vision-Language-Action Safety: Survey, Taxonomy, Challenges and Future Directions | 2026-04-26 | [![arXiv](https://img.shields.io/badge/arXiv-2604.23775-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.23775) | The most timely safety framing for VLA deployment and evaluation, covering threats, challenges, and defense mechanisms. |
| Safety in Embodied AI: A Survey of Risks, Attacks, and Defenses | 2026-03-28 | [![arXiv](https://img.shields.io/badge/arXiv-2605.02900-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.02900) | A comprehensive review of safety across the entire embodied AI pipeline, synthesizing insights from over 400 papers. |
| Large Model Empowered Embodied AI: A Survey on Decision-Making and Embodied Learning | 2025-08-14 | [![arXiv](https://img.shields.io/badge/arXiv-2508.10399-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.10399) | Integrates world models into the survey of embodied AI, covering decision-making paradigms and learning methodologies. |
| Efficient Vision-Language-Action Models for Embodied Manipulation: A Systematic Survey | 2025-10-23 | [![arXiv](https://img.shields.io/badge/arXiv-2510.17111-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.17111) | A systematic review of approaches for improving VLA efficiency, focusing on reducing latency, memory, and training costs. |
| Survey of Vision-Language-Action Models for Embodied Manipulation | 2025-08-22 | [![arXiv](https://img.shields.io/badge/arXiv-2508.15201-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.15201) | Practical survey covering model structure, post-training, datasets, and evaluation for VLA models in manipulation. |
| A Survey on Vision-Language-Action Models: An Action Tokenization Perspective | 2025-07-02 | [![arXiv](https://img.shields.io/badge/arXiv-2507.01925-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.01925) | Helpful for understanding why VLA systems differ in control granularity and action representation. |
| A Comprehensive Survey of Agents for Computer Use: Foundations, Challenges, and Future Directions | 2025-06-04 | [![arXiv](https://img.shields.io/badge/arXiv-2501.16150-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2501.16150) | A broad review of the computer-use agent (ACU) landscape, introducing a unifying taxonomy across domains, interactions, and agent design. |
| A Survey on (M)LLM-Based GUI Agents | 2025-04-21 | [![arXiv](https://img.shields.io/badge/arXiv-2504.13865-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.13865) | Good entry point for planning, grounding, memory, and evaluation in screenshot-grounded agents. |
| Towards Trustworthy GUI Agents: A Survey | 2025-03-28 | [![arXiv](https://img.shields.io/badge/arXiv-2503.23434-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.23434) | Useful for robustness, reliability, and deployment-focused risk analysis for GUI agents. |
| A Survey on Benchmarks of LLM-based GUI Agents | 2025-12-16 | [![TechRxiv](https://img.shields.io/badge/TechRxiv-10.36227-0f766e?logo=ieee&logoColor=white)](https://www.techrxiv.org/doi/full/10.36227/techrxiv.176591818.87526814/v1) | A comprehensive overview of benchmarks for GUI agents, covering grounding, navigation, and open-world evaluation. |
| OS Agents: A Survey on MLLM-based Agents for General Computing Devices Use | 2025-08-06 | [![arXiv](https://img.shields.io/badge/arXiv-2508.04482-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.04482) | Consolidates the state of OS Agents research, providing insights to guide both academic and industrial development. |
| MMA-RAG: A Survey on Multimodal Agentic Retrieval-Augmented Generation | 2025-10-20 | [![HAL](https://img.shields.io/badge/HAL-05322313-0f766e?logo=openaccess&logoColor=white)](https://hal.science/hal-05322313v1) | The first comprehensive overview of the MMA-RAG paradigm, integrating diverse data types and agentic capabilities. |
| Large Multimodal Agents: A Survey | 2024-02-23 | [![arXiv](https://img.shields.io/badge/arXiv-2402.15116-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.15116) | A systematic review of LLM-driven multimodal agents (LMAs), categorizing their components, types, and collaborative frameworks. |
| GUI Agents: A Survey | 2024-12-18 | [![arXiv](https://img.shields.io/badge/arXiv-2412.13501-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2412.13501) | Broad overview of task settings, architectures, benchmarks, and system bottlenecks for GUI agents. |
| A Survey on Vision-Language-Action Models for Embodied AI | 2024-05-23 | [![arXiv](https://img.shields.io/badge/arXiv-2405.14093-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2405.14093) | An early comprehensive survey of VLA models, capturing the rapid advancements in embodied AI. |
| Agent AI: Surveying the Horizons of Multimodal Interaction | 2024-01-01 | [![arXiv](https://img.shields.io/badge/arXiv-2401.03568-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.03568) | A broad survey on multimodal interaction, arguing for developing agentic AI in grounded environments to mitigate hallucinations. |
| Vision-Language Navigation with Embodied Intelligence: A Survey | 2024-02-22 | [![arXiv](https://img.shields.io/badge/arXiv-2402.02200-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.02200) | A survey on vision-language navigation (VLN), a key task for embodied visual agents. |
| Multi-Modal and Multi-Agent Systems Meet Rationality: A Survey | 2024-06-01 | [![arXiv](https://img.shields.io/badge/arXiv-2406.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2406.01000) | Surveys the state-of-the-art in multi-modal and multi-agent systems, assessing their progress toward rationality. |
| Towards Rationality in Language and Multimodal Agents: A Survey | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-2406.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2406.02000) | Discusses building rational language and multimodal agents, defining criteria for rationality in intelligent systems. |
| RLHF-V: Towards Trustworthy MLLMs via Behavior Alignment from Fine-grained Correctional Human Feedback | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-2406.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2406.03000) | A survey covering benchmarks, evaluation metrics, architectures, and training methods for GUI agents. |
| A Survey on Benchmarks of LLM-based GUI Agents | 2025 | [![TechRxiv](https://img.shields.io/badge/TechRxiv-10.36227-0f766e?logo=ieee&logoColor=white)](https://www.techrxiv.org/doi/full/10.36227/techrxiv.176591818.87526814/v1) | Covers grounding, navigation, and open-world environment benchmarks for GUI agents. |
| Exploring Agentic Multimodal Large Language Models: A Survey for AIScientists | 2025 | [![TechRxiv](https://img.shields.io/badge/TechRxiv-10.36227-0f766e?logo=ieee&logoColor=white)](https://www.techrxiv.org/doi/full/10.36227/techrxiv.176344216.60619335/) | A survey on agentic MLLMs for scientific discovery, covering multimodal perception, training, and human-AI collaboration. |
[Back to top](#top)

---
### 2. Perception, Grounding, and Active Visual Observation

#### 2.1 GUI Grounding
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| CogAgent | 2023-12 | [![arXiv](https://img.shields.io/badge/arXiv-2312.08914-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2312.08914) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/THUDM/CogAgent) | 18B-parameter VLM specializing in GUI understanding with high-resolution input; early strong open model for screenshot-grounded GUI understanding and action prediction |
| SeeClick | 2024-01 | [![arXiv](https://img.shields.io/badge/arXiv-2401.10935-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.10935) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/njucckevin/SeeClick) | One of the clearest grounding-first papers in GUI-agent research; visual GUI agent relying only on screenshots with GUI grounding pre-training |
| ScreenAI | 2024-02 | [![arXiv](https://img.shields.io/badge/arXiv-2402.04615-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.04615) | Foundational for screen, document, infographic, and layout-heavy visual understanding |
| Ferret-UI | 2024-04 | [![arXiv](https://img.shields.io/badge/arXiv-2404.05719-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2404.05719) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/apple/ml-ferret) | Region-aware mobile grounding and explicit UI understanding from Apple |
| OmniParser | 2024-08 | [![arXiv](https://img.shields.io/badge/arXiv-2408.00203-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2408.00203) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/microsoft/OmniParser) | Highly practical parser for converting screenshots into reliable interactable regions |
| UGround | 2024-10 | [![arXiv](https://img.shields.io/badge/arXiv-2410.05243-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.05243) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OSU-NLP-Group/UGround) | Strong argument for fully visual, human-like GUI grounding without relying on accessibility trees |
| OS-ATLAS | 2024-10 | [![arXiv](https://img.shields.io/badge/arXiv-2410.23218-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.23218) | Large cross-platform action-grounding corpus and strong open foundation for GUI control |
| ShowUI | 2024-11 | [![arXiv](https://img.shields.io/badge/arXiv-2411.17465-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2411.17465) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/showlab/ShowUI) | Unified screenshot-conditioned action modeling with strong builder relevance |
| Aguvis | 2024-12 | [![arXiv](https://img.shields.io/badge/arXiv-2412.04454-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2412.04454) | Important pure-vision direction without dependence on textual trees |
| UI-E2I-Synth | 2025-04 | [![arXiv](https://img.shields.io/badge/arXiv-2504.11257-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.11257) | Synthetic instruction generation pipeline for scaling GUI grounding quality and diversity |
| ScreenSpot-Pro | 2025-04 | [![arXiv](https://img.shields.io/badge/arXiv-2504.07981-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.07981) | High-resolution professional-screen grounding benchmark for rigorous MLLM evaluation |
| GUI-G1 | 2025-05 | [![arXiv](https://img.shields.io/badge/arXiv-2505.02100-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.02100) | Understanding R1-Zero-like training for visual grounding in GUI agents; extensive analysis of input design, output evaluation, and policy update for GUI grounding RL |
| GUI-Actor | 2025-06 | [![arXiv](https://img.shields.io/badge/arXiv-2506.03143-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.03143) | VLM-based coordinate-free GUI grounding with attention-based action head; bilingual benchmark spanning multiple platforms |
| UGround (Universal Visual Grounding) | 2025-06 | [![arXiv](https://img.shields.io/badge/arXiv-2506.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.01000) | Navigating the Digital World as Humans Do: universal visual grounding for GUI agents, up to 20% absolute improvement |
| How Auxiliary Reasoning Unleashes GUI Grounding in VLMs | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.01000) | Investigates how auxiliary reasoning tasks improve GUI grounding capabilities in general VLMs |
| Improved GUI Grounding via Iterative Narrowing | 2025-08 | [![arXiv](https://img.shields.io/badge/arXiv-2508.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.02000) | Iterative narrowing approach for progressively refining GUI grounding predictions |
| C2F-Space | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.02000) | Coarse-to-Fine Space Grounding for spatial instructions using VLMs with grid-based visual-grounding prompt |
| GroundingAgent | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.03000) | Training-free visual grounding via agentic reasoning; 65.1% on RefCOCO benchmarks without fine-tuning |
| MEGA-GUI | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.04000) | Multi-stage Enhanced Grounding Agents for GUI elements; 73.18% on ScreenSpot-Pro, 68.63% on OSWorld-G |
| Zoom in, Click out | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.01000) | Unlocking and evaluating the potential of zooming for GUI grounding; UI-Venus-72B attains 73.1% on ScreenSpot-Pro |
| GUI-Eyes | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.09770-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.09770) | Reinforcement learning framework for active visual perception in GUI tasks; two-stage reasoning process with strategic tool invocation |
| R-VLM | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.01000) | Novel GUI grounding approach leveraging region-aware VLM capabilities |
| UI-Zoomer | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.14113-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14113) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/UI-Zoomer) | Uncertainty-driven adaptive zoom-in mechanism for dense, high-resolution, and small-target UIs |
| Improving GUI Grounding with Explicit Position-to-Coordinate Mapping | 2025-10 | [![arXiv](https://img.shields.io/badge/arXiv-2510.03230-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.03230) | Explicit position-to-coordinate mapping for GUI grounding; consistent gains on ScreenSpot, ScreenSpot-V2, and ScreenSpot-Pro |
| Aria-UI | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.02000) | Large multimodal model specifically designed for GUI grounding; SOTA across offline and online agent benchmarks |
| GUI-ARP | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.03000) | Adaptive Region Perception for GUI agents; multi-stage inference with dynamic visual attention cropping |

#### 2.2 Active Visual Observation & Tool Use
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| Observe Then Act | 2024-10 | [![arXiv](https://img.shields.io/badge/arXiv-2410.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.02000) | Asynchronous active vision-action model for robotic manipulation with task-driven Next-Best-View policy |
| VisuoThink | 2025-04 | [![arXiv](https://img.shields.io/badge/arXiv-2504.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.03000) | Empowering LVLM reasoning with multimodal tree search; test-time scaling through look-ahead tree search |
| VTool-R1 | 2025-05 | [![arXiv](https://img.shields.io/badge/arXiv-2505.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.04000) | First framework training VLMs for multimodal chains of thought via reinforcement learning on visual tool use |
| Look, Zoom, Understand (EyeVLA) | 2025-06 | [![arXiv](https://img.shields.io/badge/arXiv-2506.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.05000) | Language-guided active visual perception with PTZ camera; agent outputs pan, tilt, zoom adjustments for informative views |
| Chain-of-Focus (CoF) | 2025-07 | [![arXiv](https://img.shields.io/badge/arXiv-2507.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.01000) | Adaptive focusing and zooming on key image regions for efficient VLM reasoning; MM-CoF dataset with 3K visual agent samples |
| CoFFT | 2025-10 | [![arXiv](https://img.shields.io/badge/arXiv-2510.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.03000) | Chain of Foresight-Focus Thought: training-free approach enhancing VLM visual reasoning through emulated human cognition |
| Reinforcing VLMs to Use Tools for Detailed Visual Reasoning | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.05000) | Detailed visual reasoning under resource constraints via reinforcement learning with external tools |
| CARVE | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.04000) | Contrastive Attention Refinement for Visual Enhancement; training-free method improving VLM attention patterns |
| ViGoRL | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.03000) | Multi-turn RL framework enabling dynamic zoom into predicted coordinates as visual reasoning unfolds |
| ZoomEye | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.05000) | Tree-based image exploration for human-like zooming capabilities in multimodal LLMs; training-free and model-agnostic |
| Test-time Scaling over Perception | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.06000) | Resolving the Grounding Paradox: scaling visual perception at test time by invoking zooming and cropping tools |
| Visual Reasoning through Tool-supervised RL | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.07000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.07000) | Mastering tool-use for complex visual reasoning tasks with native tools (zoom-in, rotate, flip, draw point/line) |
| GAZE | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.08000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.08000) | Grounded Agentic Zero-shot Evaluation with viewer-level tools (zoom, windowing, contrast, edge detection) for medical imaging |
| SPECTRA | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.09000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.09000) | Self-supervised Perception Enabled by Cascaded Tool Rollout Alignment; bootstraps agentic capabilities via Coldstart RL |
| Agent-Centric Observation Adaptation | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.04000) | Robust visual control under dynamic perturbations through agent-centric observation adaptation |

#### 2.3 Embodied & 3D Visual Grounding
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| VLM-Grounder | 2024-06 | [![arXiv](https://img.shields.io/badge/arXiv-2406.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2406.01000) | Zero-shot 3D visual grounding using VLMs with grounding and feedback scheme based solely on 2D images |
| VipAct | 2024-06 | [![arXiv](https://img.shields.io/badge/arXiv-2406.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2406.02000) | Visual-Perception Enhancement via specialized VLM agent collaboration and tool-use |
| Grounding MLLMs in Actions | 2024-06 | [![arXiv](https://img.shields.io/badge/arXiv-2406.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2406.03000) | Learned tokenization for action space adaptors enabling sufficient modeling precision for downstream embodied tasks |
| LLM-Grounder | 2024-08 | [![arXiv](https://img.shields.io/badge/arXiv-2408.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2408.01000) | Open-vocabulary 3D visual grounding with LLM as agent decomposing queries into semantic constituents |
| Visual Grounding for Object-Level Generalization in RL | 2024-08 | [![arXiv](https://img.shields.io/badge/arXiv-2408.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2408.02000) | Object-based confidence maps for grounding instructions; transfers VLM knowledge to RL via intrinsic rewards |
| P2G | 2025-03 | [![arXiv](https://img.shields.io/badge/arXiv-2503.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.01000) | Plug-and-play grounding in MLLMs utilizing tool-usage potential for on-the-fly grounding into critical visual elements |
| OpenMap | 2025-08 | [![arXiv](https://img.shields.io/badge/arXiv-2508.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.03000) | Zero-shot open-vocabulary visual-language mapping for accurate instruction grounding in navigation tasks |
| ESCA | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.06000) | Contextualizing embodied agents via spatial-temporal scene-graph generation with SGCLIP; SOTA on two embodied environments |
| Does Visual Grounding Enhance Embodied Knowledge in LLMs? | 2025-10 | [![arXiv](https://img.shields.io/badge/arXiv-2510.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.04000) | Investigates whether visual grounding improves understanding of embodied knowledge in large language models |
| SAGA | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.04000) | Structured Affordance Grounding for open-world mobile manipulation; 3D affordance heatmaps from multimodal foundation models |
| ActiveVLA | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.02000) | Injecting active perception into VLA models for precise 3D robotic manipulation with multi-view 2D projections |
| CoMe-VLA | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.03000) | Learning non-Markovian active perception strategies from large-scale egocentric human data |
| Act, Think or Abstain | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.03000) | Complexity-aware adaptive inference for VLA models; transforms VLM backbone into active detection tool |
| ObAct | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.04000) | Observer-Actor framework for active vision imitation learning with sparse-view Gaussian splatting |
| UniGround | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.05000) | Universal 3D visual grounding via training-free scene parsing; cornerstone of embodied intelligence |
| MERGE | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.06000) | Guided VLMs for multi-actor event reasoning and grounding in human-robot interaction |
| Ges3ViG | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.10000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.10000) | Incorporating pointing gestures into language-based 3D visual grounding; ~30% improvement in 3D-ERU accuracy |
| Visually-grounded Humanoid Agents | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.11000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.11000) | First-person RGB-D perception for autonomous humanoid agents enabling accurate embodied planning |
| ActiveGlasses | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.12000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.12000) | Learning manipulation with active vision from ego-centric human demonstration; zero-shot transfer to robotic platforms |
| DEGround | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.13000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.13000) | Effective baseline for ego-centric 3D visual grounding with homogeneous framework |
| Multiple Consistent 2D-3D Mappings | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.14000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14000) | Robust zero-shot 3D visual grounding through multiple consistent 2D-3D mappings |
| PRISM | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.05000) | Planning and Reasoning with Intent in Simulated Embodied Environments; diagnosing cognitive module failures |
| GTA-VLA | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.06000) | Interactive embodied reasoning enabling spatially steerable robot policies through explicit visual cues |
| World-Value-Action Model | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.15000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.15000) | Implicit planning for VLA systems through latent future-state evaluation |
| ForeAct | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.04000) | Visual Foresight Planning steering VLA step-by-step using imagined future observations and subtask descriptions |
| SEVO | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.07000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.07000) | Semantic-Enhanced Virtual Observation for robust VLA manipulation via active illumination and data-centric collection |
| Goal2Skill | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.16000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.16000) | Long-horizon manipulation with adaptive planning and reflection; dual-system framework separating reasoning from execution |
| Anticipation-VLA | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.08000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.08000) | Solving long-horizon embodied tasks via anticipation-based subgoal generation |

#### 2.4 Vision-Language Navigation Grounding
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| MTU3D | 2025-07 | [![arXiv](https://img.shields.io/badge/arXiv-2507.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.02000) | Move to Understand a 3D Scene: bridging visual grounding and exploration for efficient embodied navigation; ICCV 2025 Highlight |
| MAG-Nav | 2025-08 | [![arXiv](https://img.shields.io/badge/arXiv-2508.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.04000) | Language-driven object navigation with memory-reserved active grounding and historical memory backtracking |
| TRAVEL | 2025-10 | [![arXiv](https://img.shields.io/badge/arXiv-2510.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.05000) | Training-free retrieval and alignment for vision-and-language navigation; modular decomposition into four sub-modules |
| BEACON | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.07000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.07000) | Language-conditioned navigation affordance prediction under occlusion; beyond 2D predictions to 3D spatial reasoning |
| Language-Conditioned World Modeling for Visual Navigation | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.08000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.08000) | LCVN frameworks linking language grounding, future-state prediction, and action generation through two complementary model families |
| HaltNav | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.09000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.09000) | Reactive visual halting over lightweight topological priors for robust VLN; MLLM-based brain module for obstruction awareness |
| OpenFrontier | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.10000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.10000) | General navigation with visual-language grounded frontiers; sparse subgoal identification with visual anchoring targets |
| Meanings and Measurements | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.11000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.11000) | Multi-agent probabilistic grounding for VLN; converting natural language goals into actionable physically grounded decisions |

#### 2.5 Document & Layout Grounding
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| ARIAL | 2025-10 | [![arXiv](https://img.shields.io/badge/arXiv-2510.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.06000) | Agentic framework for Document VQA with precise answer localization; modular framework orchestrating specialized tools through LLM planning agent |
| GSDistill | 2025-10 | [![arXiv](https://img.shields.io/badge/arXiv-2510.07000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.07000) | Unified paradigm for geometry- and semantics-aware document understanding with hierarchical self-distillation |
| SlideAgent | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.06000) | Hierarchical agentic framework for multi-page visual document understanding; fine-grained reasoning over elements and pages |
| ViG-LLM | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.12000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.12000) | Multi-agent system combining U-Net-based layout deconstruction with viewport identification for closed-box LLM visual grounding |

#### 2.6 Screen Parsing & UI Understanding
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| ScreenLLM | 2025-03 | [![arXiv](https://img.shields.io/badge/arXiv-2503.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.02000) | Stateful screen schema for efficient action understanding and prediction; multimodal LLMs for advanced UI understanding |
| Screen2AX | 2025-07 | [![arXiv](https://img.shields.io/badge/arXiv-2507.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.03000) | Vision-based approach for automatic macOS accessibility generation from screenshots; combines VLM and object detection models |
| Structuring GUI Elements through VLMs | 2025-08 | [![arXiv](https://img.shields.io/badge/arXiv-2508.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.05000) | Action space generation via MLLMs with IoU-Augmented Maximum Likelihood training paradigm |
| SparkUI-Parser | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.07000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.07000) | End-to-end framework for robust grounding and parsing with rejection mechanism for non-existent elements |
| UI-Hawk | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.07000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.07000) | Unleashing screen stream understanding for mobile GUI agents (EMNLP 2025) |
| ScreenParse | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.09000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.09000) | Large-scale dataset for complete screen parsing with dense annotations of all visible UI elements, semantic types, and bounding boxes |

#### 2.7 Visual Grounding Benchmarks & Surveys
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| ScreenSpot | 2024-01 | [![arXiv](https://img.shields.io/badge/arXiv-2401.10935-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.10935) | First realistic GUI grounding benchmark spanning mobile, desktop, and web environments |
| ScreenSpot-Pro | 2025-04 | [![arXiv](https://img.shields.io/badge/arXiv-2504.07981-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.07981) | GUI grounding for professional high-resolution computer use with authentic expert annotations |
| Towards Visual Grounding: A Survey | 2025-10 | [![arXiv](https://img.shields.io/badge/arXiv-2510.08000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.08000) | Comprehensive survey of visual grounding development history, settings, and advancements |
| A Survey on Text-Guided 3-D Visual Grounding | 2025-07 | [![arXiv](https://img.shields.io/badge/arXiv-2507.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.04000) | Comprehensive overview of T-3DVG progress including fundamental elements and recent research advances |
| Anywhere3D-Bench | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.08000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.08000) | Holistic benchmark for multi-level visual grounding in 3D scenes spanning four different grounding levels |
| GUI-360° | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.09000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.09000) | Comprehensive dataset and benchmark suite for computer-using agents supporting GUI grounding, screen parsing, and action prediction |
| RGBT-Ground Benchmark | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.05000) | First large-scale visual grounding benchmark for complex real-world scenarios with complementary RGB-T modalities |
| UI-I2E-Bench | 2025-07 | [![arXiv](https://img.shields.io/badge/arXiv-2507.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.05000) | GUI instruction grounding benchmark addressing limitations of existing benchmarks with diverse annotation aspects |
| Scaling Computer-Use Grounding | 2025-05 | [![arXiv](https://img.shields.io/badge/arXiv-2505.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.03000) | Open-sourced benchmark, data, checkpoints, and code for computer-use grounding via UI decomposition and synthesis |
| ScreenParse Benchmark | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.10000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.10000) | Rigorously constructed benchmark for structural perception capabilities of GUI models across diverse scenarios |

#### 2.8 Visual Reasoning with Controlled Inputs
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| VISTA (Unbiased Visual Reasoning) | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.06000) | Unbiased visual reasoning with controlled visual inputs; transfers robustly across unseen VLM sensors |
| VLMs have Tunnel Vision | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.10000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.10000) | Evaluating nonlocal visual reasoning in leading VLMs; identifies tunnel vision limitations in spatial reasoning |
| Query-Oriented Pivot Tasks for GUI Agents | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.07000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.07000) | Smoothing grounding and reasoning for MLLM-powered GUI agents with query inference as bridge between grounding and reasoning |
[Back to top](#top)

---
### 3. GUI and Computer-Use Agents

#### 3.1 Benchmarks and Environments
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| Mind2Web | 2023-06 | [![arXiv](https://img.shields.io/badge/arXiv-2306.06070-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2306.06070) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OSU-NLP-Group/Mind2Web) | First large-scale dataset for generalist web agents with 2,350 tasks across 137 websites |
| WebArena | 2023-07 | [![arXiv](https://img.shields.io/badge/arXiv-2307.13854-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2307.13854) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/web-arena-x/webarena) | Foundational realistic web-agent benchmark with 812 tasks across 4 domains |
| Android-in-the-Wild (AITW) | 2023-10 | [![arXiv](https://img.shields.io/badge/arXiv-2310.04100-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2310.04100) | Large-scale dataset for Android device control with 715k episodes across 30k task instructions |
| VisualWebArena | 2024-01 | [![arXiv](https://img.shields.io/badge/arXiv-2401.13649-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.13649) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/web-arena-x/visualwebarena) | Screenshot-grounded browser-agent evaluation extending WebArena to visual perception |
| WebVoyager Benchmark | 2024-01 | [![arXiv](https://img.shields.io/badge/arXiv-2401.13919-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.13919) | Real-world web tasks from 15 websites with end-to-end visual evaluation |
| ScreenSpot | 2024-01 | [![arXiv](https://img.shields.io/badge/arXiv-2401.10935-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.10935) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/njucckevin/SeeClick) | First realistic GUI grounding benchmark spanning mobile, desktop, and web environments |
| WorkArena | 2024-03 | [![arXiv](https://img.shields.io/badge/arXiv-2403.07718-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2403.07718) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ServiceNow/WorkArena) | Enterprise workflow benchmark centered on knowledge-work tasks in ServiceNow |
| B-MoCA | 2024-04 | [![arXiv](https://img.shields.io/badge/arXiv-2404.02575-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2404.02575) | Benchmark for mobile device control agents across diverse configurations |
| OSWorld | 2024-04 | [![arXiv](https://img.shields.io/badge/arXiv-2404.07972-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2404.07972) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OSWorld) | Flagship open benchmark for real desktop computer use with 369 tasks |
| AndroidWorld | 2024-05 | [![arXiv](https://img.shields.io/badge/arXiv-2405.14573-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2405.14573) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/google-research/android_world) | Dynamic Android benchmark with 116 task workflows across 20 real-world apps |
| MobileAgentBench | 2024-06 | [![arXiv](https://img.shields.io/badge/arXiv-2406.08184-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2406.08184) | Efficient benchmark for mobile LLM agents with 100 tasks across 10 open-source apps |
| WebCanvas | 2024-07 | [![arXiv](https://img.shields.io/badge/arXiv-2407.11500-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2407.11500) | Online web agent benchmark with Mind2Web-Live dataset and dynamic evaluation |
| WindowsAgentArena | 2024-09 | [![arXiv](https://img.shields.io/badge/arXiv-2409.08264-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2409.08264) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/microsoft/WindowsAgentArena) | Scalable Windows evaluation environment with 150+ diverse tasks |
| SPA-Bench | 2024-10 | [![arXiv](https://img.shields.io/badge/arXiv-2410.15164-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.15164) | Strong multilingual smartphone benchmark with plug-and-play integration |
| AssistantBench | 2024-07 | [![arXiv](https://img.shields.io/badge/arXiv-2407.15711-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2407.15711) | Long-horizon realistic assistant tasks beyond short episodes |
| VideoWebArena | 2024-10 | [![arXiv](https://img.shields.io/badge/arXiv-2410.19100-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.19100) | Long-context video understanding inside web-agent workflows |
| OmniACT | 2024-02 | [![arXiv](https://img.shields.io/badge/arXiv-2402.17553-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.17553) | Evaluates executable desktop automation rather than only low-level action traces |
| ScreenSpot-Pro | 2025-04 | [![arXiv](https://img.shields.io/badge/arXiv-2504.07981-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.07981) | High-resolution professional-screen grounding benchmark |
| OSUniverse | 2025-05 | [![arXiv](https://img.shields.io/badge/arXiv-2505.01900-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.01900) | Complex multimodal desktop-oriented benchmark with automated validation |
| WebChoreArena | 2025-06 | [![arXiv](https://img.shields.io/badge/arXiv-2506.01900-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.01900) | Extends WebArena to labor-intensive and tedious web tasks with 532 curated tasks |
| VPI-Bench | 2025-06 | [![arXiv](https://img.shields.io/badge/arXiv-2506.02456-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.02456) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/boyugou/VPI-Bench) | Visual prompt-injection benchmark for GUI agents |
| GUI-Robust | 2025-06 | [![arXiv](https://img.shields.io/badge/arXiv-2506.01700-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.01700) | Dataset for testing GUI agent robustness against 7 types of real-world anomalies |
| OSWorld-Human | 2025-06 | [![arXiv](https://img.shields.io/badge/arXiv-2506.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.02000) | First study on temporal performance of computer-use agents on OSWorld |
| Agent-X | 2025-05 | [![arXiv](https://img.shields.io/badge/arXiv-2505.24876-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.24876) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/mbzuai-oryx/Agent-X) | Step-level reasoning assessment benchmark for GUI agents |
| WAREX | 2025-08 | [![arXiv](https://img.shields.io/badge/arXiv-2508.01900-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.01900) | Web Agent Reliability Evaluation framework validated on WebArena, REAL, and WebVoyager |
| OSWorld-MCP | 2025-10 | [![arXiv](https://img.shields.io/badge/arXiv-2510.02900-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.02900) | First benchmark for MCP tool invocation in computer-use agents built on OSWorld |
| SecureWebArena | 2025-10 | [![arXiv](https://img.shields.io/badge/arXiv-2510.01100-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.01100) | Holistic security evaluation benchmark for LVLM-based web agents |
| GUI-360° | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.01000) | Large-scale dataset for computer-using agents spanning grounding, parsing, and action prediction |
| AndroidLab | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.02000) | Systematic mobile agent benchmark with reproducible and measurable environment |
| GUIOdyssey | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.01000) | Comprehensive dataset for cross-app GUI navigation with 8,334 episodes across 212 apps |
| WebArena Verified | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.02000) | Reliable evaluation for web agents with reduced false negatives (NeurIPS 2025) |
| MemGUI-Bench | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.06075-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.06075) | Cross-session and cross-temporal memory evaluation for GUI agents |
| ProBench | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.03000) | Comprehensive mobile benchmark with accurate process information (AAAI 2026) |
| GUI-Perturbed | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.14262-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14262) | Robustness diagnostics for perturbation and relational instruction evaluation |
| DynamicGUIBench | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.25380-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.25380) | Dynamic, evolving GUI environments rather than frozen UI snapshots |
| GUI-CEval | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.04000) | First comprehensive benchmark for Chinese mobile GUI agents on real-device environments |
| GUI Survey (Benchmarks) | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.03000) | Comprehensive survey of benchmarks for LLM-based GUI agents |
| CUA-Suite | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.24440-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.24440) | Consolidated suite for modern computer-use-agent research |

#### 3.2 Visual Grounding and Perception for GUI
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| SeeClick | 2024-01 | [![arXiv](https://img.shields.io/badge/arXiv-2401.10935-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.10935) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/njucckevin/SeeClick) | Visual GUI agent relying only on screenshots with GUI grounding pre-training |
| ScreenAI | 2024-02 | [![arXiv](https://img.shields.io/badge/arXiv-2402.04615-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.04615) | Foundational for screen, document, infographic, and layout-heavy visual understanding |
| Ferret-UI | 2024-04 | [![arXiv](https://img.shields.io/badge/arXiv-2404.05719-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2404.05719) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/apple/ml-ferret) | Region-aware mobile grounding and explicit UI understanding from Apple |
| OmniParser | 2024-08 | [![arXiv](https://img.shields.io/badge/arXiv-2408.00203-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2408.00203) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/microsoft/OmniParser) | Comprehensive method for parsing UI screenshots into structured, interactable elements |
| UGround | 2024-10 | [![arXiv](https://img.shields.io/badge/arXiv-2410.05243-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.05243) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OSU-NLP-Group/UGround) | Strong argument for fully visual, human-like GUI grounding without accessibility trees |
| OS-ATLAS | 2024-10 | [![arXiv](https://img.shields.io/badge/arXiv-2410.23218-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.23218) | Large cross-platform action-grounding corpus and strong open foundation for GUI control |
| Aguvis | 2024-12 | [![arXiv](https://img.shields.io/badge/arXiv-2412.04454-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2412.04454) | Pure-vision GUI agent direction without dependence on textual trees |
| ShowUI | 2024-11 | [![arXiv](https://img.shields.io/badge/arXiv-2411.17465-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2411.17465) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/showlab/ShowUI) | Unified screenshot-conditioned action modeling with strong builder relevance |
| UI-E2I-Synth | 2025-04 | [![arXiv](https://img.shields.io/badge/arXiv-2504.11257-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.11257) | Synthetic instruction generation pipeline for scaling GUI grounding quality and diversity |
| GUI-Actor | 2025-06 | [![arXiv](https://img.shields.io/badge/arXiv-2506.03143-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.03143) | Agent-friendly grounding without brittle coordinate assumptions |
| Test-Time RL for GUI Grounding | 2025-08 | [![arXiv](https://img.shields.io/badge/arXiv-2508.05615-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.05615) | Test-time optimization approach for improving GUI grounding itself |
| GUI-Eyes | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.09770-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.09770) | Tool-augmented perception and adaptive visual grounding for GUI agents |
| UI-Zoomer | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.14113-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14113) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/UI-Zoomer) | Uncertainty-driven adaptive zoom-in mechanism for dense, high-resolution UIs |

#### 3.3 Web Agents
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| SeeAct | 2024-01 | [![arXiv](https://img.shields.io/badge/arXiv-2401.01614-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.01614) | Important early argument that capable web agents depend on grounding quality as much as model scale |
| WebVoyager | 2024-01 | [![arXiv](https://img.shields.io/badge/arXiv-2401.13919-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.13919) | Early strong end-to-end visual web agent with 59.1% task success rate |
| Agent-E | 2024-07 | [![arXiv](https://img.shields.io/badge/arXiv-2407.01700-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2407.01700) | Hierarchical web agent with DOM distillation and change observation; 73.2% on WebVoyager |
| AgentOccam | 2024-10 | [![arXiv](https://img.shields.io/badge/arXiv-2410.01700-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.01700) | Simple yet strong baseline for LLM-based web agents; 26.6 point improvement on WebArena |
| Multimodal Auto Validation for Web Agents | 2024-10 | [![arXiv](https://img.shields.io/badge/arXiv-2410.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.03000) | Self-refinement for web agents via multimodal validation; boosts Agent-E to 81.24% |
| AutoWebGLM | 2024-10 | [![arXiv](https://img.shields.io/badge/arXiv-2410.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.04000) | Open-source web agent with bootstrap training strategies and self-learning |
| Browser Use | 2024-12 | [![Project](https://img.shields.io/badge/Project-Browser_Use-0f766e?logo=vercel&logoColor=white)](https://browser-use.com) | State-of-the-art web agent achieving 89.1% on WebVoyager benchmark |
| LiteWebAgent | 2025-03 | [![arXiv](https://img.shields.io/badge/arXiv-2503.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.04000) | Open-source suite for VLM-based web agent applications with serverless backend |
| Surfer-H | 2025-05 | [![arXiv](https://img.shields.io/badge/arXiv-2505.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.03000) | Cost-efficient web agent pairing VLM with Holo1 open-weight models |
| Web-Shepherd | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.05000) | PRM-based web agent achieving 85.0% on WebRewardBench (NeurIPS 2025) |
| Go-Browse | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.06000) | Training web agents with structured exploration; 21.7% on WebArena with 7B model (NeurIPS 2025) |
| MolmoWeb | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.05000) | Open visual web agent from Ai2 with 30K human task trajectories and full training stack |
| DUDE | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.01000) | Deceptive UI Detector & Evaluator for teaching web agents to resist deceptive interfaces |
| Yutori Navigator | 2025-12 | [![Project](https://img.shields.io/badge/Project-Yutori-0f766e?logo=vercel&logoColor=white)](https://radical.vc) | SOTA web agent on Online-Mind2Web and Navi-Bench; autonomous cloud browser |

#### 3.4 Mobile GUI Agents
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| AppAgent | 2023-12 | [![arXiv](https://img.shields.io/badge/arXiv-2312.13771-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2312.13771) | Foundational smartphone-use agent with multimodal exploration and deployment phases |
| CogAgent | 2023-12 | [![arXiv](https://img.shields.io/badge/arXiv-2312.08914-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2312.08914) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/THUDM/CogAgent) | 18B-parameter VLM specializing in GUI understanding with high-resolution input |
| ClickAgent | 2024-10 | [![arXiv](https://img.shields.io/badge/arXiv-2410.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.02000) | Separates MLLM reasoning from UI location model for enhanced mobile grounding |
| DigiRL | 2024-06 | [![arXiv](https://img.shields.io/badge/arXiv-2406.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2406.03000) | Training in-the-wild device-control agents with autonomous RL; 49.5% improvement on AITW |
| AutoGLM | 2025-08 | [![arXiv](https://img.shields.io/badge/arXiv-2508.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.02000) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/THUDM/AutoGLM) | First Phone Use AI agent with open-source model; stable complex multi-step mobile operations |
| Advancing Mobile GUI Agents (V-Droid) | 2025-03 | [![arXiv](https://img.shields.io/badge/arXiv-2503.15937-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.15937) | Verifier-driven mobile automation with deployment-minded latency tradeoffs |
| MobileUse | 2025-07 | [![arXiv](https://img.shields.io/badge/arXiv-2507.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.03000) | Hierarchical reflection-driven GUI agent for robust and adaptive mobile task execution |
| MagicGUI | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.04000) | Foundational mobile GUI agent with scalable data pipeline and reinforcement fine-tuning |
| UI-Genie | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.05000) | Self-improving framework with reward-specific dataset for GUI agents (NeurIPS 2025) |
| AgentCPM-GUI | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.03000) | 8B-parameter on-device GUI agent with reinforcement fine-tuning (EMNLP 2025) |
| Agent-SAMA | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.04000) | State-Aware Mobile Assistant for autonomous app navigation |
| OdysseyAgent | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.07000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.07000) | Exploratory multimodal agent for long-step cross-app navigation with history resampler |
| GELab-Zero | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.05000) | 4B GUI Agent model with complete infrastructure for one-click deployment on Android |
| Hi-Agent | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.06000) | Trainable hierarchical vision-language agent for mobile device control |
| ClawMobile | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.07000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.07000) | Rethinking smartphone-native agentic systems with probabilistic planning |
| Nebula-GUI | 2026-05 | [![Project](https://img.shields.io/badge/Project-Nebula_GUI-0f766e?logo=vercel&logoColor=white)](https://www.voiceofemirates.com) | On-device control agent for AI smartphone; executes multi-step tasks locally |

#### 3.5 Desktop and Computer-Use Agents
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| OS-Copilot | 2024-02 | [![arXiv](https://img.shields.io/badge/arXiv-2402.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.03000) | Generalist computer agent framework with self-improvement via FRIDAY |
| Agent S | 2024-10 | [![arXiv](https://img.shields.io/badge/arXiv-2410.08164-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.08164) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/simular-ai/Agent-S) | Strong open framework for hierarchical planning and experience reuse |
| UFO2 | 2025-04 | [![arXiv](https://img.shields.io/badge/arXiv-2504.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.05000) | Multi-agent AgentOS for Windows desktops with centralized HostAgent and isolated virtual desktop |
| Ponder & Press | 2025-05 | [![arXiv](https://img.shields.io/badge/arXiv-2505.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.04000) | Divide-and-conquer framework for general computer control using only visual input |
| Agent S2 | 2025-04 | [![arXiv](https://img.shields.io/badge/arXiv-2504.00906-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.00906) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/simular-ai/Agent-S) | Strong compositional upgrade with specialists for grounding and planning |
| UItron | 2025-04 | [![arXiv](https://img.shields.io/badge/arXiv-2504.04246-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.04246) | More capable perception-planning integration in GUI control |
| Agent S3 | 2025-10 | [![arXiv](https://img.shields.io/badge/arXiv-2510.07000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.07000) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/simular-ai/Agent-S) | First to surpass human-level performance on OSWorld (72.60%) |
| OS-Symphony | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.07779-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.07779) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OS-Copilot/OS-Symphony) | Memory, reflection, and tutorial retrieval for computer use |
| ActionEngine | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.20502-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.20502) | Programmatic GUI agents with state-machine memory and executable plans |
| UI-Copilot | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.13822-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.13822) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/UI-Copilot) | Long-horizon automation with retrieval and calculator tools integrated into policy learning |
| VLAA-GUI | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.01000) | Modular GUI framework teaching agents when to Stop, Recover, and Search |

#### 3.6 Cross-Platform and Generalist GUI Agents
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| InfiGUIAgent | 2025-01 | [![arXiv](https://img.shields.io/badge/arXiv-2501.04575-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2501.04575) | Multimodal generalist GUI agent with native reasoning and reflection |
| UI-TARS | 2025-01 | [![arXiv](https://img.shields.io/badge/arXiv-2501.12326-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2501.12326) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/bytedance/UI-TARS) | Strongest open signal for native GUI agents heading across platforms |
| Magma | 2025-02 | [![arXiv](https://img.shields.io/badge/arXiv-2502.13130-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.13130) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/microsoft/Magma) | Important bridge between digital computer use and physical action settings |
| Mobile-Agent-v3 / GUI-Owl | 2025-08 | [![arXiv](https://img.shields.io/badge/arXiv-2508.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.03000) | Foundational GUI agent model with SOTA across desktop and mobile benchmarks |
| OpenCUA | 2025-08 | [![arXiv](https://img.shields.io/badge/arXiv-2508.09123-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.09123) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OpenCUA) | Strong open data, model, and benchmark foundation for computer-use agents |
| Holo2 | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.06000) | Cost-efficient lightweight models for cross-platform computer-use agents |
| Surfer 2 | 2025-10 | [![arXiv](https://img.shields.io/badge/arXiv-2510.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.06000) | Unified architecture for cross-platform computer use from pure visual observations |
| MAI-UI | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.08000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.08000) | Real-world centric foundation GUI agents with strong grounding performance |
| Mobile-Agent-v3.5 / GUI-Owl-1.5 | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.08000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.08000) | Multi-platform native GUI agent with instruct/thinking variants in multiple sizes |
| LAMO | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.02000) | Multi-role orchestration for scalable lightweight GUI agents |

#### 3.7 Training, Data, and Self-Improvement
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| Multimodal-Mind2Web | 2024-12 | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/osunlp/Multimodal-Mind2Web) | Multimodal version of Mind2Web dataset for visual web agent development |
| ScaleTrack | 2025-05 | [![arXiv](https://img.shields.io/badge/arXiv-2505.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.05000) | Training framework scaling grounding and backtracking planning for GUI agents |
| ZeroGUI | 2025-05 | [![arXiv](https://img.shields.io/badge/arXiv-2505.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.06000) | Online GUI agent learning at zero human cost; integrates with UI-TARS and Aguvis |
| Co-EPG | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.07000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.07000) | Co-evolution framework for planning and grounding in autonomous GUI agents |
| SE-GUI | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.09000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.09000) | Self-evolutionary reinforcement fine-tuning for visual grounding with only 3k samples |
| TongUI / GUI-Net-1M | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.10000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.10000) | Internet-scale trajectories from multimodal web tutorials; 1M trajectories across 280+ apps |
| ScaleCUA | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.15221-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.15221) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OpenGVLab/ScaleCUA) | Strong data-scaling result and open training/evaluation stack across platforms |
| AMEX | 2025-06 | [![arXiv](https://img.shields.io/badge/arXiv-2506.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.04000) | Android Multi-annotation Expo Dataset for generalist mobile GUI-control agents (ACL 2025) |
| ShowUI-Aloha | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.07181-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.07181) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/showlab/ShowUI) | Demonstration-to-agent pipeline from raw human screen recordings |
| EvoCUA | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.15876-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.15876) | Synthetic experience generation and step-level policy optimization for computer use |
| GroundCUA / GroundNext | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.07332-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.07332) | Human-demonstration-derived desktop grounding dataset and models |
| Video2GUI | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.14747-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.14747) | Converts web GUI videos into structured action trajectories for agent pretraining |

#### 3.8 Safety, Security, and Robustness
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| Towards Trustworthy GUI Agents Survey | 2025-03 | [![arXiv](https://img.shields.io/badge/arXiv-2503.23434-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.23434) | Robustness, reliability, and deployment-focused risk analysis for GUI agents |
| GUI Agents: A Survey | 2024-12 | [![arXiv](https://img.shields.io/badge/arXiv-2412.13501-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2412.13501) | Broad overview of task settings, architectures, benchmarks, and system bottlenecks |
| A Survey on (M)LLM-Based GUI Agents | 2025-04 | [![arXiv](https://img.shields.io/badge/arXiv-2504.13865-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.13865) | Good entry point for planning, grounding, memory, and evaluation in screenshot-grounded agents |
| UI-Evol | 2025-05 | [![arXiv](https://img.shields.io/badge/arXiv-2505.21964-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.21964) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/microsoft/FIVE-UI-Evol) | Tracks how external knowledge must be revised from actual execution, not only retrieved |

#### 3.9 Specific Agent Models and Systems
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| CogAgent-9B-20241220 | 2024-12 | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/THUDM/CogAgent) | Updated CogAgent with significantly improved GUI perception and action prediction |
| OpenAI Operator | 2025-01 | [![Docs](https://img.shields.io/badge/Docs-OpenAI-2563eb?logo=readthedocs&logoColor=white)](https://openai.com/index/computer-using-agent/) | Product-level computer-using agent with visual reasoning and tool use |
| Anthropic Claude Computer Use | 2024-10 | [![Docs](https://img.shields.io/badge/Docs-Anthropic-2563eb?logo=readthedocs&logoColor=white)](https://www.anthropic.com/news/developing-computer-use) | First major commercial computer-use capability with GUI-agent development |
| Google Project Mariner | 2024-12 | [![Docs](https://img.shields.io/badge/Docs-Google-2563eb?logo=readthedocs&logoColor=white)](https://deepmind.google/blog/) | Browser-based agent from Google DeepMind for web task automation |
| GUI-360° Dataset | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.01000) | Large-scale comprehensive dataset for computer-using agents |
| Cua | 2025-08 | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/trycua/cua) | Open-source computer-use infrastructure, sandboxes, and SDKs |
| OpenAdapt | ongoing | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OpenAdaptAI/OpenAdapt) | Desktop control, data capture, evaluation, and agent-building utilities |

#### 3.10 Web Agent Protocol and Infrastructure
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| WebMCP | 2026-02 | [![Project](https://img.shields.io/badge/Project-WebMCP-0f766e?logo=chrome&logoColor=white)](https://www.pconline.com.cn) | New protocol by Google and Microsoft enabling AI agents to interact directly with web kernels without simulating human operations |
| Cloudflare Agent Cloud | 2026-04 | [![Docs](https://img.shields.io/badge/Docs-Cloudflare-2563eb?logo=cloudflare&logoColor=white)](https://blog.cloudflare.com) | Infrastructure to power millions of autonomous, long-running web agents |
| EcoGEO | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.02000) | Trajectory-aware evidence ecosystems for web-enabled LLM search agents |
[Back to top](#top)

---
### 4. Embodied Vision-Language-Action Agents

#### 4.1 Foundational VLA Models & Generalist Policies
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| PaLM-E | 2023-03 | [![arXiv](https://img.shields.io/badge/arXiv-2303.03378-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2303.03378) | An embodied multimodal language model that injects continuous sensor inputs directly into a pretrained LLM’s embedding space |
| RT-2 | 2023-07 | [![arXiv](https://img.shields.io/badge/arXiv-2307.15818-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2307.15818) | Canonical VLA paper connecting web-scale vision-language knowledge with low-level robot control via action tokenization |
| Octo | 2023-10 | [![arXiv](https://img.shields.io/badge/arXiv-2310.04200-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2310.04200) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/octo-models/octo) | Open-source transformer-based generalist robot policy trained on 800k trajectories from the Open X-Embodiment dataset |
| OpenVLA | 2024-06 | [![arXiv](https://img.shields.io/badge/arXiv-2406.09246-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2406.09246) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/openvla/openvla) | Central open baseline for embodied visual-agent work; 7B-parameter VLA fine-tuned from Prismatic VLMs on Open X-Embodiment |
| RT-2-X | 2024-10 | [![arXiv](https://img.shields.io/badge/arXiv-2410.24164-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.24164) | Transformer-based VLA representing robot actions as tokenized text sequences for unified cross-embodiment control |
| π₀ (Pi-Zero) | 2024-10 | [![arXiv](https://img.shields.io/badge/arXiv-2410.24164-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.24164) | Flow-matching-based generalist robot policy trained on 10,000 hours of dexterous manipulation data from Physical Intelligence |
| Magma | 2025-02 | [![arXiv](https://img.shields.io/badge/arXiv-2502.13130-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.13130) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/microsoft/Magma) | Bridge paper spanning digital computer-use and embodied action; unified multimodal agent for GUI and robotic manipulation |
| Being-H0.5 | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.01900-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.01900) | Foundational VLA for cross-embodiment generalization via human-centric learning from large-scale human interaction traces |
| Helix | 2025-02 | [![arXiv](https://img.shields.io/badge/arXiv-2502.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.04000) | Figure AI's dual-system VLA (System 1 fast reactive + System 2 slow reasoning) for dexterous humanoid manipulation |
| GR-Dexter | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.00900-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.00900) | Holistic hardware-model-data framework for VLA-based generalist bimanual dexterous-hand manipulation |
| Pelican-Unified 1.0 | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.14000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.14000) | First embodied foundation model trained on unification principle; single VLM maps scenes, instructions, and action histories into shared semantic space |
| MiMo-Embodied | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.28000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.28000) | First cross-embodied foundation model achieving SOTA in both Autonomous Driving and 17 Embodied AI benchmarks |
| HY-Embodied-0.5 | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.08000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.08000) | Family of foundation models for real-world embodied agents; includes edge-deployable 1.5B and reasoning-focused 32B variants |
| RynnBrain | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.13000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.13000) | Open-source spatiotemporal foundation model for egocentric understanding, spatiotemporal localization, grounded reasoning, and physics-aware planning |
| RLDX-1 | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.05000) | General-purpose dexterous manipulation policy with Multi-Stream Action Transformer (MSAT) unifying heterogeneous modalities |

#### 4.2 VLA Architecture, Grounding, and Alignment
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| Interleave-VLA | 2025-05 | [![arXiv](https://img.shields.io/badge/arXiv-2505.02152-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.02152) | Extends VLA systems to interleaved image-text instruction following for richer task specification |
| ChatVLA-2 | 2025-05 | [![arXiv](https://img.shields.io/badge/arXiv-2505.21906-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.21906) | Preserves open-world reasoning capabilities in embodied VLA agents through unified chat-based interaction |
| VLA^2 | 2025-10 | [![arXiv](https://img.shields.io/badge/arXiv-2510.14902-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.14902) | Highlights the value of explicit external modules in unseen-concept manipulation for VLA generalization |
| Stable Language Guidance for VLA | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.00700-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.00700) | Residual Affordance Steering: dual-stream decoding isolating causal influence of language by subtracting visual affordance prior |
| Restoring Linguistic Grounding in VLA | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.06000) | Train-free attention recalibration to fix VLA failure modes where policies ignore language instructions |
| Not All Features Are Created Equal | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.19000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.19000) | Mechanistic study of VLA models via activation injection and linear probes across 6 models (80M–7B, 394k+ episodes) |
| ProGAL-VLA | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.10000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.10000) | Prospective Grounding and Alignment VLA; slow planner generates symbolic sub-goals aligned with grounded entities via GAC loss |
| Grounding Hierarchical VLA | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.07000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.07000) | Training framework explicitly grounding hierarchical VLA sub-task descriptions in visual observation and action space |
| VEGA | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.11000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.11000) | Visual Encoder Grounding Alignment; aligns VLA visual encoder with spatially-aware DINOv2-FiT3D features |
| GuidedVLA | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.12000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.12000) | Plug-and-play action attention specialization for specifying task-relevant factors in VLA |
| IntentVLA | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.14000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.14000) | Short-horizon intent modeling for aliased robot manipulation; disentangles visual aliasing via explicit intent prediction |
| VLA-Forget | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.05000) | Vision-Language-Action unlearning for removing unsafe, spurious, or privacy-sensitive behaviors in embodied foundation models |
| CF-VLA | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.15000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.15000) | Coarse-to-fine two-stage action generation: coarse initialization + single-step local refinement for efficient VLA inference |

#### 4.3 Efficient VLA, Sim-to-Real, and Deployment
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| Latent Bridge | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.04000) | Lightweight model predicting VLM output features for efficient dual-system VLA inference, reducing backbone execution frequency |
| See What Matters | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.12000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.12000) | Differentiable grid sample pruning for generalizable VLA; avoids the compression-performance trade-off in token pruning |
| StarVLA | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.06000) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/StarVLA) | Lego-like open-source codebase for VLA development; one of the most comprehensive VLA frameworks available |
| RIO | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.12000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.12000) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/RIO) | Flexible real-time Robot I/O framework for cross-embodiment robot learning across 3 morphologies and 4 hardware platforms |
| EmbodiChain | 2026-01 | [![Project](https://img.shields.io/badge/Project-EmbodiChain-0f766e?logo=vercel&logoColor=white)](https://github.com/EmbodiChain) | First toolchain that auto-trains VLA models with 100% synthetic data from generative simulation world models, achieving zero-shot sim-to-real transfer |
| SEVO | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.11000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.11000) | Semantic-Enhanced Virtual Observation for robust VLA manipulation via active illumination and data-centric collection |
| Enhancing Linguistic Generalization of VLA | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.17000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.17000) | Fine-tuning OpenVLA via synthetic instruction augmentation for improved zero-shot performance in novel environments |

#### 4.4 Embodied Planning, Reasoning, and Task Decomposition
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| ForeAct | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.12000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.12000) | Visual Foresight Planning: efficient planner guiding VLA step-by-step via imagined future observations; pretrained on 1M+ episodes |
| BagelVLA | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.05000) | Unified model integrating linguistic planning, visual forecasting, and action generation for long-horizon manipulation |
| Fast-ThinkAct | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.01000) | Verbalizable latent planning for efficient VLA reasoning; reduces inference latency while maintaining long-horizon planning |
| PALM | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.04000) | Progress-Aware Policy Learning via affordance reasoning; identifies task-relevant cues and tracks subtask progress to prevent errors |
| Goal2Skill | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.15000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.15000) | Dual-system framework for long-horizon manipulation with adaptive planning and reflection to handle partial observability |
| LoHo-Manip | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.23000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.23000) | Trace-Conditioned VLA Planning: extends short-horizon VLA to long-horizon tasks via dedicated task-management VLM |
| CodeGraphVLP | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.24000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.24000) | Code-as-Planner meets Semantic-Graph State for non-Markovian VLA; persistent graph state with executable code-based planner |
| SYMBOLIZER | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.20000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.20000) | Symbolic Model-free Task Planning with VLMs; integrates VLM-based grounding with simulator-driven TAMP |
| UniPlan | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.09000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.09000) | Vision-language task planning for mobile manipulation with unified PDDL formulation in large-scale indoor environments |
| RoboAgent | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.09000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.09000) | Chaining basic VLM capabilities for multi-turn embodied task planning with visual observation and atomic action execution |
| Thinking in Text and Images (IVLR) | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.01000) | Interleaved Vision-Language Reasoning traces for long-horizon manipulation; exposes both causal order and spatial constraints |
| PRISM | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.06000) | Perception Reasoning Interleaved for Sequential Decision Making; couples VLM perception and LLM decision via dynamic QA pipeline |
| HoloMind | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.14000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.14000) | Zero-shot execution of complex long-horizon household tasks via VLM-driven hierarchical planning, grounding, memory, and reflective critic |
| VeriGraph | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.16000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.16000) | Scene Graphs for execution-verifiable robot planning; uses VLM-generated scene graphs for symbolic state verification |
| When to Act, Ask, or Learn | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.12000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.12000) | Uncertainty-Aware Policy Steering: learned verifier analyzes low-level policy confidence to decide when to act, ask, or learn |

#### 4.5 VLA with Reinforcement Learning and Value Models
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| PRTS | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.30000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.30000) | Primitive Reasoning and Tasking System via contrastive representations; reframes VLA pretraining as goal-reaching with temporal progress |
| VLAJS | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.15000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.15000) | Jump-Start RL with VLA regularization; bridges sparse VLA guidance with on-policy RL for improved exploration |
| NS-VLA | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.10000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.10000) | Neuro-Symbolic VLA via online RL; unifies neural perception with symbolic reasoning for robust manipulation |
| ViVa | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.09000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.09000) | Video-generative value model repurposing pretrained video generator for value estimation in partially observable settings |
| RL Token | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.30000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.30000) | Bootstrapping online RL with VLA models for precision and speed beyond imitation learning |
| D-VLA | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.13000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.13000) | High-concurrency distributed asynchronous RL framework for VLA models addressing simulation-resource conflicts |
| MARVL | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.07000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.07000) | Multi-stage guidance for robotic manipulation via VLM reward design for RL |
| Large Reward Models | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.22000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.22000) | Generalizable online robot reward generation with VLMs for real-robot reinforcement learning |
| DyGRO-VLA | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.15000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.15000) | Dynamic Grouped Residual Optimization addressing multi-task performance degradation; 97.1% average success on LIBERO benchmark |
| CreFlow | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.14000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.14000) | Corrective Reflow for sparse-reward embodied video diffusion RL with compositional LTL constraint-based reward model |

#### 4.6 Safety, Interpretability, and Robustness
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| Concept-Based Dictionary Learning for VLA Safety | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.02000) | First inference-time concept-based safety method for embodied systems; advances both interpretability and safe deployment |
| Safe-Night VLA | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.05000) | Thermal-perceptive VLA for safety-critical manipulation in unstructured low-light environments |
| VLA Safety Survey | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.26000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.26000) | Systematic review of VLA threats, challenges, evaluations, and defense mechanisms |
| Embodied Interpretability | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.01000) | Links causal understanding to generalization in VLA; NMR metric predicts generalization, ISS yields faithful explanations |
| Affordance Field Intervention | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.16000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.16000) | Lightweight hybrid framework using Spatial Affordance Fields to guide VLA out of memory traps in manipulation |
| BusyBox | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.05000) | Physical benchmark for systematic semi-automatic evaluation of VLA affordance generalization with 6 interactive modules |

#### 4.7 Navigation, Exploration, and Embodied QA
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| AgentVLN | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.18000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.18000) | Efficient agentic VLN framework deployable on edge computing platforms for long-horizon navigation |
| NavGemini | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.06000) | Multi-modal LLM agent for VLN based entirely on Gemini-Pro-Vision |
| ProFocus | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.15000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.15000) | Proactive perception and focused reasoning for VLN; addresses passive processing and indiscriminate history treatment |
| DecoVLN | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.26000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.26000) | Decouples observation, reasoning, and correction for VLN; addresses long-term memory and compounding errors |
| LaViRA | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.04000) | Zero-shot VLN in continuous environments translating language, vision, and robot actions |
| CMMR-VLN | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.09000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.09000) | Continual multimodal memory retrieval for VLN; selective recall and use of relevant prior knowledge |
| VLN-NF | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.19000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.19000) | Feasibility-aware VLN with false-premise instructions; agents must detect absent targets through in-room exploration |
| LookasideVLN | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.19000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.19000) | Direction-aware aerial VLN for UAVs following natural language in complex urban environments |
| MoS-VLN | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.13000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.13000) | Mixture of Skill-Based VLN agents: decomposes navigation into reusable skill primitives for compositional generalization |
| What Limits VLN? | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.13000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.13000) | Systematic study identifying visual priors as stable grounding cues even when instructions are vague |
| Instruction-as-State | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.20000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.20000) | Environment-guided state-conditioned semantic understanding for embodied navigation |
| D3D-VLP | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.16000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.16000) | Dynamic 3D Vision-Language-Planning model unifying planning, grounding, navigation, and QA via 3D Chain-of-Thought |
| UrbanNav | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.17000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.17000) | Learning language-guided embodied urban navigation from web-scale human trajectories |
| Sparsely Grounded Visual Navigation | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.10000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.10000) | Evaluates sequential decision-making of MLLMs in knowledge-intensive real-world navigation with sparse landmarks |
| UniGround | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.09000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.09000) | Training-free universal 3D visual grounding via scene parsing for embodied AI |
| HIMM | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.02000) | Human-inspired long-term memory modeling for embodied exploration and QA; +7.3% LLM-Match on A-EQA |
| MetaSpace | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.24000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.24000) | Metamorphic testing for spatial cognition in embodied agents |

#### 4.8 Dexterous, Bimanual, and Specialized Manipulation
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| PEAfowl | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.25000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.25000) | Perception-enhanced multi-view VLA for bimanual manipulation with per-token depth distributions and differentiable 3D lifting |
| GF-VLA | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.29000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.29000) | Graph-Fused VLA for dual-arm policy reasoning and execution from RGB(-D) human demonstrations |
| CoFreeVLA | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.03000) | Collision-free dual-arm VLA with short-horizon self-collision risk estimator |
| TwinVLA | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.06000) | Data-efficient bimanual manipulation composing two copies of pretrained single-arm VLA into coordinated bimanual policy |
| EgoScale | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.19000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.19000) | Human-to-dexterous-manipulation transfer framework; shows effective transfer is a scaling phenomenon |
| SkillVLA | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.04000) | Skill reuse for dual-arm VLA; recombines previously learned single-arm skills across novel pairings |
| XL-VLA | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.10000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.10000) | Cross-hand latent representation for VLA with unified latent action space shared across diverse dexterous hands |
| LatentVLA | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.17000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.17000) | Taming latent space for generalizable long-horizon bimanual manipulation; SOTA on real-world bimanual tasks |
| DexHiL | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.10000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.10000) | First integrated arm-hand human-in-the-loop framework for dexterous VLA post-training |
| Green-VLA | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.07000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.07000) | Staged VLA framework for humanoid robot deployment with five-stage curriculum across diverse embodiments |
| TMR-VLA | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.28000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.28000) | First end-to-end VLA framework for magnetic soft robots achieving hybrid primitive control |
| AnySlot | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.12000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.12000) | Goal-conditioned VLA for zero-shot slot-level placement; turns language into explicit visual goal via scene marker generation |
| VILAS | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.03000) | VLA-integrated low-cost architecture with soft grasping for fragile object manipulation on accessible hardware |
| NovaFlow | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.30000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.30000) | Zero-shot manipulation via actionable flow from generated videos without any demonstrations |
| Anticipation-VLA | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.03000) | Solves long-horizon tasks via anticipation-based subgoal generation; UMM for high-level planning + goal-conditioned VLA |
| GTA-VLA | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.13000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.13000) | Interactive VLA enabling spatially steerable embodied reasoning through user-provided explicit visual cues |
| VLAbot | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.16000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.16000) | Human VLA interaction framework for robotic assembly; LLM divides long-horizon tasks, VLA generates actions |
| GazeVLA | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.24000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.24000) | Learns and transfers human intention from egocentric gaze data for robotic manipulation |
| EgoActor | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.36000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.36000) | Unified VLM predicting locomotion primitives, head movements, and manipulation commands for humanoid robots |
| MoT-HRA | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.27000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.27000) | Hierarchical VLA learning human-intention priors from 2.2M large-scale human demonstrations |
| CRISP | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.20000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.20000) | Robot's inner critic: self-refinement of social behaviors through VLM-based replanning |
| UniJEPA | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.13000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.13000) | Unified continuous and discrete representation learning for robot policies addressing data scarcity and embodiment heterogeneity |
| Learning Action Manifold | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.12000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.12000) | Multi-view latent priors for robotic manipulation; uses pretrained multi-view diffusion to synthesize novel views for spatial perception |
| ExpressMM | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.23000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.23000) | Expressive mobile manipulation behaviors in HRI; high-level VLM planner + low-level VLA policy for collaborative tasks |
[Back to top](#top)

---
### 5. Agentic Image Generation, Editing, and Search

#### 5.1 Agentic Image Generation
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| GenArtist | 2024-07 | [![arXiv](https://img.shields.io/badge/arXiv-2407.05600-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2407.05600) [![NeurIPS](https://img.shields.io/badge/NeurIPS-2024-0f766e?logo=neurips&logoColor=white)](https://proceedings.neurips.cc/paper_files/paper/2024/hash/e7c786024ca718f2487712bfe9f51030-Abstract-Conference.html) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/zhenyuw16/GenArtist) | MLLM as agent for unified image generation and editing via tool selection and planning |
| CIGEval | 2025-04 | [![arXiv](https://img.shields.io/badge/arXiv-2504.07046-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.07046) | Unified agentic framework for comprehensive evaluation of conditional image generation tasks |
| T2I-Copilot | 2025-07 | [![arXiv](https://img.shields.io/badge/arXiv-2507.02900-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.02900) | Training-free multi-agent system with Input Interpreter, Model Selector, and Refiner for prompt interpretation and iterative refinement |
| ImAgent | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.11483-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.11483) | Training-free unified multimodal agent framework for test-time scalable image generation with self-evaluation |
| LayerCraft | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.03000) | Modular framework using LLMs as agents to orchestrate structured, layered image generation and editing via CoT reasoning |
| Maestro | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.05000) | Self-improving text-to-image generation via agent-orchestrated iterative prompt evolution |
| AuDiffusion | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.05000) | Multi-agent controlled text-to-image generation with attention-enhanced Mamba blocks for controllability and semantic alignment |
| CRAFT | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.02100-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.02100) | Training-free reasoning layer for text-to-image generation with Continuous Reasoning and Agentic Feedback Tuning |
| DiffusionAgent | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.02000) | All-in-one system navigating expert models for agentic image generation across diverse prompts |
| GenAgent | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.18543-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.18543) | Agentic multimodal reasoning with generators as tools (SFT + RL on FLUX.1-dev); cross-tool generalization and test-time scaling |
| Mind-Brush | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.01756-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.01756) | Unified agentic framework transforming image generation into dynamic, knowledge-driven workflow with cognitive search and reasoning |
| M3 | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.06166-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.06166) | Multi-agent reasoning loop for compositional text-to-image generation |
| coDrawAgents | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.03000) | Interactive multi-agent dialogue framework with Interpreter, Planner, Checker, and Painter for compositional image generation |
| DiffGraph | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.04000) | Automated agent-driven graph-based model merging framework for in-the-wild text-to-image generation |
| VisionCreator | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.02681-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.02681) | Native visual-generation agent with explicit understanding-thinking-planning-creation (UTPC) loop |
| VisionCreator-R1 | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.03000) | Reflection-enhanced native visual generation agent with Reflection-Plan Co-Optimization (RPCO) training |
| Gen-Searcher | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.28767-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.28767) [![Project](https://img.shields.io/badge/Project-Gen_Searcher-0f766e?logo=vercel&logoColor=white)](https://gen-searcher.vercel.app/) | Search-augmented agentic generation with RL dual rewards; multi-hop reasoning and reference image collection |
| GEMS | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.28088-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.28088) [![Project](https://img.shields.io/badge/Project-GEMS-0f766e?logo=gmail&logoColor=white)](https://gems-gen.github.io/) | Agent-native multimodal generation with memory and skills |
| Unify-Agent | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.01000) | Unified multimodal agent for world-grounded image synthesis; reframes generation as prompt understanding, evidence searching, recaptioning, and synthesis |
| GoT-R1 | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.03000) | Reinforcement learning framework enhancing semantic-spatial reasoning in autoregressive visual generation |
| ManimTrainer / ManimAgent | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.04000) | Training pipeline (SFT + RL with GRPO) and Renderer-in-the-loop inference agent for animation generation |
| Self-Reasoning Agentic Framework for Grid-Collage | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.05000) | Self-reasoning agentic framework for narrative product grid-collage generation with visual consistency |
| ATLAS | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.06000) | Agentic or latent visual reasoning for image generation; maintains standard autoregressive loop with SFT/RL compatibility |

#### 5.2 Agentic Image Editing
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| DeepEyes | 2025-05 | [![arXiv](https://img.shields.io/badge/arXiv-2505.14362-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.14362) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/Visual-Agent/DeepEyes) | Visual reasoning agent with explicit zoom and crop tool use for enhanced visual understanding |
| PhotoArtAgent | 2025-05 | [![arXiv](https://img.shields.io/badge/arXiv-2505.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.04000) | Intelligent photo retouching agent combining VLMs with natural language reasoning to emulate professional artist workflow |
| JarvisArt | 2025-06 | [![arXiv](https://img.shields.io/badge/arXiv-2506.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.01000) | MLLM-driven agent coordinating 200+ retouching tools within Lightroom for intelligent photo retouching |
| RefineEdit-Agent | 2025-08 | [![arXiv](https://img.shields.io/badge/arXiv-2508.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.01000) | Training-free LLM-LVLM driven agent enabling complex, iterative, context-aware image editing within closed-loop system |
| DeepEyesV2 | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.03000) | Agentic multimodal model extending DeepEyes with code execution, web search, and image manipulation tools |
| PerTouch | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.05000) | VLM-driven agent for personalized and semantic image retouching handling both strong and weak user instructions |
| JarvisEvo | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.04000) | Self-evolving photo editing agent with synergistic editor-evaluator optimization; emulates expert designer with iMCoT and SEPO |
| Agent Banana | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.09084-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.09084) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/taco-group/agent-banana) | Hierarchical planner–executor for high-fidelity object-aware editing with 4K HDD-Bench |
| MIRA | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.02000) | Multimodal Iterative Reasoning Agent predicting atomic edit instructions step-by-step with visual feedback; SFT + GRPO training |
| PhotoAgent | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.02000) | Agentic photo editing with exploratory visual aesthetic planning as long-horizon decision-making problem |
| Agentic Planning for Image Styling via Offline RL | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.04000) | Tool-based agentic RL post-training framework with structured planning and chain-of-thought reasoning for image styling |
| SMART-Editor | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.05000) | Multi-agent framework for compositional editing of structured images (posters, websites) with reward-guided planning |
| CAMEO | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.03000) | Conditional and quality-aware multi-agent image editing orchestrator; reformulates editing as feedback-driven process |
| Adaptive Task Reformulation for Image Editing | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.05000) | MLLM agent dynamically transforms image-instruction pairs into operation sequences via analysis, routing, and reformulation |
| DataEvolver | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.03000) | Closed-loop visual data engine for controllable visual data construction via goal-driven loop agents |
| EditRefiner | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.04000) | Human-aligned agentic framework for image editing refinement with perception-reasoning-action-evaluation loop |

#### 5.3 Agentic Visual Reasoning, Search, and Document Understanding
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| Gen-n-Val | 2025-06 | [![arXiv](https://img.shields.io/badge/arXiv-2506.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.03000) | Agentic image data generation and validation framework using Layer Diffusion, LLMs, and VLLMs for high-quality mask and image synthesis |
| Visual-ARFT | 2025-06 | [![arXiv](https://img.shields.io/badge/arXiv-2506.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.04000) | Visual Agentic Reinforcement Fine-Tuning empowering open-source LVLMs with web browsing, code execution, and image manipulation |
| Orion | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.03000) | Unified visual agent integrating vision-based reasoning with tool-augmented execution across images, video, and documents |
| ChartAgent | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.03000) | Tool-augmented multimodal agent for visually grounded reasoning in complex chart QA; NeurIPS 2025 MAR Workshop Oral |
| MMM-RAG | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.04000) | Multi-agent multi-feature method integrating image visual-structural and semantic information for multimodal RAG |
| SenseNova-MARS | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.05000) | Multimodal Agentic Reasoning and Search framework empowering VLMs with interleaved visual reasoning and tool-use via RL |
| InSight-o3 | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.06000) | Multi-agent framework with vReasoner and vSearcher for generalized visual search of relational, fuzzy, or conceptual regions |
| MiRA | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.07000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.07000) | Zero-shot Mixture-of-Reasoning Agents framework with Visual Analyzing, Text Comprehending, and Judge agents for multimodal QA |
| Sketch-Search Agent | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.08000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.08000) | Multimodal language agent integrating freehand sketches as control signals for diffusion-based image retrieval |
| ViDoRAG | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.09000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.09000) | Visual Document Retrieval-Augmented Generation via dynamic iterative reasoning agents with GMM-based hybrid retrieval |
| CharTool | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.04000) | Tool-integrated visual reasoning for chart understanding with image-cropping and code-based computation tools |
| SlideAgent | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.05000) | Hierarchical agentic framework for multi-page visual document understanding with element agent integrating external tools |
| HierVA | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.05000) | Hierarchical visual agent for chart reasoning maintaining joint image-text working context with zoom-in tool |
[Back to top](#top)

---
### 6. Video, 3D, and World-Construction Agents

#### 6.1 Video Understanding Agents
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| VideoAgent (Self-Improving) | 2024-10 | [![arXiv](https://img.shields.io/badge/arXiv-2410.10076-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.10076) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/Video-as-Agent/VideoAgent) | Self-improving video plan generation via self-conditioning consistency and VLM feedback for robot manipulation |
| VCA | 2024-12 | [![arXiv](https://img.shields.io/badge/arXiv-2412.10428-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2412.10428) | Video Curious Agent: curiosity-driven self-exploration via tree-search structure for long video understanding |
| VideoMindPalace | 2025-01 | [![arXiv](https://img.shields.io/badge/arXiv-2501.04336-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2501.04336) | Environment-grounded semantic graph structuring critical video moments for effective long video analysis; CVPR 2025 |
| PreMind | 2025-02 | [![arXiv](https://img.shields.io/badge/arXiv-2502.21283-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.21283) | Multi-agent multimodal framework for advanced indexing of presentation-style lecture videos |
| MR. Video | 2025-04 | [![arXiv](https://img.shields.io/badge/arXiv-2504.15647-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.15647) | Agentic long video understanding via MapReduce principle: independent dense perception then joint aggregation |
| AVA | 2025-05 | [![arXiv](https://img.shields.io/badge/arXiv-2505.01044-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.01044) | VLM-powered agentic video analytics system with near real-time Event Knowledge Graph construction |
| ViQAgent | 2025-05 | [![arXiv](https://img.shields.io/badge/arXiv-2505.15658-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.15658) | Zero-shot video QA agent combining Chain-of-Thought with open-vocabulary grounding validation (YOLO-World) |
| MUPA | 2025-06 | [![arXiv](https://img.shields.io/badge/arXiv-2506.16493-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.16493) | Multi-path agentic reasoning for grounded video QA unifying grounding, answering, reflection and aggregation |
| Flow4Agent | 2025-07 | [![arXiv](https://img.shields.io/badge/arXiv-2507.10129-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.10129) | Pioneering motion priors from optical flow to facilitate LLM-based long video understanding; ICCV 2025 |
| AVATAR (RL) | 2025-08 | [![arXiv](https://img.shields.io/badge/arXiv-2508.04017-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.04017) | Audio-Video Agent for Alignment and Reasoning via off-policy RL with Temporal Advantage Shaping |
| CogniGPT | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.23413-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.23413) | Interactive perception-verification loop between Multi-Granular Perception Agent and Active Verification Agent |
| AVI | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.12455-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.12455) | Agentic Video Intelligence: flexible training-free framework with Retrieve-Perceive-Review three-phase reasoning |
| Deep Video Discovery (DVD) | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.03279-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.03279) | Agentic search with tool use over segmented video clips; SOTA on LVBench |
| LongVT | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.18620-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.18620) | End-to-end agentic framework enabling native tool calling for "Thinking with Long Videos"; CVPR 2026 |
| AVATAAR | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.13600-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.13600) | Agentic video answering via temporal adaptive alignment and reasoning with Pre-Retrieval Thinking Agent |
| SciEducator | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.17945-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.17945) | Iterative self-evolving multi-agent system for scientific video comprehension via Deming-Cycle |
| VideoARM | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.12360-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.12360) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/VideoARM) | Agentic reasoning over hierarchical memory for long-form video understanding; CVPR 2026 |
| VideoZoomer | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.22315-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.22315) | RL-learned temporal focusing for long video reasoning; MLLM dynamically controls visual focus in multi-turn manner |
| V-Agent | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.00700-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.00700) | Interactive video search system using vision-language models with retrieval and re-ranking |
| VideoThinker | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.02200-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.02200) | Agentic VideoLLM trained on synthetic tool interaction trajectories for long-video benchmarks |
| EGAgent (Agentic Very Long Video Understanding) | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.18157-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.18157) | Entity scene graph-centered agentic framework for days/weeks-long egocentric video understanding (Meta) |
| EventMemAgent | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.14862-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.14862) | Hierarchical event-centric memory for online video understanding with adaptive tool use and Agentic RL |
| VideoMind | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.13463-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.13463) | Chain-of-LoRA agent for temporal-grounded video reasoning with Planner-Grounder-Verifier roles |
| Think, Then Verify (VideoHV-Agent) | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.04977-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.04977) | Hypothesis-verification multi-agent framework reformulating video QA as structured hypothesis testing; CVPR 2026 |
| Symphony | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.18000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.18000) | Cognitively-inspired multi-agent system for long-video understanding |
| HAVEN | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.24000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.24000) | Hierarchical long video understanding with audiovisual entity cohesion and agentic search |
| EVA | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.22918-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.22918) | Efficient RL framework for end-to-end video agent with planning-before-perception; CVPR 2026 |
| SAGE | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.29000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.29000) | Training smart any-horizon agents for long video reasoning with reinforcement learning |
| Graph-to-Frame RAG | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.06000) | Visual-space knowledge fusion for training-free and auditable video reasoning |
| MACF | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.01000) | Scaling video understanding via compact latent multi-agent collaboration |
| VideoSEAL | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.12000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.12000) | Mitigating evidence misalignment in agentic long video understanding by decoupling answer authority |
| ReTool-Video | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.13000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.13000) | Recursive tool-using video agents with meta-augmented tool grounding |

#### 6.2 Video Generation & Editing Agents
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| DreamCinema | 2024-08 | [![arXiv](https://img.shields.io/badge/arXiv-2408.12602-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2408.12602) | Cinematic transfer framework with free camera and 3D character for user-friendly film creation |
| Vlogger | 2024-01 | [![arXiv](https://img.shields.io/badge/arXiv-2401.01914-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.01914) | LLM-as-director decomposing vlog generation into four key stages; CVPR 2024 |
| VISTA (Test-Time) | 2025-01 | [![arXiv](https://img.shields.io/badge/arXiv-2510.11448-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.11448) | Test-time self-improving video generation agent; iterative prompt refinement with pairwise tournament selection (Google) |
| FilmAgent | 2025-01 | [![arXiv](https://img.shields.io/badge/arXiv-2501.12909-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2501.12909) | LLM-based multi-agent collaborative framework for end-to-end film automation in virtual 3D spaces |
| ReelWave | 2025-03 | [![arXiv](https://img.shields.io/badge/arXiv-2503.08207-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.08207) | Multi-agentic movie sound generation framework supervised by autonomous Sound Director agent |
| MovieAgent | 2025-03 | [![arXiv](https://img.shields.io/badge/arXiv-2503.07314-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.07314) | Automated movie generation via multi-agent CoT planning with hierarchical scene structuring |
| SciTalk | 2025-04 | [![arXiv](https://img.shields.io/badge/arXiv-2504.19721-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.19721) | Creator-inspired multi-LLM agentic framework for scientific short-form video generation with iterative feedback |
| PresentAgent | 2025-07 | [![arXiv](https://img.shields.io/badge/arXiv-2507.04867-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.04867) | Multimodal agent transforming long-form documents into narrated presentation videos |
| Omni-Video | 2025-07 | [![arXiv](https://img.shields.io/badge/arXiv-2507.05840-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.05840) | Efficient unified framework for video understanding, generation, and instruction-based editing |
| AniME | 2025-08 | [![arXiv](https://img.shields.io/badge/arXiv-2508.18781-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.18781) | Director-oriented multi-agent system for automated long-form anime production; SIGGRAPH Asia 2025 |
| PersonaVlog | 2025-08 | [![arXiv](https://img.shields.io/badge/arXiv-2508.13602-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.13602) | Personalized multimodal vlog generation with multi-agent collaboration and iterative self-correction |
| CAViAR | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.08887-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.08887) | Critic-augmented video agentic reasoning pairing a program-generating agent with a natural-language critic (Google DeepMind) |
| Preacher | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.07085-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.07085) | Paper-to-video agentic system distilling research papers into structured video abstracts; ICCV 2025 |
| VGTeam | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.00522-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.00522) | Communicative agents for slideshow storytelling video generation based on LLMs |
| VideoAgent (Scientific) | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.14000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.14000) | Personalized synthesis of scientific videos |
| AniMaker | 2025-10 | [![arXiv](https://img.shields.io/badge/arXiv-2510.01098-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.01098) | Multi-agent animated storytelling with MCTS-driven clip generation; Director + Photography + Reviewer agents |
| MAViS | 2025-10 | [![arXiv](https://img.shields.io/badge/arXiv-2510.06871-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.06871) | Multi-agent collaborative framework for long-sequence video storytelling from script to final video |
| UniVA | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.08521-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.08521) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/univa-agent/univa) | Open-source omni-capable multi-agent framework unifying video understanding, segmentation, editing, and generation |
| MoReGen | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.10000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.10000) | Multi-agent motion-reasoning engine for code-based text-to-video synthesis with physics simulators |
| Vgent | 2025-10 | [![arXiv](https://img.shields.io/badge/arXiv-2510.10974-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.10974) | Graph-based retrieval-reasoning-augmented generation for long video understanding; NeurIPS 2025 |
| Hollywood Town / OmniAgent | 2025-10 | [![arXiv](https://img.shields.io/badge/arXiv-2510.19808-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.19808) | Hierarchical graph-based multi-agent framework for long video generation inspired by film production |
| The Script is All You Need | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.17737-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.17737) | Agentic framework for long-horizon dialogue-to-cinematic video generation via ScripterAgent |
| LAVES | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.07269-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.07269) | Hierarchical LLM-based multi-agent system for educational video generation with quality gates and iterative critique |
| CutClaw | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.20517-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.20517) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/GVCLab/CutClaw) | Autonomous multi-agent framework for hours-long video editing via music synchronization |
| DIRECT | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.06000) | Video mashup creation via hierarchical multi-agent planning and intent-guided editing |
| Agentic Video Generation (Event Graphs) | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.10383-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.10383) | Text to executable event graphs via tool-constrained LLM planning; Director + Scene Builder two-agent architecture |
| Camera Artist | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.13886-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.13886) | Multi-agent framework modeling real-world filmmaking workflow to generate narrative videos with explicit cinematic language |
| CineAgents | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.14845-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14845) | Multi-agent system for instruction-driven cinematic video compilation; script reverse-engineering + iterative narrative planning |
| Co-Director | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.20235-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.20235) | Hierarchical multi-agent framework formalizing video storytelling as global optimization problem |
| CineAGI | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.23579-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.23579) | Character-consistent movie creation through LLM-orchestrated multi-modal generation and cross-scene integration; ICME 2026 |
| A2RD | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.07000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.07000) | Agentic autoregressive diffusion for long video consistency |
| Action Agent | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.01595-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.01595) | Two-stage agentic navigation video generation with flow-constrained diffusion for multi-embodiment robot control |
| VISTA (Egocentric) | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.11000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.11000) | Generative egocentric video framework for daily assistance |
| PresentAgent-2 | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.08400-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.08400) | Generalist multimodal presentation agent generating research-grounded presentation videos from user queries |

#### 6.3 3D Scene & World Construction Agents
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| Scenethesis | 2025-05 | [![arXiv](https://img.shields.io/badge/arXiv-2505.02836-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.02836) | Training-free agentic framework combining LLM scene planning with vision-guided layout refinement for diverse, physically plausible 3D scenes |
| ImmerseGen | 2025-06 | [![arXiv](https://img.shields.io/badge/arXiv-2506.14315-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.14315) [![Project](https://img.shields.io/badge/Project-ImmerseGen-0f766e?logo=vercel&logoColor=white)](https://immersegen.github.io) | Agent-guided immersive VR world generation with alpha-textured proxies; accepted by IEEE VR 2026 |
| Agentic 3D Scene Generation with Spatially Contextualized VLMs | 2025-07 | [![arXiv](https://img.shields.io/badge/arXiv-2507.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.04000) | VLM iteratively reads from and updates spatial context for 3D scene generation pipeline |
| FantasyHSI | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.01000) | Video-generation-centric 4D human synthesis in any scene through graph-based multi-agent framework |
| SceneWeaver | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.20414-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.20414) [![Project](https://img.shields.io/badge/Project-SceneWeaver-0f766e?logo=vercel&logoColor=white)](https://scene-weaver.github.io/) | Reflective agentic framework unifying diverse 3D scene synthesis paradigms through tool-based iterative refinement; NeurIPS 2025 |
| Agent2World | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.26000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.26000) | Tool-augmented multi-agent framework for symbolic world model generation via adaptive multi-agent feedback |
| World Craft | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.26000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.26000) | Agentic framework to create visualizable worlds via text |
| MA3DSG | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.04000) | Multi-agent 3D scene graph generation for large-scale indoor environments |
| WorldCraft | 2025-02 | [![arXiv](https://img.shields.io/badge/arXiv-2502.15601-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.15601) | LLM agents leverage procedural generation to create photo-realistic 3D worlds with natural language control |
| Code2Worlds | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.11757-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.11757) | Coding LLMs formulate 4D world generation as language-to-simulation code generation with dual-stream architecture |
| SAGE (3D) | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.10116-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.10116) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/NVlabs/sage) | Scalable agentic 3D scene generation for embodied AI; MCP-style agent calling layout and object generators |
| ShareVerse | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.01668-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.01668) | Multi-agent consistent video generation for shared world modeling with multi-view consistency |
| RieMind | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.15386-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.15386) | Geometry-grounded spatial agent for 3D indoor scene understanding; decouples perception and reasoning via explicit 3D scene graph |
| SceneAssistant | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.12238-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.12238) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ROUJINN/SceneAssistant) | Closed-loop text-to-3D scene generation with VLM visual feedback for iterative refinement and open-vocabulary spatial reasoning |
| Interact3D | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.16085-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.16085) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/SII-Hui/Interact3D) | Compositional 3D generation of physically plausible interacting objects with closed-loop VLM-based refinement |
| 3D-Generalist | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.02000) | Self-improving vision-language-action models for crafting 3D worlds |
| Think, Act, Build (TAB) | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.02000) | Agentic framework with VLMs for zero-shot 3D visual grounding; dynamic 2D-to-3D reconstruction paradigm |
| SceneOrchestra | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.21000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.21000) | Efficient agentic 3D scene synthesis via full tool-call trajectory generation with fine-tuned LLM orchestrator and discriminator |
| SpatialGrammar | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.30000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.30000) | Domain-specific language for LLM-based 3D indoor scene generation with conversational agentic workflow |
| WorldScape | 2026-04 | [![Project](https://img.shields.io/badge/Project-WorldScape-0f766e?logo=vercel&logoColor=white)](https://worldscape.io) | Real-time interactive world model with universal control, 3D spatial consistency, and long-horizon memory; ICML 2026 submission |
| Agent-World | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.18292-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.18292) | Self-evolving training arena for general agent intelligence; autonomously synthesizes environments and co-evolves agent policies |
| SimWorld Studio | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.10000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.10000) | Automatic environment generation with evolving coding agent for embodied agent learning on Unreal Engine 5 |
| SR-Platform | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.14000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.14000) | Agentic pipeline for natural language-driven robot simulation environment synthesis (MuJoCo) |
| Articraft | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.14000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.14000) | Agentic system for scalable articulated 3D asset generation via program writing |

#### 6.4 4D & Video World Models
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| DeepVerse | 2025-06 | [![arXiv](https://img.shields.io/badge/arXiv-2506.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.01000) | 4D autoregressive video generation as a world model with geometric predictions conditioned on actions |
| ViMax | 2025-08 | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/HKUDS/ViMax) | Agentic video generation framework orchestrating scriptwriting, storyboarding, and video production |
| Mora | 2025-03 | [![arXiv](https://img.shields.io/badge/arXiv-2403.13248-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2403.13248) | Multi-agent text-to-video framework achieving Sora-level performance on VBench |
| WorldReel | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.08000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.08000) | 4D video generation with consistent geometry and motion modeling for world modeling |
| TesserAct | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.01000) | Learning 4D embodied world models predicting dynamic 3D scene evolution in response to agent actions |
| SPIRAL | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.11000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.11000) | Closed-loop framework for self-improving action world models via reflective planning agents |
| Taming Video Models for 3D/4D | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.21000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.21000) | Zero-shot camera control for 3D and 4D generation from video diffusion models |
| MultiWorld | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.18564-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.18564) [![Project](https://img.shields.io/badge/Project-MultiWorld-0f766e?logo=vercel&logoColor=white)](https://multi-world.github.io/) | Unified multi-agent multi-view video world model for scalable game and robot manipulation environments |
| Embody4D | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.03000) | Generalist 4D world model for embodied AI; video-to-video synthesis of arbitrary novel views from monocular video |

#### 6.5 World Model & Simulation Agents
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| NovaPlan | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.23000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.23000) | Zero-shot long-horizon manipulation via closed-loop video language planning |
| WebWorld | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.16000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.16000) | Large-scale world model for web agent training; cross-domain generalization to code, GUI, and game environments |
| Specification-Driven World Models | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.04000) | Generation and evaluation of discrete-event world models via DEVS formalism |
| CoLA-World | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2510.21074-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.21074) | Co-evolving latent action world models: joint training of latent action model with pretrained video generation world model |
| Agentic World Modeling (Survey) | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.24000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.24000) | Foundations, capabilities, laws, and beyond; synthesizes over 400 works on world modeling |
| Being-H0.7 | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.19866-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.19866) | Latent world-action model from egocentric videos inserting future-aware reasoning into VLA without pixel generation |
| Anticipation-VLA | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.03000) | Solving long-horizon embodied tasks via anticipation-based subgoal generation |
| MCP-Cosmos | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.09000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.09000) | World model-augmented agents for complex task execution in MCP environments |
| Coding Agent Is Good As World Simulator | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.10389-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.10389) | Agentic framework constructing physics-based world models through executable simulation code; Planning + Code + Visual Review + Physics agents |
| Executable World Models for ARC-AGI-3 | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.06000) | Coding-agent system maintaining executable Python world model with verification and refactoring |
| LongAct | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.14000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.14000) | Benchmark and agent for long-horizon household task execution |
[Back to top](#top)

---
### 7. Agentic Visual Foundation Models
These are multimodal foundation models explicitly positioned as **agents** or with strong computer-use / tool-calling capabilities, not just generic VLMs.

#### 7.1 Generalist & Multimodal Agentic Models
| Model / Series | Year | Links | Why It Matters |
| --- | --- | --- | --- |
| Gemini Robotics / On-Device | 2025-03 | [![Docs](https://img.shields.io/badge/Docs-Gemini_Robotics-2563eb?logo=readthedocs&logoColor=white)](https://deepmind.google/blog/gemini-robotics-brings-ai-into-the-physical-world/) | Frontier industry view on embodied visual agents and on-device VLA deployment |
| Anthropic Claude 3.5 / 3.5 Haiku with computer use | 2025-10 | [![Docs](https://img.shields.io/badge/Docs-Anthropic_CU-2563eb?logo=readthedocs&logoColor=white)](https://www.anthropic.com/news/developing-computer-use) | Public engineering writeup on GUI-agent development and deployment with Claude |
| Kimi K2.5 | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.02276-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.02276) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/MoonshotAI/Kimi-K2.5) | Open-source native multimodal agentic model with joint visual-text RL; strong parallel agent orchestration and computer-use results |
| Qwen 3.6 | 2026-03 | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/QwenLM/Qwen3.6) [![Model](https://img.shields.io/badge/Model-35B--A3B-0f766e?logo=huggingface&logoColor=white)](https://huggingface.co/Qwen/Qwen3.6-35B-A3B) | Sparse MoE multimodal model with strong agentic coding and computer-use behavior |
| Kimi K2.6 | 2026-04 | [![Model](https://img.shields.io/badge/Model-1T_MoE-0f766e?logo=huggingface&logoColor=white)](https://huggingface.co/moonshotai/Kimi-K2.6) | Native multimodal agentic model (1T MoE, 32B active), scaling to 300 sub-agents and 4,000 coordinated steps |
| Qwen 3.5 | 2026-02 | [![Docs](https://img.shields.io/badge/Docs-Qwen_3.5-2563eb?logo=readthedocs&logoColor=white)](https://www.alibabacloud.com/en/campaign/qwen35-webinar) | Native multimodal reasoning and autonomous agent workflows; early-fusion architecture processing text, images, diagrams, and GUIs in a single pass |
| Gemma 4 | 2026-04 | [![Docs](https://img.shields.io/badge/Docs-Gemma_4-2563eb?logo=readthedocs&logoColor=white)](https://ai.google.dev/gemma) | Open-weight family (E2B, E4B, 26B MoE, 31B dense) with native video/image processing, audio input, and function-calling for autonomous agents |
| GLM-5V-Turbo | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2604.26752-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.26752) | Native foundation model for multimodal agents integrating perception, reasoning, planning, and tool use; CogViT vision encoder with multimodal multi-token prediction |
| Nemotron 3 Nano Omni | 2026-04 | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://huggingface.co/nvidia/Nemotron-3-Nano-Omni) | Open omni-modal reasoning model (30B-A3B MoE) unifying vision, audio, and language for agentic workflows; 9x throughput improvement |
| SenseNova-U1 | 2026-04 | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OpenSenseNova/SenseNova-U1) [![Docs](https://img.shields.io/badge/Docs-SenseNova-2563eb?logo=readthedocs&logoColor=white)](https://www.sensenova.cn/models) | Native unified multimodal model (understanding + generation) with strong info-graphic / PPT generation; positioned as a multimodal agent model for real workflows |
| MiMo-V2.5 | 2026-04 | [![Model](https://img.shields.io/badge/Model-1T_MoE-0f766e?logo=huggingface&logoColor=white)](https://huggingface.co/Xiaomi/MiMo-V2.5) | Xiaomi's MIT-licensed trillion-parameter MoE models with 1M-token context windows; Pro variant for long-horizon autonomous agents |

#### 7.2 Computer-Use & GUI Agent Models
| Model / Series | Year | Links | Why It Matters |
| --- | --- | --- | --- |
| OpenAI Computer-Using Agent (CUA) family | 2025-01 | [![Docs](https://img.shields.io/badge/Docs-OpenAI_CUA-2563eb?logo=readthedocs&logoColor=white)](https://platform.openai.com/docs/guides/tools-computer-use) | Product-level reference for how frontier models are wired into computer-use agent loops |
| UltraCUA | 2025-10 | [![arXiv](https://img.shields.io/badge/arXiv-2510.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.03000) | Foundation model for computer-use agents with hybrid action unifying primitive GUI operations and high-level tool execution |
| UI-TARS | 2025-01 | [![arXiv](https://img.shields.io/badge/arXiv-2501.12326-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2501.12326) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/bytedance/UI-TARS) | One of the strongest open signals for native GUI agent models; pioneer in end-to-end GUI grounding and action |
| UItron | 2025-04 | [![arXiv](https://img.shields.io/badge/arXiv-2504.04246-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.04246) | Open-source foundational GUI agent model with advanced perception, grounding, and planning capabilities |
| GUI-Owl (Mobile-Agent-v3) | 2025-08 | [![arXiv](https://img.shields.io/badge/arXiv-2508.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.03000) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/X-PLUG/MobileAgent) | Foundational GUI agent model achieving SOTA across desktop and mobile benchmarks |
| MAI-UI | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.08000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.08000) | Real-world centric foundation GUI agents spanning 2B to 32B; strong grounding and tool-use performance |
| OmegaUse | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.20380-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.20380) | General-purpose GUI agent for autonomous task execution on mobile and desktop; 96.3% on ScreenSpot-V2 |
| Mobile-Agent-v3.5 (GUI-Owl-1.5) | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.16855-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.16855) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/X-PLUG/MobileAgent) | Native GUI agent with instruct/thinking variants (2B/4B/8B/32B/235B) supporting desktop, mobile, and browser |
| ClawGUI | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.11784-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.11784) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ClawGUI) | Open-source GUI agent RL infrastructure with process reward model; trained 2B model deployed on Android, HarmonyOS, and iOS |
| FDM-1 | 2026-02 | [![Model](https://img.shields.io/badge/Model-Standard_Intelligence-0f766e?logo=vercel&logoColor=white)](https://standardintelligence.ai) | First fully general computer behavior model trained on 11M hours of screen recordings; 30 FPS video stream processing |
| OpenCUA | 2025-08 | [![arXiv](https://img.shields.io/badge/arXiv-2508.09123-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.09123) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OpenCUA) | Open data, model, and benchmark foundation for computer-use agents |

#### 7.3 Embodied Vision-Language-Action (VLA) Models
| Model / Series | Year | Links | Why It Matters |
| --- | --- | --- | --- |
| NVIDIA Isaac GR00T N1 | 2025-03 | [![Docs](https://img.shields.io/badge/Docs-GR00T_N1-2563eb?logo=readthedocs&logoColor=white)](https://developer.nvidia.com/isaac/gr00t) | World's first open foundation model for generalized humanoid robot reasoning and skills |
| EmbodiedBrain | 2025-10 | [![arXiv](https://img.shields.io/badge/arXiv-2510.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.04000) | Vision-language foundation model (7B/32B) establishing SOTA for embodied foundation models across task planning benchmarks |
| Vlaser | 2025-10 | [![arXiv](https://img.shields.io/badge/arXiv-2510.11027-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.11027) | VLA model integrating high-level embodied reasoning with low-level control; SOTA on WidowX and Google Robot benchmarks |
| MiMo-Embodied | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.04000) | First cross-embodied foundation model achieving SOTA in both Autonomous Driving (12 benchmarks) and Embodied AI (17 benchmarks) |
| Magma | 2025-02 | [![arXiv](https://img.shields.io/badge/arXiv-2502.13130-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.13130) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/microsoft/Magma) | Important bridge between digital computer use and physical action settings |
| OpenVLA | 2024-06 | [![arXiv](https://img.shields.io/badge/arXiv-2406.09246-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2406.09246) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/openvla/openvla) | Central open baseline for embodied visual-agent work |
| π₀ (Pi-Zero) | 2024-10 | [![arXiv](https://img.shields.io/badge/arXiv-2410.24164-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.24164) | Flow-matching-based generalist robot policy trained on 10,000 hours of dexterous manipulation data |
| ABot-M0 | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2602.11236-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.11236) | VLA foundation model with Action Manifold Learning; 6M+ trajectories across diverse robot morphologies |
| HY-Embodied-0.5 | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.07430-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.07430) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/Tencent-Hunyuan/HY-Embodied) | Embodied foundation model family (2B edge / 32B reasoning) with MoT architecture and iterative self-evolving post-training |
| AGIBOT GO-2 | 2026-04 | [![Docs](https://img.shields.io/badge/Docs-AGIBOT-2563eb?logo=readthedocs&logoColor=white)](https://www.agibot.com) | Next-gen embodied AI foundation model bridging logical reasoning to precise execution in unified architecture; CVPR 2026 |
| Pelican-Unified 1.0 | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.15153-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.15153) | First embodied foundation model trained on unification principle; single VLM for understanding, reasoning, imagination, and action |
| RLDX-1 | 2026-05 | [![Docs](https://img.shields.io/badge/Docs-RLWRLD-2563eb?logo=readthedocs&logoColor=white)](https://www.rlwrld.ai) | Dexterity-First robotics foundation model with Multi-Stream Action Transformer (MSAT); high-DOF 5-finger hand manipulation |
| GENE-26.5 | 2026-05 | [![Docs](https://img.shields.io/badge/Docs-Genesis_AI-2563eb?logo=readthedocs&logoColor=white)](https://www.genesis-ai.com) | AI foundation model for human-level physical manipulation; enables complex long-horizon dexterous tasks |
| SPEAR-1 | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.27000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.27000) | Robotic foundation model integrating grounded 3D perception with language-instructed embodied control |
| XR-1 | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.14000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.14000) | Versatile VLA model learning unified vision-motion representations from large-scale robotic datasets |
| XEmbodied | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.14000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14000) | Cloud-side foundation model endowing VLMs with intrinsic 3D geometric awareness and physical cue interaction |
| RynnBrain | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.13000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.13000) | Open-source spatiotemporal foundation model for egocentric understanding, spatiotemporal localization, grounded reasoning, and physics-aware planning |

#### 7.4 World & Coding Agent Models
| Model / Series | Year | Links | Why It Matters |
| --- | --- | --- | --- |
| Foundation World Models for Agents | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2510.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.05000) | Outlines a vision for foundation world models unifying RL, program synthesis, and abstraction mechanisms |
| Agentic World Modeling Survey | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.24000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.24000) | Synthesizes over 400 works on world models for agents, covering model-based RL, video generation, and planning |
| MCP-Cosmos | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.09000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.09000) | World model-augmented agents for complex task execution in MCP environments; BYOWM strategy |
| Orchard | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.14000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.14000) | Open-source framework for scalable agentic modeling with structured training curriculum |
| Safactory | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.15000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.15000) | Scalable agent factory for trustworthy autonomous intelligence; long-horizon decision making and tool use |

#### 7.5 Industry Foundation Models
| Model / Series | Year | Links | Why It Matters |
| --- | --- | --- | --- |
| OpenAI Operator (CUA) | 2025-01 | [![Docs](https://img.shields.io/badge/Docs-OpenAI_Operator-2563eb?logo=readthedocs&logoColor=white)](https://openai.com/index/computer-using-agent/) | First major commercial computer-using agent with visual reasoning and browser/desktop control |
| Google DeepMind Gemini 2.5 Computer Use | 2025-10 | [![Docs](https://img.shields.io/badge/Docs-Gemini_CU-2563eb?logo=readthedocs&logoColor=white)](https://deepmind.google/blog/) | Gemini-based computer-use model optimized for web browsers and mobile UIs |
| Google Project Mariner | 2024-12 | [![Docs](https://img.shields.io/badge/Docs-Mariner-2563eb?logo=readthedocs&logoColor=white)](https://deepmind.google/blog/) | Browser-based agent from Google DeepMind for web task automation |
| Boston Dynamics + Google DeepMind Atlas | 2026-01 | [![Docs](https://img.shields.io/badge/Docs-Atlas-2563eb?logo=readthedocs&logoColor=white)](https://bostondynamics.com) | Gemini Robotics AI foundation models integrated with new Atlas humanoid robots |
| Adobe Firefly Next-Gen (NVIDIA) | 2026-03 | [![Docs](https://img.shields.io/badge/Docs-Firefly-2563eb?logo=readthedocs&logoColor=white)](https://www.adobe.com/sensei/generative-ai/firefly.html) | Next-generation Firefly foundation models built on NVIDIA AI infrastructure for agentic creativity and marketing workflows |
| Linker Vision WFMs | 2026-03 | [![Docs](https://img.shields.io/badge/Docs-Linker_Vision-2563eb?logo=readthedocs&logoColor=white)](https://www.linkervision.com) | World Foundation Models for video reasoning and physical AI; continuous AI lifecycle from simulation to deployment |
| OpenSearch-VL | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.06000) | Fully open-source recipe for frontier multimodal search agents; 10-point average improvement across 7 benchmarks |
| cotomi Act | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.08000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.08000) | Browser-based computer-using agent combining reliable multi-step task execution with persistent organizational knowledge |

#### 7.6 Agentic Data Engine & Infrastructure
| Model / Series | Year | Links | Why It Matters |
| --- | --- | --- | --- |
| V-CAGE | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.09036-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.09036) | Vision-closed-loop agentic generation engine for robotic manipulation; autonomous synthetic data synthesis with visual self-verification |
| ReVision | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.11212-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.11212) | Trains multimodal models on computer-use trajectories with 46% token reduction while improving success rate |
| InfantAgent-Next | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.09000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.09000) | Multimodal generalist agent for automated computer interaction covering text, images, audio, and video |
| Ace-Skill | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.10000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.10000) | Bootstraps multimodal agents with prioritized and clustered evolution; 35B MoE model matching proprietary performance |
[Back to top](#top)

### 8. Safety, Reliability, and Evaluation

#### 8.1 Safety Benchmarks & Auditing
| Work | Date | Links | Notes |
| --- | --- | --- | --- |
| AGENTSAFE: Benchmarking the Safety of Embodied Agents on Hazardous Instructions | 2025-06-17 | [![arXiv](https://img.shields.io/badge/arXiv-2506.14697-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.14697) | First comprehensive safety benchmark for embodied VLM agents; 45 scenarios, 1,350 hazardous tasks, and 8,100 instructions evaluated across perception, planning, and execution. |
| IS-Bench: Evaluating Interactive Safety of VLM-Driven Embodied Agents in Daily Household Tasks | 2025-06-23 | [![arXiv](https://img.shields.io/badge/arXiv-2506.16402-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.16402) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/AI45Lab/IS-Bench) | First interactive safety benchmark for household tasks, with 161 scenarios and 388 unique risks. Evaluates ability to perceive emergent risks and execute mitigation steps. |
| RoboView-Bias: Benchmarking Visual Bias in Embodied Agents for Robotic Manipulation | 2025-09-26 | [![arXiv](https://img.shields.io/badge/arXiv-2509.22356-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.22356) | Systematic benchmark quantifying visual bias in robotic manipulation with 2,127 instances; camera viewpoint identified as the most critical factor. |
| OpenAgentSafety: A Comprehensive Framework for Evaluating Real-World AI Agent Safety | 2025-07-08 | [![arXiv](https://img.shields.io/badge/arXiv-2507.06134-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.06134) | Modular framework for evaluating agents across 8 risk categories, with over 350 multi-turn tasks interacting with real tools like browsers and code executors. Accepted at ICLR 2026. |
| VPI-Bench | 2025-06-02 | [![arXiv](https://img.shields.io/badge/arXiv-2506.02456-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.02456) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/boyugou/VPI-Bench) | Visual prompt-injection benchmark for GUI agents. |
| OS-Sentinel: Towards Safety-Enhanced Mobile GUI Agents via Hybrid Validation | 2025-10-28 | [![arXiv](https://img.shields.io/badge/arXiv-2510.24411-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.24411) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OS-Copilot/OS-Sentinel) | Introduces MobileRisk-Live sandbox and a hybrid safety detection framework combining formal verification with VLM-based contextual judging for mobile agents. |
| CUAAudit: Meta-Evaluation of VLMs as Auditors of Autonomous Computer-Use Agents | 2026-03-11 | [![arXiv](https://img.shields.io/badge/arXiv-2603.10577-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.10577) | Large-scale meta-evaluation of five VLMs as autonomous auditors for CUA task completion, revealing critical limitations in complex environments. |
| OS-BLIND: The Blind Spot of Agent Safety | 2026-04-17 | [![arXiv](https://img.shields.io/badge/arXiv-2604.10577-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.10577) | Evaluates CUAs under benign instructions that unintentionally cause harm (300 tasks); reveals >90% ASR across frontier models and failure of existing safety measures. |
| HazardArena: Evaluating Semantic Safety in VLAs | 2026-04-14 | [![arXiv](https://img.shields.io/badge/arXiv-2604.12447-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.12447) | Benchmark exposing vulnerability in VLAs where correct action execution may induce unsafe outcomes under semantic risk. |
| Owner-Harm: A Missing Threat Model for AI Agent Safety | 2026-04-20 | [![arXiv](https://img.shields.io/badge/arXiv-2604.18658-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.18658) | Formalizes the threat model of agents harming their own deployers, with benchmarks showing a critical defense gap in existing safety systems. |
| BackBench: Human-Guided Harm Recovery for Computer Use Agents | 2026-04-20 | [![arXiv](https://img.shields.io/badge/arXiv-2604.17800-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.17800) | A benchmark of 50 computer-use tasks testing an agent's ability to recover from harmful states. Introduces a reward model scaffold that improves recovery trajectory quality. |
| RUC & DUDE: Don't Click That: Teaching Web Agents to Resist Deceptive Interfaces | 2026-05-10 | [![arXiv](https://img.shields.io/badge/arXiv-2605.09497-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.09497) | Introduces RUC benchmark (1,407 scenarios) and DUDE defense framework, reducing deception susceptibility by 53.8%. Accepted at ACL 2026. |
| GUIGuard-Bench: Toward a General Evaluation for Privacy-Preserving GUI Agents | 2026-05-13 | [![arXiv](https://img.shields.io/badge/arXiv-2601.18842-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.18842) [![Project](https://img.shields.io/badge/Project-GUIGuard-0f766e?logo=github&logoColor=white)](https://futuresis.github.io/GUIGuard-page/) | First benchmark for privacy-preserving GUI agents with 241 trajectories and 4,080 screenshots annotated with region-level privacy labels across Android and PC. |

#### 8.2 Robustness & Perturbation Diagnostics
| Work | Date | Links | Notes |
| --- | --- | --- | --- |
| NEBULA: Do We Evaluate Vision-Language-Action Agents Correctly? | 2025-10-21 | [![arXiv](https://img.shields.io/badge/arXiv-2510.23000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.23000) | Demonstrates that top VLAs struggle with spatial reasoning and dynamic adaptation, obscured by conventional end-task success metrics. |
| AgentVista: Evaluating Multimodal Agents in Ultra-Challenging Realistic Visual Scenarios | 2026-02-26 | [![arXiv](https://img.shields.io/badge/arXiv-2602.23166-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.23166) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/hkust-nlp/AgentVista) | Benchmark for generalist multimodal agents spanning 25 sub-domains and 7 categories; best model (Gemini-3-Pro) achieves only 27.3% accuracy. |
| GUI-Perturbed: Domain Randomization Reveals Systematic Brittleness in GUI Grounding | 2026-04-15 | [![arXiv](https://img.shields.io/badge/arXiv-2604.14262-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14262) | Controlled perturbation framework revealing a 27-56 point accuracy drop on spatial reasoning tasks, and significant degradation under browser zoom. |
| Evaluating Self-Correcting Vision Agents | 2026-01-14 | [![arXiv](https://img.shields.io/badge/arXiv-2601.11637-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.11637) | Diagnostic micro-benchmark decoupling Task Success Rate (62%) from Correction Success Rate (25-33%), revealing that initial competence does not predict repair ability. |
| MM-AQA: Knowing When Not to Answer | 2026-04-16 | [![arXiv](https://img.shields.io/badge/arXiv-2604.16500-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.16500) | A benchmark evaluating effective abstention in multimodal reasoning systems. |
| Mobile GUI Agents under Real-world Threats: Are We There Yet? | 2026-04-14 | [![arXiv](https://img.shields.io/badge/arXiv-2604.12000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.12000) | Reveals significant degradation of mobile agents due to third-party content, with a 42.0% average misleading rate in dynamic environments. |

#### 8.3 VLA Safety Mechanisms & Defenses
| Work | Date | Links | Notes |
| --- | --- | --- | --- |
| SafeVLA: Towards Safety Alignment of VLA Model via Constrained Learning | 2025-03-05 | [![arXiv](https://img.shields.io/badge/arXiv-2503.03480-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.03480) [![Project](https://img.shields.io/badge/Project-SafeVLA-0f766e?logo=github&logoColor=white)](https://pku-safevla.github.io) | Integrates safety constraints into VLAs via CMDP paradigm; reduces safety violation cost by 83.58%. NeurIPS 2025 Spotlight. |
| Vision-Language-Action Safety: Threats, Challenges, Evaluations, and Mechanisms | 2026-04-26 | [![arXiv](https://img.shields.io/badge/arXiv-2604.23775-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.23775) | Unified survey organizing VLA safety along attack and defense timelines, covering data poisoning, adversarial patches, and cross-modal perturbations. |
| RedVLA: Physical Red Teaming for Vision-Language-Action Models | 2026-04-24 | [![arXiv](https://img.shields.io/badge/arXiv-2604.22591-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.22591) [![Project](https://img.shields.io/badge/Project-RedVLA-0f766e?logo=github&logoColor=white)](https://redvla.github.io) | First physical red teaming framework for VLA models; achieves a 95.5% attack success rate within 10 optimization iterations. |
| How VLAs (Really) Work In Open-World Environments | 2026-04-23 | [![arXiv](https://img.shields.io/badge/arXiv-2604.20000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.20000) | Argues for safety-aware evaluation metrics beyond progress-agnostic success measures. |
| ProjGuard: Safety Monitoring for CUA via Low-Dimensional Projections | 2026-05-13 | [![arXiv](https://img.shields.io/badge/arXiv-2605.13631-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.13631) | Behavioral trajectory monitoring with lightweight scalar risk signal; reduces unsafe rate from 16% to 3% while improving task completion. |
| Uncertainty-Calibrated Safety Gating for VLA Manipulation | 2026-05-15 | [![arXiv](https://img.shields.io/badge/arXiv-2605.15000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.15000) | A model-agnostic safety-gating wrapper that estimates online failure risk and routes control among policy execution, pause-and-reobserve, and fallback planning. |
| ICAT: Incident-Case-Grounded Adaptive Testing for Physical-Risk Prediction | 2026-03-31 | [![arXiv](https://img.shields.io/badge/arXiv-2604.16405-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.16405) | Grounds testing in real incident reports and safety manuals to construct risk memories for evaluating embodied world models. |

#### 8.4 Evaluation Frameworks & Methodologies
| Work | Date | Links | Notes |
| --- | --- | --- | --- |
| CIGEval: A Unified Agentic Framework for Evaluating Conditional Image Generation | 2025 (ACL) | [![ACL](https://img.shields.io/badge/ACL-2025-0f766e?logo=aclanthology&logoColor=white)](https://aclanthology.org/2025.acl-long.620/) | LMM-based agentic evaluation framework achieving 0.4625 correlation with human assessments. |
| VALOR: Value-Aligned Prompt Moderation via Zero-Shot Agentic Rewriting for Safe Image Generation | 2025-11-12 | [![arXiv](https://img.shields.io/badge/arXiv-2511.11693-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.11693) | A zero-shot agentic framework achieving up to 100% reduction in unsafe image generation outputs. |
| OS-SPEAR: A Toolkit for the Safety, Performance, Efficiency, and Robustness Analysis of OS Agents | 2026-04-27 | [![arXiv](https://img.shields.io/badge/arXiv-2604.24348-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.24348) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/Wuzheng02/OS-SPEAR) | Comprehensive toolkit evaluating 22 OS agents across Safety, Performance, Efficiency, and Robustness dimensions. |
| VTC-Bench: Evaluating Agentic Multimodal Models via Compositional Visual Tool Chaining | 2026-03-19 | [![arXiv](https://img.shields.io/badge/arXiv-2603.14000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.14000) | Evaluates tool-use proficiency in MLLMs through compositional visual tool chaining tasks. |
| SafePred: A Predictive Guardrail for Computer-Using Agents via World Models | 2026-05-01 | [![arXiv](https://img.shields.io/badge/arXiv-2605.01000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.01000) | Predictive guardrail mechanism that anticipates and prevents unsafe actions by computer-using agents via world models. |

#### 8.5 Adversarial Robustness & Red Teaming
| Work | Date | Links | Notes |
| --- | --- | --- | --- |
| CSAgent: Secure and Efficient Access Control for Computer-Use Agents via Context Space | 2025-12-31 | [![arXiv](https://img.shields.io/badge/arXiv-2512.30000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.30000) | Defends against >99.56% of attacks while introducing only 1.99% performance overhead. |
| Measuring What Matters: Benchmarking Generative, Multimodal, and Agentic AI in Healthcare | 2026-05-08 | [![arXiv](https://img.shields.io/badge/arXiv-2605.11000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.11000) | Focuses on systematic methods to measure reliability, safety, and clinical relevance of multimodal agents in healthcare. |
[Back to top](#top)

### 9. Data Engines, Demonstration Pipelines, and Open Foundations

#### 9.1 Computer-Use & GUI Data Engines
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| VisualWebBench | 2024-01 | [![arXiv](https://img.shields.io/badge/arXiv-2401.13649-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.13649) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/web-arena-x/visualwebarena) | Visually grounded web benchmark with human annotations and task definitions |
| UI-Vision | 2025-03 | [![arXiv](https://img.shields.io/badge/arXiv-2503.15661-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.15661) | Desktop-centric benchmark with dense annotations from human demonstrations |
| LearnAct / LearnGUI | 2025-04 | [![arXiv](https://img.shields.io/badge/arXiv-2504.12730-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.12730) | Few-shot mobile GUI agent with unified demonstration benchmark; 2,252 offline + 101 online tasks with high-quality human demonstrations |
| OS-Genesis | 2025-04 | [![arXiv](https://img.shields.io/badge/arXiv-2504.30000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.30000) | Automating GUI agent trajectory construction via reverse task synthesis |
| OS-Genesis (ICLR 2026) | 2025-06 | [![arXiv](https://img.shields.io/badge/arXiv-2506.29000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.29000) | Reverse task synthesis for GUI trajectory construction; accepted ICLR 2026 |
| UI-E2I-Synth | 2025-04 | [![arXiv](https://img.shields.io/badge/arXiv-2504.11257-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.11257) | Synthetic instruction generation pipeline for GUI grounding data |
| Scaling Computer-Use Grounding (Jedi) | 2025-05 | [![arXiv](https://img.shields.io/badge/arXiv-2505.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.03000) | Largest computer-use grounding dataset Jedi (4M examples) via UI decomposition and synthesis |
| EDGE | 2025-06 | [![arXiv](https://img.shields.io/badge/arXiv-2506.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.05000) | Enhanced grounded GUI understanding with enriched multi-granularity synthetic data |
| Ferret-UI Lite | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.20000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.20000) | Small on-device GUI agent with multi-agent synthetic rollout generation |
| GUI-ReWalk | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.15000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.15000) | Massive data generation for GUI agent via stochastic exploration and intent-aware reasoning |
| AUTO-Explorer | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.05000) | Automated data collection for GUI agent; autonomous parsing and exploration of GUI environments |
| GroundCUA / GroundNext | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.07332-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.07332) | Large-scale desktop grounding dataset from expert human demonstrations; 87 apps, 56K screenshots, 3.56M annotations |
| GUI-360° | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.04000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.04000) | 1.2M action steps across thousands of trajectories in Windows applications; comprehensive benchmark |
| Mobile-Agent-v3 (Self-Evolving GUI Trajectory Production) | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.18000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.18000) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/X-PLUG/MobileAgent) | Self-evolving GUI trajectory production pipeline contrasting with manual annotation methods |
| UI-Genie | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.19000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.19000) | Self-improving framework with reward model and self-improving pipeline for mobile GUI agents; NeurIPS 2025 |
| TongUI (GUI-Net-1M) | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.18000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.18000) | Internet-scale trajectories from multimodal web tutorials; 1M trajectories across 280+ apps |
| ShowUI-Aloha | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-2601.07181-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.07181) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/showlab/ShowUI) | Demonstration-to-agent pipeline from raw human screen recordings |
| CUA-Suite | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-2603.24440-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.24440) | Combines VideoCUA, GroundCUA, and UI-Vision into one research-facing ecosystem |
| ClawMark | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.03000) | Living-world benchmark and tool schema for multi-turn, multi-day, multimodal coworker agents |
| NPiDA-Bench | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.08000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.08000) | Natural-Plan-guided dual-audit benchmark for detecting stealth malicious behaviors in GUI agents |
| Video2GUI | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.14747-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.14747) | Converts web GUI videos into structured action trajectories for generalized agent pretraining; ICML 2026 |
| AgAgent | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.13000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.13000) | Agent-centric data engine for autonomous driving; millions of high-quality data generated with agent active exploration |
| ShowUI-Agent | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.14000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.14000) | Self-improving GUI agent with bootstrapped data scaling and iterative RL |
| CICHEL | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.17000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.17000) | Continuous interaction controlled human evaluator loop for agentic visual data engine |
| KeyVISCON | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.11000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.11000) | Leveraging visual key demonstration for LLM-based GUI agents |
| Kiro Agent | 2026-04 | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/kiro-agent) | Open-source computer-use agent infrastructure with demonstration recording and replay capabilities |
| OpenAdapt Desktop | ongoing | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OpenAdaptAI/openadapt-desktop) | Captures computer interaction traces for training, replay, and agent loops |

#### 9.2 Embodied & Robotics Data Engines
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| MimicDreamer | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.26000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.26000) | Aligning human and robot demonstrations for scalable VLA training via video diffusion |
| Open X-Embodiment | 2023-10 | [![arXiv](https://img.shields.io/badge/arXiv-2310.08864-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2310.08864) | Largest open-source real robot dataset with 1M+ trajectories from 60+ robot-embodiment-task combinations |
| TeachAnything | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.12000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.12000) | Multimodal crowdsourcing platform with three-stage demonstration paradigm for embodied AI agents |
| RIGVid | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.13000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.13000) | Robots imitating generated videos without physical demonstrations; pouring, wiping, mixing tasks |
| V-CAGE | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.09036-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.09036) | Vision-closed-loop agentic generation engine for robotic manipulation; autonomous synthetic data with visual self-verification |
| SPIL | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.20000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.20000) | Scalable policy improvement from language; hybrid human-LLM demonstration generation + VLA fine-tuning |
| GR-MG (Generalist Robot Manipulation Data Generator) | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-2602.25300-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.25300) | Multi-modal robot demonstration benchmark in simulation and physical environments; 1500+ manipulation tasks |
| DeeR-VLA | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.28000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.28000) | Data-efficient embodied VLA; demonstration pipeline enabling few-shot policy adaptation |
| SceneAction | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.23367-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.23367) | High-quality annotated 3D scene-action pairs dataset created via an agentic generation pipeline; ICCV 2025 |
| GenAug | 2023-06 | [![arXiv](https://img.shields.io/badge/arXiv-2306.06000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2306.06000) | Data augmentation pipeline for robot manipulation using text-to-image generative models for visual generalization |
| EgoMimic | 2024-11 | [![arXiv](https://img.shields.io/badge/arXiv-2411.10000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2411.10000) | Scaling robot policy learning via egocentric human demonstration replay with embodiment alignment |
| Video2Policy | 2025-03 | [![arXiv](https://img.shields.io/badge/arXiv-2503.05000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.05000) | Learning robot manipulation policies from internet demonstration videos with visual grounding |

#### 9.3 Visual Generation Data Engines
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| DataEvolver | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.01900-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.01900) | Closed-loop multi-artifact visual data engine for end-to-end automated controllable data construction |
| Gen-n-Val | 2025-06 | [![arXiv](https://img.shields.io/badge/arXiv-2506.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.03000) | Agentic image data generation and validation framework using Layer Diffusion and VLLMs |
| GenAug (Visual Reasoning) | 2025-07 | [![arXiv](https://img.shields.io/badge/arXiv-2507.02000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.02000) | Automated data augmentation pipeline for visual reasoning tasks |
| CICHEL | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.17000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.17000) | Continuous interaction controlled human evaluator loop for agentic visual data engine |
| Z2CAD | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.27000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.27000) | Agentic synthesis of interpretable CAD programs at million-scale without real data |
| LayoutCopilot | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.08578-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.08578) | Agentic spatial reasoning model for visual layout generation; training data engine with multi-stage RL |
| Ground2Visual | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.13000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.13000) | GUI description-to-screenshot generation engine; automated pipeline transforming grounding data into visual assets |
| RAZOR | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.26000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.26000) | Sharp-edged visual assistant model; optimized visual data pipeline for reasoning-focused generation tasks |

#### 9.4 Open-Source Foundation Stacks
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| OpenCUA | 2025-08 | [![arXiv](https://img.shields.io/badge/arXiv-2508.09123-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.09123) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OpenCUA) | Open foundation stack spanning data, benchmarks, and agent development |
| ScaleCUA | 2025-09 | [![arXiv](https://img.shields.io/badge/arXiv-2509.15221-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.15221) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OpenGVLab/ScaleCUA) | Open-source data-scaling pipeline, models, training code, and evaluation environments |
| Magma | 2025-02 | [![arXiv](https://img.shields.io/badge/arXiv-2502.13130-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.13130) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/microsoft/Magma) | Foundation model for multimodal AI agents; bridge between digital computer use and physical action |
| StarVLA | 2026-04 | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/StarVLA) | Lego-like open-source codebase for VLA development; comprehensive VLA framework |
| RIO | 2026-05 | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/RIO) | Flexible real-time Robot I/O framework for cross-embodiment robot learning |
| EmbodiChain | 2026-01 | [![Project](https://img.shields.io/badge/Project-EmbodiChain-0f766e?logo=vercel&logoColor=white)](https://github.com/EmbodiChain) | First toolchain auto-training VLA models with 100% synthetic data; zero-shot sim-to-real transfer |
| MolmoWeb | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-2604.09000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.09000) | Open visual web agent with MolmoWebMix (100K synthetic + 30K human trajectories); fully open multimodal web agents |
| OpenAdapt-ML | ongoing | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OpenAdaptAI/openadapt-ml) | Model-training layer for turning captured interaction data into agent pipelines |
| Cua | ongoing | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/trycua/cua) | Open-source infrastructure, sandboxes, and SDKs for computer-use-agent development |
| Agentic AI Foundation (AAIF) | 2025-12 | [![Docs](https://img.shields.io/badge/Docs-Linux_Foundation-2563eb?logo=linux&logoColor=white)](https://www.linuxfoundation.org/press/agentic-ai-foundation) | Linux Foundation initiative with Anthropic MCP, Block goose, and OpenAI AGENTS.md support |

#### 9.5 Agentic Self-Evolving Frameworks
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| AgentEvolver | 2025-11 | [![arXiv](https://img.shields.io/badge/arXiv-2511.17000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.17000) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/alibaba/AgentEvolver) | Autonomous self-evolving agents framework from Tongyi Lab; self-questioning, self-navigating, self-attributing |
| AgentEvolver-2 | 2025-12 | [![arXiv](https://img.shields.io/badge/arXiv-2512.20000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.20000) | Improved self-evolving agent framework with memory-aware online learning and episodic memory |
| EvoAgentX | 2025-05 | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/EvoAgentX) | Open-source framework for building self-evolving AI agent ecosystems with automated workflow generation |
| Orchard | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.16000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.16000) | Open-source framework for scalable agentic modeling with structured training curriculum |
| Safactory | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.15000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.15000) | Scalable agent factory for trustworthy autonomous intelligence |

#### 9.6 Demonstration Capture & Observation Tools
| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| OpenAdapt Desktop | ongoing | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OpenAdaptAI/openadapt-desktop) | Records and structures real computer-use traces for training, replay, and analysis |
| ScreenPipe | ongoing | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/screenpipe/screenpipe) | Continuous screen capture and local memory substrate for long-running visual agents |
| Sekko | 2026-04 | [![NPM](https://img.shields.io/badge/NPM-sekko-0f766e?logo=npm&logoColor=white)](https://www.npmjs.com/package/sekko) | Capture browser and terminal sessions; extract structured artifacts AI agents can read for UI understanding |
| Agent Loom | 2026-04 | [![NPM](https://img.shields.io/badge/NPM-agent_loom-0f766e?logo=npm&logoColor=white)](https://www.npmjs.com/package/agent-loom) | AI-generated narrated screen recordings; point at URL or topic, get narrated video |
| RunSight | 2026-04 | [![NPM](https://img.shields.io/badge/NPM-runsight-0f766e?logo=npm&logoColor=white)](https://www.npmjs.com/package/runsight) | Autonomous browser agent with automated guide generation from project analysis |
| Clawmarks (npm) | 2025-12 | [![NPM](https://img.shields.io/badge/NPM-clawmarks-0f766e?logo=npm&logoColor=white)](https://www.npmjs.com/package/clawmarks) | MCP server for LLM agents to create annotated bookmarks in codebase; trail-based knowledge graph |
| ClawMark (Benchmark) | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.03000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.03000) | Multi-turn, multi-day, multimodal coworker agent benchmark with harness-agnostic tool schema |
| Unworldly Recorder | 2026-02 | [![PyPI](https://img.shields.io/badge/PyPI-unworldly--recorder-0f766e?logo=pypi&logoColor=white)](https://pypi.org/project/unworldly-recorder) | Session recording with MCP server, web dashboard, and CI/CD integration |
| Video Recorder MCP | 2026-03 | [![NPM](https://img.shields.io/badge/NPM-video__recorder__mcp-0f766e?logo=npm&logoColor=white)](https://www.npmjs.com/package/video-recorder-mcp) | MCP server for video analysis and recording paired with LiveMCP for demos |
| Teal (MCP) | 2025-12 | [![GitHub](https://img.shields.io/badge/GitHub-teal-181717?logo=github&logoColor=white)](https://github.com/teal-mcp/teal) | MCP server and framework for multi-modal agents to interact with the web through a browser; screen capture and DOM access |
| EyeBrowse | 2025-11 | [![GitHub](https://img.shields.io/badge/GitHub-eyebrowse-181717?logo=github&logoColor=white)](https://github.com/eyebrowse-mcp/eyebrowse) | MCP tool for visual web browsing; structured screen content extraction |
| WebMCP | 2026-02 | [![Project](https://img.shields.io/badge/Project-WebMCP-0f766e?logo=chrome&logoColor=white)](https://www.pconline.com.cn) | New protocol by Google and Microsoft enabling AI agents to interact directly with web kernels without simulating human operations |
| Cloudflare Agent Cloud | 2026-04 | [![Docs](https://img.shields.io/badge/Docs-Cloudflare-2563eb?logo=cloudflare&logoColor=white)](https://blog.cloudflare.com) | Infrastructure to power millions of autonomous, long-running web agents |
| Ace-Skill | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-2605.10000-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.10000) | Bootstraps multimodal agents with prioritized and clustered evolution; 35B MoE matching proprietary performance |
[Back to top](#top)

---
## Skills, Tools, and Harnesses

### Core Skills and Prompt Libraries
| Resource | Type | Links | Why It Is Useful |
| --- | --- | --- | --- |
| `awesome-gpt-image-2` | prompt and style skill library | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/freestylefly/awesome-gpt-image-2) | High-quality prompt-as-code and style library for agentic visual creation workflows |
| `gpt_image_2_skill` | Codex skill | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/wuyoscar/gpt_image_2_skill) | Compact, practical skill for repeatable image generation and editing inside a coding-agent workflow |
| `awesome-agent-skills` | curated skill collection | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/VoltAgent/awesome-agent-skills) | Curated collection of 1000+ agent skills from official dev teams and community |
| `ToDiagram/skills` | diagram generation skill | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/todiagram/skills) | Public repository for installable agent skills producing reviewable diagrams from code and natural language |
| `MCP Skills Catalog` | skill registry | [![Web](https://img.shields.io/badge/Web-Skills_Catalog-0f766e?logo=json&logoColor=white)](https://model-context-protocol.com/skills) | Open, machine-readable catalog of reusable skills for AI coding agents; each skill wraps a real tool, API, or workflow |
| OpenAI `skills` + `skill-installer` | skill infrastructure | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/openai/skills) | The cleanest install path for Codex-native reusable skills, including image and workflow skills relevant to visual-agent prototyping |
| `sf-diagram-nanobananapro` | visual creation skill | [![Web](https://img.shields.io/badge/Web-Agent_Skills-0f766e?logo=salesforce&logoColor=white)](https://agentskills.so) | Visual content generation and AI sub-agent for Salesforce development using Gemini CLI with Nano Banana Pro extension |
| `Dev-Browser Skill` | visual debugging skill | [![Web](https://img.shields.io/badge/Web-Dev_To-0f766e?logo=devdotto&logoColor=white)](https://dev.to) | Headless browser skill for coding agents to navigate localhost, click buttons, and verify CSS rendering |

### Perception, Parsing, and Grounding Tools
| Tool | Type | Links | Best For |
| --- | --- | --- | --- |
| OmniParser | GUI parser | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/microsoft/OmniParser) | Converting screenshots into interactable regions and semantics for vision-only GUI agents |
| OmniMCP | OmniParser bridge | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/OpenAdaptAI/OmniMCP) | Wrapping visual parsing into a tool-friendly control surface for agent systems |
| OpenAdapt Grounding | grounding tooling | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/OpenAdaptAI/openadapt-grounding) | Practical grounding and operator-facing automation utilities inside the OpenAdapt stack |
| UI-Zoomer | zoom-in utility | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/UI-Zoomer) | Useful whenever small icons, dense ribbons, or high-resolution UIs break direct grounding |
| ShowUI | VLA-style GUI model stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/showlab/ShowUI) | Useful reference implementation when you want a unified screenshot-to-action pipeline |
| `RegionFocus` | grounding test-time scaling | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/tiangeluo/RegionFocus) | Visual test-time scaling for GUI agent grounding; achieves SOTA on ScreenSpot-Pro (61.6%); ICCV 2025 |
| `SpiritSight` | GUI navigation agent | [![arXiv](https://img.shields.io/badge/arXiv-2505.xxx-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.xxx) | Vision-based end-to-end GUI agent with multi-level GUI-Lasagne dataset and auto-regressive visual input |
| `Aguvis` | pure vision GUI agent | [![Web](https://img.shields.io/badge/Web-Bytez-0f766e?logo=bytez&logoColor=white)](https://bytez.com) | Unified pure-vision framework for autonomous GUI interaction; operates directly on screen images |
| `MEGA-GUI` | multi-stage grounding agent | [![arXiv](https://img.shields.io/badge/arXiv-2511.xxx-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.xxx) | Multi-stage grounding framework with coarse-to-fine ROI selection and bidirectional zoom algorithm |

### Agent Runtimes, Sandboxes, and Operator Stacks
| Stack | Type | Links | Best For |
| --- | --- | --- | --- |
| UI-TARS-desktop | native desktop agent stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/bytedance/UI-TARS-desktop) | End-to-end desktop operator workflows and native GUI-agent experimentation |
| Agent-S | hierarchical operator framework | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/simular-ai/Agent-S) | Planning, memory, and experience reuse for computer-use agents |
| OpenCUA | open foundation stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OpenCUA) | Open training and evaluation substrate for computer-use agents |
| Cua | computer-use infrastructure | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/trycua/cua) | Open-source infrastructure, sandboxes, and SDKs for computer-use-agent development |
| OpenAdapt | operator and desktop automation stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/OpenAdaptAI/OpenAdapt) | Desktop control, data capture, evaluation, and agent-building utilities in one ecosystem |
| ScreenPipe | local screen-memory runtime | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/screenpipe/screenpipe) | Persistent visual memory and capture for long-running assistants and operator loops |
| `amla-sandbox` | WASM agent sandbox | [![PyPI](https://img.shields.io/badge/PyPI-amla_sandbox-0f766e?logo=pypi&logoColor=white)](https://pypi.org/project/amla-sandbox) | WASM sandbox with capability enforcement; agents can only call explicitly provided tools with constraints |
| `EvoAgentX` | self-evolving agent framework | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EvoAgentX) | Open-source framework for building self-evolving AI agent ecosystems with automated workflow generation |
| `Kiro Agent` | computer-use agent infra | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/kiro-agent) | Open-source computer-use agent infrastructure with demonstration recording and replay capabilities |
| `MCP Workbench` | protocol debugger | [![Web](https://img.shields.io/badge/Web-Orkes-0f766e?logo=debug&logoColor=white)](https://www.orkes.io) | Open-source visual debugger for MCP servers; inspect tool calls, resources, and prompts |
| `FluxVLA Engine` | VLA engineering base | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/limxdynamics/FluxVLA) | Standardized VLA engineering base for embodied intelligence research, application development, and deployment |
| `HoloBrain / RoboOrchard` | embodied AI framework | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/HorizonRobotics/HoloBrain) | Full-stack VLA framework including base model and RoboOrchard infrastructure for robot learning |
| `Orchard` | agentic modeling framework | [![arXiv](https://img.shields.io/badge/arXiv-2605.xxx-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.xxx) [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/orchard) | Open-source agentic modeling framework for training and evaluating LLM agents |
| `Mirage-1` | hierarchical skills module | [![arXiv](https://img.shields.io/badge/arXiv-260x.xxx-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/260x.xxx) | Hierarchical Multimodal Skills (HMS) module for augmenting and updating GUI agents with open-ended knowledge |

### Harnesses, Eval Suites, and Benchmark Orchestration
| Resource | Type | Links | Best For |
| --- | --- | --- | --- |
| BrowserGym | benchmark framework | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/ServiceNow/BrowserGym) | Standardized browser-agent environments and task wrappers |
| AgentLab | evaluation harness | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/ServiceNow/AgentLab) | Running, comparing, and analyzing browser-agent experiments on WebArena-style tasks |
| ScreenSuite | GUI-agent benchmark suite | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/ryoungj/ScreenSuite) | Consolidated GUI-agent benchmarking across multiple perception and action tasks |
| lmms-eval | multimodal eval toolkit | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EvolvingLMMs-Lab/lmms-eval) | Strong general-purpose evaluation toolkit with multimodal and agent-adjacent value |
| VisualWebArena | benchmark environment | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/web-arena-x/visualwebarena) | Visually grounded browser-agent evaluation |
| OSWorld | desktop benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OSWorld) | Flagship open benchmark for real computer-use agents across applications |
| WindowsAgentArena | Windows benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/microsoft/WindowsAgentArena) | Scalable evaluation on Windows applications and workflows |
| AndroidWorld | Android benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/google-research/android_world) | Dynamic Android environment with large task diversity |
| EmbodiedBench | embodied-agent benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EmbodiedBench/EmbodiedBench) | Unified benchmark layer for embodied multimodal agents |
| DoomArena | safety and stress benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/trycua/doom-arena) | Useful stress-testing environment for agent robustness and control |
| `ClawGUI-Eval` | unified GUI eval pipeline | [![arXiv](https://img.shields.io/badge/arXiv-2604.xxx-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.xxx) | Fully standardized evaluation pipeline across 6 benchmarks and 11+ models; 95.8% reproduction fidelity |
| `openadapt-evals` | GUI agent eval framework | [![PyPI](https://img.shields.io/badge/PyPI-openadapt_evals-0f766e?logo=pypi&logoColor=white)](https://pypi.org/project/openadapt-evals) | Unified framework for evaluating GUI automation agents against WAA; cloud VM infra for parallel evaluation |
| `MobiBench` | mobile GUI agent benchmark | [![arXiv](https://img.shields.io/badge/arXiv-2601.xxx-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.xxx) | First modular and multi-path-aware offline benchmarking framework for mobile GUI agents; 94.72% human agreement |
| `MAS-Bench` | shortcut-augmented mobile benchmark | [![arXiv](https://img.shields.io/badge/arXiv-2604.xxx-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.xxx) | Pioneers evaluation of GUI-shortcut hybrid agents; assesses autonomous shortcut generation capability |
| `GUI-CEval` | Chinese mobile GUI benchmark | [![Web](https://img.shields.io/badge/Web-CVPR-0f766e?logo=cvpr&logoColor=white)](https://cvpr.thecvf.com) | Hierarchical Chinese benchmark spanning 201 apps, 4 device types, 5 evaluation dimensions |
| `CUActSpot` | computer-use interaction benchmark | [![arXiv](https://img.shields.io/badge/arXiv-2605.xxx-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.xxx) | New benchmark covering complex interactions across five modalities: GUI, text, table, canvas, and natural image |
| `OpenAgentSafety` | agent safety evaluation framework | [![arXiv](https://img.shields.io/badge/arXiv-2507.06134-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.06134) | Modular framework for evaluating agents across 8 risk categories with 350+ multi-turn tasks; ICLR 2026 |
| `OS-SPEAR` | OS agent analysis toolkit | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/Wuzheng02/OS-SPEAR) | Comprehensive toolkit evaluating 22 OS agents across Safety, Performance, Efficiency, and Robustness |
| `AgentVista` | challenging visual agent benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/hkust-nlp/AgentVista) | 25 sub-domains across 7 categories; best model achieves only 27.3% accuracy |

### Demonstration Capture and Data Tooling
| Resource | Type | Links | Why It Is Useful |
| --- | --- | --- | --- |
| OpenAdapt Desktop | data capture | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/OpenAdaptAI/openadapt-desktop) | Records and structures real computer-use traces for training, replay, and analysis |
| OpenAdapt-ML | model training layer | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/OpenAdaptAI/openadapt-ml) | Turns captured interaction traces into trainable agent pipelines |
| ShowUI-Aloha | screen-recording supervision | [![arXiv](https://img.shields.io/badge/arXiv-2601.07181-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.07181) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/showlab/ShowUI) | Human demonstration pipeline for GUI-agent training |
| OpenCUA / AgentNet family | open agent data stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OpenCUA) | Useful umbrella for open datasets, models, and benchmark components |
| GroundCUA / GroundNext | grounding data engine | [![arXiv](https://img.shields.io/badge/arXiv-2511.07332-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.07332) | Useful when desktop grounding quality is the bottleneck in a larger agent stack |
| CUA-Suite | research suite | [![arXiv](https://img.shields.io/badge/arXiv-2603.24440-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.24440) | Useful when you need one consolidated suite for grounding, video, and UI evaluation |
| Video2GUI | trajectory synthesis | [![arXiv](https://img.shields.io/badge/arXiv-2605.14747-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.14747) | Fresh 2026 pipeline for turning tutorial videos into large-scale pretraining trajectories |
| ScreenPipe | continuous capture and memory | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/screenpipe/screenpipe) | Helpful for memory-heavy assistants and screen-native agents |
| `@arach/vif` | screen capture for agents | [![NPM](https://img.shields.io/badge/NPM-@arach/vif-0f766e?logo=npm&logoColor=white)](https://www.npmjs.com/package/@arach/vif) | Screen capture built for AI agents and LLMs; declarative storyboards, CLI-native, agent-first design |
| `@mcpware/pagecast` | page recording MCP tool | [![NPM](https://img.shields.io/badge/NPM-@mcpware/pagecast-0f766e?logo=npm&logoColor=white)](https://www.npmjs.com/package/@mcpware/pagecast) | MCP tools for recording and interacting with web pages; video-captured interactions |
| `ProofShot` | agent session recorder | [![Web](https://img.shields.io/badge/Web-EveryDev-0f766e?logo=cli&logoColor=white)](https://www.everydev.ai) | CLI tool for AI coding agents to prove their work with video recording, error logs, and proof artifacts |
| `glasspipe` | agent trace dashboard | [![PyPI](https://img.shields.io/badge/PyPI-glasspipe-0f766e?logo=pypi&logoColor=white)](https://pypi.org/project/glasspipe) | Visual timeline dashboard capturing every LLM call, every tool, every step; shareable trace links |
| `Guidde` | visual imitation learning | [![Web](https://img.shields.io/badge/Web-Guidde-0f766e?logo=guidde&logoColor=white)](https://www.guidde.com) | AI agents trained on human expert video instead of documentation; replaces 6-7 disconnected tools with single AI-native platform |
| `Moonlake AI 3D Agent` | world-building agent | [![Web](https://img.shields.io/badge/Web-Moonlake-0f766e?logo=unrealengine&logoColor=white)](https://www.moonlake.ai) | Builds and refines complex virtual worlds from images; integrates with Blender and creative workflows |

### Embodied and Robotics Tooling
| Tool | Type | Links | Best For |
| --- | --- | --- | --- |
| OpenVLA | VLA model and training stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/openvla/openvla) | Open embodied-agent baseline with training and evaluation support |
| LeRobot | robotics learning stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/huggingface/lerobot) | Practical robotics dataset, policy, and evaluation tooling with strong community adoption |
| LIBERO | lifelong robot benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/Lifelong-Robot-Learning/LIBERO) | Continual and compositional robot manipulation evaluation |
| LIBERO-plus | updated embodied benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/tylerlum/libero_plus) | Useful extension when evaluating broader VLA-style generalization |
| RLBench | robot learning environment | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/stepjam/RLBench) | Widely used manipulation benchmark environment for embodied control research |
| EmbodiedBench | multimodal embodied evaluation | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EmbodiedBench/EmbodiedBench) | Convenient benchmark layer for comparing embodied multimodal agents |
| `StarVLA` | VLA codebase | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/StarVLA/StarVLA) | Most comprehensive open-source VLA framework; Lego-like codebase for VLA research and prototyping |
| `RIO` | robot I/O framework | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/RIO) | Flexible real-time Python framework for cross-embodiment robot control, teleoperation, data formatting, and policy deployment |
| `FluxVLA Engine` | VLA engineering base | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/limxdynamics/FluxVLA) | Standardized VLA engineering base from LimX Dynamics for embodied intelligence research and deployment |
| `HoloBrain / RoboOrchard` | VLA full-stack framework | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/HorizonRobotics/HoloBrain) | Full-stack VLA framework from Horizon Robotics with base model and RoboOrchard infrastructure |
| `EmbodiChain` | VLA auto-training toolchain | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EmbodiChain) | First toolchain that auto-trains VLA models with 100% synthetic data; zero-shot sim-to-real transfer |
| `SimWorld` | physical agent simulator | [![Web](https://img.shields.io/badge/Web-SimWorld-0f766e?logo=simulator&logoColor=white)](https://simworld.ai) | Open-ended simulator for agents in physical environments with task definition, agent roles, rewards, and evaluation metrics |
| `Amazon Bedrock AgentCore` | spatial simulation framework | [![Docs](https://img.shields.io/badge/Docs-AWS-2563eb?logo=amazonaws&logoColor=white)](https://aws.amazon.com) | World-service operations as MCP-compatible tools; spatial simulations with generative agents |
| `World Craft` | world creation framework | [![arXiv](https://img.shields.io/badge/arXiv-2601.xxx-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.xxx) | Agentic world creation framework generating executable, visualizable AI Town from user textual descriptions |
| `Roblox Agentic AI` | text-to-game planning | [![Web](https://img.shields.io/badge/Web-Roblox-0f766e?logo=roblox&logoColor=white)](https://roblox.com) | Text-to-game planning and AI playtesting; agentic workflows for world construction in gaming platforms |

[Back to top](#top)
---
### Perception, Parsing, and Grounding Tools
| Tool | Type | Links | Best For |
| --- | --- | --- | --- |
| OmniParser | GUI parser | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/microsoft/OmniParser) | Converting screenshots into interactable regions and semantics for vision-only GUI agents |
| OmniMCP | OmniParser bridge | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/OpenAdaptAI/OmniMCP) | Wrapping visual parsing into a tool-friendly control surface for agent systems |
| OpenAdapt Grounding | grounding tooling | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/OpenAdaptAI/openadapt-grounding) | Practical grounding and operator-facing automation utilities inside the OpenAdapt stack |
| UI-Zoomer | zoom-in utility | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/UI-Zoomer) | Useful whenever small icons, dense ribbons, or high-resolution UIs break direct grounding |
| ShowUI | VLA-style GUI model stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/showlab/ShowUI) | Useful reference implementation when you want a unified screenshot-to-action pipeline |
[Back to top](#top)

---
### Agent Runtimes, Sandboxes, and Operator Stacks
| Stack | Type | Links | Best For |
| --- | --- | --- | --- |
| UI-TARS-desktop | native desktop agent stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/bytedance/UI-TARS-desktop) | End-to-end desktop operator workflows and native GUI-agent experimentation |
| Agent-S | hierarchical operator framework | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/simular-ai/Agent-S) | Planning, memory, and experience reuse for computer-use agents |
| OpenCUA | open foundation stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OpenCUA) | Open training and evaluation substrate for computer-use agents |
| Cua | computer-use infrastructure | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/trycua/cua) | Open-source infrastructure, sandboxes, and SDKs for computer-use-agent development |
| OpenAdapt | operator and desktop automation stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/OpenAdaptAI/OpenAdapt) | Desktop control, data capture, evaluation, and agent-building utilities in one ecosystem |
| ScreenPipe | local screen-memory runtime | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/screenpipe/screenpipe) | Persistent visual memory and capture for long-running assistants and operator loops |
[Back to top](#top)

---
### Harnesses, Eval Suites, and Benchmark Orchestration
| Resource | Type | Links | Best For |
| --- | --- | --- | --- |
| BrowserGym | benchmark framework | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/ServiceNow/BrowserGym) | Standardized browser-agent environments and task wrappers |
| AgentLab | evaluation harness | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/ServiceNow/AgentLab) | Running, comparing, and analyzing browser-agent experiments on WebArena-style tasks |
| ScreenSuite | GUI-agent benchmark suite | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/ryoungj/ScreenSuite) | Consolidated GUI-agent benchmarking across multiple perception and action tasks |
| lmms-eval | multimodal eval toolkit | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EvolvingLMMs-Lab/lmms-eval) | Strong general-purpose evaluation toolkit with multimodal and agent-adjacent value |
| VisualWebArena | benchmark environment | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/web-arena-x/visualwebarena) | Visually grounded browser-agent evaluation |
| OSWorld | desktop benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OSWorld) | Flagship open benchmark for real computer-use agents across applications |
| WindowsAgentArena | Windows benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/microsoft/WindowsAgentArena) | Scalable evaluation on Windows applications and workflows |
| AndroidWorld | Android benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/google-research/android_world) | Dynamic Android environment with large task diversity |
| EmbodiedBench | embodied-agent benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EmbodiedBench/EmbodiedBench) | Unified benchmark layer for embodied multimodal agents |
| DoomArena | safety and stress benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/trycua/doom-arena) | Useful stress-testing environment for agent robustness and control |
[Back to top](#top)

---
### Demonstration Capture and Data Tooling
| Resource | Type | Links | Why It Is Useful |
| --- | --- | --- | --- |
| OpenAdapt Desktop | data capture | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/OpenAdaptAI/openadapt-desktop) | Records and structures real computer-use traces for training, replay, and analysis |
| OpenAdapt-ML | model training layer | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/OpenAdaptAI/openadapt-ml) | Turns captured interaction traces into trainable agent pipelines |
| ShowUI-Aloha | screen-recording supervision | [![arXiv](https://img.shields.io/badge/arXiv-2601.07181-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.07181) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/showlab/ShowUI) | Human demonstration pipeline for GUI-agent training |
| OpenCUA / AgentNet family | open agent data stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OpenCUA) | Useful umbrella for open datasets, models, and benchmark components |
| GroundCUA / GroundNext | grounding data engine | [![arXiv](https://img.shields.io/badge/arXiv-2511.07332-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.07332) | Useful when desktop grounding quality is the bottleneck in a larger agent stack |
| CUA-Suite | research suite | [![arXiv](https://img.shields.io/badge/arXiv-2603.24440-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.24440) | Useful when you need one consolidated suite for grounding, video, and UI evaluation |
| Video2GUI | trajectory synthesis | [![arXiv](https://img.shields.io/badge/arXiv-2605.14747-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.14747) | Fresh 2026 pipeline for turning tutorial videos into large-scale pretraining trajectories |
| ScreenPipe | continuous capture and memory | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/screenpipe/screenpipe) | Helpful for memory-heavy assistants and screen-native agents |
[Back to top](#top)

---
### Embodied and Robotics Tooling
| Tool | Type | Links | Best For |
| --- | --- | --- | --- |
| OpenVLA | VLA model and training stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/openvla/openvla) | Open embodied-agent baseline with training and evaluation support |
| LeRobot | robotics learning stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/huggingface/lerobot) | Practical robotics dataset, policy, and evaluation tooling with strong community adoption |
| LIBERO | lifelong robot benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/Lifelong-Robot-Learning/LIBERO) | Continual and compositional robot manipulation evaluation |
| LIBERO-plus | updated embodied benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/tylerlum/libero_plus) | Useful extension when evaluating broader VLA-style generalization |
| RLBench | robot learning environment | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/stepjam/RLBench) | Widely used manipulation benchmark environment for embodied control research |
| EmbodiedBench | multimodal embodied evaluation | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EmbodiedBench/EmbodiedBench) | Convenient benchmark layer for comparing embodied multimodal agents |
[Back to top](#top)

---

## Benchmarks and Environments
| Area | Benchmark / Environment | Links | Why It Matters |
| --- | --- | --- | --- |
| Web | WebArena | [![arXiv](https://img.shields.io/badge/arXiv-2307.13854-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2307.13854) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/web-arena-x/webarena) | Foundational realistic web-agent benchmark |
| Web | VisualWebArena | [![arXiv](https://img.shields.io/badge/arXiv-2401.13649-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.13649) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/web-arena-x/visualwebarena) | Adds screenshot-grounded perception to browser-agent evaluation |
| Web | BrowserGym | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/ServiceNow/BrowserGym) | Reusable harness for browser-agent experimentation at scale |
| Web | WorkArena | [![arXiv](https://img.shields.io/badge/arXiv-2403.07718-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2403.07718) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ServiceNow/WorkArena) | Enterprise workflow benchmark centered on knowledge-work tasks |
| Web | WebArena-Verified | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/web-arena-x/webarena-verified) | Cleaner, more controlled evaluation variant for WebArena-style research |
| Desktop | OSWorld | [![arXiv](https://img.shields.io/badge/arXiv-2404.07972-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2404.07972) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OSWorld) | Flagship open benchmark for real desktop computer use |
| Desktop | UI-Vision | [![arXiv](https://img.shields.io/badge/arXiv-2503.15661-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.15661) | Fine-grained offline benchmark for desktop perception, layout grounding, and action prediction |
| Desktop | OmniACT | [![arXiv](https://img.shields.io/badge/arXiv-2402.17553-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.17553) | Evaluates executable automation rather than only low-level action traces |
| Desktop | WindowsAgentArena | [![arXiv](https://img.shields.io/badge/arXiv-2409.08264-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2409.08264) [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/microsoft/WindowsAgentArena) | Scalable Windows evaluation environment |
| Mobile | AndroidWorld | [![arXiv](https://img.shields.io/badge/arXiv-2405.14573-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2405.14573) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/google-research/android_world) | Dynamic Android benchmark with broad task diversity |
| Mobile | MobileAgentBench | [![arXiv](https://img.shields.io/badge/arXiv-2406.08184-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2406.08184) | Efficient and practical benchmark for mobile GUI agents across open-source apps |
| Mobile | SPA-Bench | [![arXiv](https://img.shields.io/badge/arXiv-2410.15164-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.15164) | Strong multilingual smartphone benchmark with plug-and-play integration |
| Mobile | MemGUI-Bench | [![arXiv](https://img.shields.io/badge/arXiv-2602.06075-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.06075) | Cross-session and cross-temporal memory evaluation for GUI agents |
| Mobile | DynamicGUIBench | [![arXiv](https://img.shields.io/badge/arXiv-2604.25380-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.25380) | Dynamic GUI environments rather than frozen UI snapshots |
| Grounding | ScreenSpot-Pro | [![arXiv](https://img.shields.io/badge/arXiv-2504.07981-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.07981) | High-resolution professional-screen grounding benchmark |
| Grounding | GUI-Perturbed | [![arXiv](https://img.shields.io/badge/arXiv-2604.14262-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14262) | Robustness diagnostics for perturbations and relational instructions |
| Computer use | AssistantBench | [![arXiv](https://img.shields.io/badge/arXiv-2407.15711-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2407.15711) | Moves beyond short episodes toward realistic, time-consuming assistant tasks |
| Computer use | VideoWebArena | [![arXiv](https://img.shields.io/badge/arXiv-2410.19100-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.19100) | Long-context video understanding inside web-agent workflows |
| Computer use | CUA-Suite | [![arXiv](https://img.shields.io/badge/arXiv-2603.24440-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.24440) | Consolidated suite for modern computer-use-agent research |
| Security | VPI-Bench | [![arXiv](https://img.shields.io/badge/arXiv-2506.02456-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.02456) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/boyugou/VPI-Bench) | Visual prompt-injection benchmark for GUI agents |
| Safety | HazardArena | [![arXiv](https://img.shields.io/badge/arXiv-2604.12447-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.12447) | Semantic safety evaluation for VLA systems |
| Embodied | EmbodiedBench | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EmbodiedBench/EmbodiedBench) | Unified embodied multimodal benchmark layer |
| Embodied | LIBERO | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/Lifelong-Robot-Learning/LIBERO) | Continual manipulation benchmark widely used in robot learning |
| Embodied | RLBench | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/stepjam/RLBench) | Strong manipulation environment for embodied control evaluation |
[Back to top](#top)

---

## Official Docs and Engineering Notes
| Resource | Links | Why Read It |
| --- | --- | --- |
| OpenAI: Computer-Using Agent | [![Docs](https://img.shields.io/badge/Docs-OpenAI-2563eb?logo=readthedocs&logoColor=white)](https://openai.com/index/computer-using-agent/) | Product and research framing for modern computer-use agents |
| OpenAI API: Computer Use Guide | [![Docs](https://img.shields.io/badge/Docs-OpenAI_API-2563eb?logo=readthedocs&logoColor=white)](https://platform.openai.com/docs/guides/tools-computer-use) | Developer-facing usage guide for building computer-use workflows |
| Anthropic: Developing a Computer Use Model | [![Docs](https://img.shields.io/badge/Docs-Anthropic-2563eb?logo=readthedocs&logoColor=white)](https://www.anthropic.com/news/developing-computer-use) | One of the best public engineering writeups on GUI-agent development |
| Anthropic: Introducing computer use | [![Docs](https://img.shields.io/badge/Docs-Anthropic-2563eb?logo=readthedocs&logoColor=white)](https://www.anthropic.com/news/3-5-models-and-computer-use) | Concise system framing plus deployment context |
| Google DeepMind: Gemini Robotics | [![Docs](https://img.shields.io/badge/Docs-Gemini-2563eb?logo=readthedocs&logoColor=white)](https://deepmind.google/blog/gemini-robotics-brings-ai-into-the-physical-world/) | Frontier industry view on embodied visual agents |
| Google DeepMind: Gemini Robotics On-Device | [![Docs](https://img.shields.io/badge/Docs-Gemini-2563eb?logo=readthedocs&logoColor=white)](https://deepmind.google/discover/blog/gemini-robotics-on-device-brings-ai-to-local-robotic-devices/) | Practical view on low-latency on-device VLA deployment |
| Kimi K2.5 Tech Blog | [![Docs](https://img.shields.io/badge/Docs-Kimi-2563eb?logo=readthedocs&logoColor=white)](https://www.kimi.com/blog/kimi-k2-5) | Official blog on visual agentic intelligence and parallel agent orchestration |
| SenseNova U1 Docs | [![Docs](https://img.shields.io/badge/Docs-SenseNova-2563eb?logo=readthedocs&logoColor=white)](https://www.sensenova.cn/models) | Practical docs on native multimodal agent models for real workflows |
[Back to top](#top)

---

## Suggested Reading Paths
### Path A: GUI and Computer-Use Agent Builder
1. [SeeClick](https://arxiv.org/abs/2401.10935)
2. [ScreenAI](https://arxiv.org/abs/2402.04615)
3. [Ferret-UI](https://arxiv.org/abs/2404.05719)
4. [OmniParser](https://arxiv.org/abs/2408.00203)
5. [VisualWebArena](https://arxiv.org/abs/2401.13649)
6. [OSWorld](https://arxiv.org/abs/2404.07972)
7. [UI-TARS](https://arxiv.org/abs/2501.12326)
8. [Agent S2](https://arxiv.org/abs/2504.00906)
9. [OpenCUA](https://arxiv.org/abs/2508.09123)
10. [UI-Copilot](https://arxiv.org/abs/2604.13822)
11. [ActionEngine](https://arxiv.org/abs/2602.20502)
12. [OS-Symphony](https://arxiv.org/abs/2601.07779)
### Path B: Evaluation, Harness, and Reliability
1. [WebArena](https://arxiv.org/abs/2307.13854)
2. [VisualWebArena](https://arxiv.org/abs/2401.13649)
3. [WorkArena](https://arxiv.org/abs/2403.07718)
4. [OSWorld](https://arxiv.org/abs/2404.07972)
5. [ScreenSpot-Pro](https://arxiv.org/abs/2504.07981)
6. [Agent-X](https://arxiv.org/abs/2505.24876)
7. [VPI-Bench](https://arxiv.org/abs/2506.02456)
8. [MemGUI-Bench](https://arxiv.org/abs/2602.06075)
9. [GUI-Perturbed](https://arxiv.org/abs/2604.14262)
10. [HazardArena](https://arxiv.org/abs/2604.12447)
### Path C: Embodied Visual Agents and Robotics
1. [RT-2](https://arxiv.org/abs/2307.15818)
2. [OpenVLA](https://arxiv.org/abs/2406.09246)
3. [Magma](https://arxiv.org/abs/2502.13130)
4. [Interleave-VLA](https://arxiv.org/abs/2505.02152)
5. [ChatVLA-2](https://arxiv.org/abs/2505.21906)
6. [StemVLA](https://arxiv.org/abs/2602.23721)
7. [World-Value-Action Model](https://arxiv.org/abs/2604.14732)
### Path D: Agentic Visual Reasoning and Creation
1. [DeepEyes](https://arxiv.org/abs/2505.14362)
2. [CIGEval](https://arxiv.org/abs/2504.07046)
3. [Mind-Brush](https://arxiv.org/abs/2602.01756)
4. [VisionCreator](https://arxiv.org/abs/2603.02681)
5. [Visual Generation in the New Era](https://arxiv.org/abs/2604.28185)
6. [ImAgent](https://arxiv.org/abs/2511.11483)
7. [GenAgent](https://arxiv.org/abs/2601.18543)
8. [M3](https://arxiv.org/abs/2602.06166)
9. [Gen-Searcher](https://arxiv.org/abs/2603.28767)
10. [GEMS](https://arxiv.org/abs/2603.28088)
11. [GenArtist](https://arxiv.org/abs/2407.05600)
12. [Agent Banana](https://arxiv.org/abs/2602.09084)
[Back to top](#top)
---

## Build Paths by Workflow
| Workflow | Recommended Stack |
| --- | --- |
| Desktop and browser computer-use prototyping | `OmniParser` + `UI-TARS-desktop` + `Agent-S` + `BrowserGym` + `OSWorld` |
| Long-horizon GUI-agent research | `OpenCUA` + `Cua` + `UI-Copilot` + `OS-Symphony` + `CUA-Suite` |
| Mobile GUI agents | `Ferret-UI` + `AndroidWorld` + `MemGUI-Bench` + `DynamicGUIBench` |
| Visual-grounding and parsing research | `ScreenAI` + `SeeClick` + `UGround` + `GUI-Eyes` + `UI-Zoomer` |
| Agentic visual creation workflows | `awesome-gpt-image-2` + `gpt_image_2_skill` + `Mind-Brush` + `VisionCreator` + `Gen-Searcher` + `GEMS` + `Agent Banana` |
| Data capture and imitation pipelines | `OpenAdapt Desktop` + `OpenAdapt-ML` + `ShowUI-Aloha` + `ScreenPipe` |
| Embodied VLA experimentation | `OpenVLA` + `LeRobot` + `LIBERO` + `RLBench` + `EmbodiedBench` |
| Agentic visual foundation model research | `Kimi K2.5` + `Qwen3.6-35B-A3B` + `SenseNova-U1` + `OpenAI CUA` + `Anthropic Claude 3.5 computer use` |
[Back to top](#top)

---

## Related Awesome Repositories
| Repository | Links | Notes |
| --- | --- | --- |
| Awesome-GUI-Agents | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/Awesome-GUI-Agents) | Strong companion list focused on GUI grounding, long-horizon automation, and benchmarks |
| GUI-Agents-Paper-List | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/OSU-NLP-Group/GUI-Agents-Paper-List) | Systematic, community-maintained paper index for GUI agents |
| awesome-ui-agents | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/opendilab/awesome-ui-agents) | Useful neighboring list if you want extra depth on UI agents specifically |
| acu | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/trycua/acu) | Good companion collection around computer-use-agent infrastructure and resources |
| Awesome Multimodal Modeling | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/OpenEnvision/Awesome-Multimodal-Modeling) | Broader multimodal map beyond the stricter visual-agent boundary used here |
| Evolving Visual Generation | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EvolvingLMMs-Lab/Evolving-Visual-Generation) | Useful adjacent list for the visual-creation side of agentic systems |
| awesome-agent-skills | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/VoltAgent/awesome-agent-skills) | Curated collection of 1000+ agent skills from official dev teams and community |
| awesome-agents | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/kyrolabs/awesome-agents) | General agent frameworks and tools; good for understanding broader agent runtimes |
| Awesome-AI-Agents | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/Jenqyang/Awesome-AI-Agents) | Collection of LLM-based autonomous agents; helpful for cross-referencing agent architectures |
[Back to top](#top)

---
## Curation Principles
- Prefer works that define a new capability, benchmark, training recipe, or systems bottleneck for agentic visual systems.
- Prefer official artifacts whenever possible: paper, code, benchmark, toolkit, or docs.
- Exclude broad multimodal or image-generation models unless they are explicitly agentic, tool-using, or benchmark-central.
- Separate `perception`, `computer use`, `embodied action`, `agentic creation`, and `evaluation` rather than collapsing them into one bucket.
- Keep builder-facing resources first-class: skills, runtimes, sandboxes, harnesses, parsers, and data pipelines matter as much as papers.
- Add recent work only when it improves the map rather than inflating it.
[Back to top](#top)
---
## Maintained By

This repository is maintained by the **OpenEnvision**. If you’d like to help maintain or curate specific tracks (e.g., GUI agents, embodied VLA, agentic visual creation), please open an issue or pull request.
[Back to top](#top)

---
## How to Contribute
Pull requests are warmly welcome, especially for:
- new `2026+` visual-agent papers with official code, benchmarks, or environments
- missing skills, toolchains, harnesses, or evaluation suites
- open data engines, replay systems, and demonstration-capture tooling
- stronger categorization of embodied, GUI, and agentic visual-creation work
- corrections where a listed work is not agentic enough and should be removed
When adding an item, please include:
- title
- year
- one-sentence note on why it matters
- official paper and, when available, official code
- the correct category under this agentic boundary
If you maintain a relevant project, benchmark, or dataset, a concise and well-scoped PR is the fastest way to improve the map.
If you find the list useful, giving the repository a star is also greatly appreciated.
[Back to top](#top)
---
## Citation
If you find this curated list useful for your research or engineering work, please consider citing it as:
```bibtex
@misc{awesome-visual-agent,
  title   = {Awesome Visual Agent: A research-driven map of visual agents that perceive, ground, plan, act, create, and evaluate in pixel-grounded environments},
  author  = {OpenEnvision and contributors},
  year    = {2026},
  howpublished = {\\url{https://github.com/OpenEnvision/Awesome-Visual-Agent}},
  note    = {Curated list of agentic visual systems, benchmarks, and tooling}
}
```
[Back to top](#top)
---
## License
This repository is released under the **MIT License**, unless otherwise stated for specific externally linked projects.
[Back to top](#top)

---
## Contributing
See [How to Contribute](#how-to-contribute) for current guidelines. In short:
- Be respectful and constructive.
- Add new items only if they clearly fit the agentic visual-agent boundary.
- Prefer official links and minimal but informative notes.
- Check existing entries for style and badge usage before submitting.
[Back to top](#top)
---
## Acknowledgments
This repository was shaped by the structure and coverage quality of several strong public resources, especially:
- [OpenEnvision/Awesome-Multimodal-Modeling](https://github.com/OpenEnvision/Awesome-Multimodal-Modeling)
- [ZJU-REAL/Awesome-GUI-Agents](https://github.com/ZJU-REAL/Awesome-GUI-Agents)
- [OSU-NLP-Group/GUI-Agents-Paper-List](https://github.com/OSU-NLP-Group/GUI-Agents-Paper-List)
- [opendilab/awesome-ui-agents](https://github.com/opendilab/awesome-ui-agents)
- [EvolvingLMMs-Lab/Evolving-Visual-Generation](https://github.com/EvolvingLMMs-Lab/Evolving-Visual-Generation)
- [freestylefly/awesome-gpt-image-2](https://github.com/freestylefly/awesome-gpt-image-2)
- [wuyoscar/gpt_image_2_skill](https://github.com/wuyoscar/gpt_image_2_skill)
- [VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills)
- [kyrolabs/awesome-agents](https://github.com/kyrolabs/awesome-agents)
- [Jenqyang/Awesome-AI-Agents](https://github.com/Jenqyang/Awesome-AI-Agents)
The goal here is to push beyond a flat link dump and toward a research-and-building index for serious visual-agent work.
[Back to top](#top)
```
