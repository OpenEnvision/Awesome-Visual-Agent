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

> [!IMPORTANT]
> This repository is intentionally **not** a generic multimodal-model list. It focuses on systems that close the loop between **visual perception**, **grounding**, **reasoning**, **memory**, **tool use**, **action**, and, where appropriate, **agentic visual creation**. Broad VLMs, generic image generators, and non-agentic multimodal models are deliberately excluded unless they are directly central to a visual-agent workflow, benchmark, or tooling stack.

> [!TIP]
> If this repository saves you reading time or helps you build visual agents faster, please consider **starring** it and opening a **pull request** for missing papers, tools, benchmarks, or systems notes.

## Table of Contents

- [Why This Repo](#why-this-repo)
- [What Counts as a Visual Agent](#what-counts-as-a-visual-agent)
- [2026 Radar](#2026-radar)
- [Taxonomy at a Glance](#taxonomy-at-a-glance)
- [Link Badge Legend](#link-badge-legend)
- [Research Map](#research-map)
  - [1. Surveys, Roadmaps, and Scope-Setting](#1-surveys-roadmaps-and-scope-setting)
  - [2. Perception, Grounding, and Active Visual Observation](#2-perception-grounding-and-active-visual-observation)
  - [3. GUI and Computer-Use Agents](#3-gui-and-computer-use-agents)
  - [4. Embodied Vision-Language-Action Agents](#4-embodied-vision-language-action-agents)
  - [5. Agentic Visual Reasoning and Creation](#5-agentic-visual-reasoning-and-creation)
  - [6. Safety, Robustness, and Reliability](#6-safety-robustness-and-reliability)
  - [7. Data Engines, Demonstration Pipelines, and Open Foundations](#7-data-engines-demonstration-pipelines-and-open-foundations)
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
- [Contributing](#contributing)
- [Acknowledgments](#acknowledgments)

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

## Link Badge Legend

- Paper: [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/)
- Code: [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/)
- Project / toolkit / repo: [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/)
- Docs: [![Docs](https://img.shields.io/badge/Docs-Reference-2563eb?logo=readthedocs&logoColor=white)](https://platform.openai.com/docs/)

[Back to top](#top)

## 2026 Radar

| Work | Date | Links | Why It Matters |
| --- | --- | --- | --- |
| GUI-Eyes | 2026-01-14 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.09770) | Strong recent step toward tool-augmented perception and adaptive visual grounding for GUI agents. |
| ShowUI-Aloha: Human-Taught GUI Agent | 2026-01-12 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.07181) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/showlab/ShowUI) | Important demonstration pipeline for turning screen recordings into GUI-agent supervision. |
| OS-Symphony | 2026-01-12 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.07779) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OS-Copilot/OS-Symphony) | Memory, reflection, and retrieval-aware computer use in one open framework. |
| MemGUI-Bench | 2026-02-03 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.06075) | Brings cross-session memory into mobile GUI-agent evaluation. |
| ActionEngine | 2026-02-27 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.20502) | Pushes GUI agents from reactive loops toward executable state-machine memory and programmatic plans. |
| CUA-Suite | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.24440) | Unified ecosystem of human-annotated video demonstrations, grounding data, and desktop-centric evaluation for computer-use agents. |
| UI-Copilot | 2026-04-15 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.13822) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/UI-Copilot) | Strong new long-horizon GUI automation result with retrieval and calculator tools. |
| UI-Zoomer | 2026-04-15 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14113) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/UI-Zoomer) | Training-free zoom-in for small targets and dense interfaces. |
| HazardArena | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.12447) | Timely benchmark for semantic safety in vision-language-action systems. |
| GUI-Perturbed | 2026-04-15 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14262) | Reveals how brittle GUI grounding still is under perturbation and relational instructions. |
| DynamicGUIBench | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.25380) | Dynamic, evolving GUI environments instead of static single-frame snapshots. |
| Video2GUI | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.14747) | Fresh large-scale trajectory-synthesis pipeline for GUI-agent pretraining from instructional videos. |
| Vision-Language-Action Safety | 2026-04-26 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.23775) | Strong safety survey on attacks, evaluation, and deployment risks for embodied visual agents. |
| Vision-Language-Action in Robotics: A Survey of Datasets, Benchmarks, and Data Engines | 2026-04-24 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.23001) | Excellent data-centric map of what now bottlenecks VLA progress in practice. |
| World-Value-Action Model | 2026-04-16 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14732) | Notable move toward latent planning and future-state evaluation in embodied agents. |

[Back to top](#top)

## Taxonomy at a Glance

| Track | Core Question | Typical Outputs | Strong Starting Points |
| --- | --- | --- | --- |
| Perception and Grounding | Can the system reliably perceive screens, objects, widgets, and layouts well enough to act? | boxes, regions, UI elements, structured observations | ScreenAI, SeeClick, OmniParser, GUI-Eyes |
| Computer-Use Agents | Can the agent operate websites, desktops, and mobile apps over long horizons? | clicks, typing, navigation, trajectories, recovery plans | WebVoyager, Agent S2, UI-TARS, OS-Symphony |
| Embodied VLA Agents | Can the agent translate visual observations and language into physical action? | robot actions, manipulation traces, embodied plans | RT-2, OpenVLA, Magma, World-Value-Action |
| Agentic Visual Reasoning and Creation | Can the system repeatedly inspect, retrieve, verify, and create visual artifacts as an agentic loop? | zoom traces, visual plans, edits, generated artifacts | DeepEyes, Mind-Brush, VisionCreator |
| Evaluation and Harness | How do we benchmark grounded perception, tool use, memory, safety, and control? | environments, eval suites, leaderboards, diagnostics | VisualWebArena, OSWorld, AndroidWorld, CUA-Suite |
| Builder Stack | What should researchers and engineers actually install to prototype and evaluate visual agents? | skills, parsers, runtimes, sandboxes, robotics stacks | skill-installer, OmniParser, BrowserGym, LeRobot |

[Back to top](#top)

## Research Map

### 1. Surveys, Roadmaps, and Scope-Setting

| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| GUI Agents: A Survey | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2412.13501) | Broad overview of task settings, architectures, benchmarks, and system bottlenecks for GUI agents. |
| A Survey on (M)LLM-Based GUI Agents | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.13865) | Good entry point for planning, grounding, memory, and evaluation in screenshot-grounded agents. |
| Towards Trustworthy GUI Agents: A Survey | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.23434) | Useful for robustness, reliability, and deployment-focused risk analysis. |
| Survey of Vision-Language-Action Models for Embodied Manipulation | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.15201) | Practical survey covering model structure, post-training, datasets, and evaluation. |
| A Survey on Vision-Language-Action Models: An Action Tokenization Perspective | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.01925) | Helpful for understanding why VLA systems differ in control granularity and action representation. |
| Vision-Language-Action in Robotics: A Survey of Datasets, Benchmarks, and Data Engines | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.23001) | Strong infrastructure-first view of embodied visual-agent progress. |
| Vision-Language-Action Safety: Survey, Taxonomy, Challenges and Future Directions | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.23775) | The most timely safety framing for VLA deployment and evaluation. |
| Visual Generation in the New Era: An Evolution from Atomic Mapping to Agentic World Modeling | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.28185) | Best recent roadmap if you care specifically about agentic visual creation rather than plain generation. |

[Back to top](#top)

### 2. Perception, Grounding, and Active Visual Observation

| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| ScreenAI: A Vision-Language Model for UI and Infographics Understanding | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.04615) | Foundational for screen, document, infographic, and layout-heavy visual understanding. |
| CogAgent: A Visual Language Model for GUI Agents | 2023 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2312.08914) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/THUDM/CogAgent) | Early strong open model for screenshot-grounded GUI understanding and action prediction. |
| SeeClick: Harnessing GUI Grounding for Advanced Visual GUI Agents | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.10935) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/njucckevin/SeeClick) | One of the clearest grounding-first papers in GUI-agent research. |
| UGround: Universal Visual Grounding for GUI Agents | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.05243) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OSU-NLP-Group/UGround) | Strong argument for fully visual, human-like GUI grounding without relying on accessibility trees alone. |
| OS-ATLAS: A Foundation Action Model for Generalist GUI Agents | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.23218) | Large cross-platform action-grounding corpus and strong open foundation for GUI control. |
| Ferret-UI: Grounded Mobile UI Understanding with Multimodal LLMs | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2404.05719) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/apple/ml-ferret) | Region-aware mobile grounding and explicit UI understanding. |
| OmniParser for Pure Vision Based GUI Agent | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2408.00203) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/microsoft/OmniParser) | Highly practical parser for converting screenshots into reliable interactable regions. |
| Aguvis: Unified Pure Vision Agents for Autonomous GUI Interaction | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2412.04454) | Important pure-vision direction without dependence on textual trees. |
| ShowUI: One Vision-Language-Action Model for GUI Visual Agent | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2411.17465) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/showlab/ShowUI) | Unified screenshot-conditioned action modeling with strong builder relevance. |
| UI-E2I-Synth: Advancing GUI Grounding with Large-Scale Instruction Synthesis | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.11257) | Useful synthetic-data direction for scaling GUI grounding quality and diversity. |
| GUI-Actor: Coordinate-Free Visual Grounding for GUI Agents | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.03143) | Worth tracking for agent-friendly grounding without brittle coordinate assumptions. |
| Test-Time Reinforcement Learning for GUI Grounding via Region Consistency | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.05615) | Interesting test-time optimization approach for grounding itself. |
| GUI-Eyes: Tool-Augmented Perception for Visual Grounding in GUI Agents | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.09770) | One of the best recent examples of perception improving through explicit tool use. |
| UI-Zoomer: Uncertainty-Driven Adaptive Zoom-In for GUI Grounding | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14113) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/UI-Zoomer) | Practical zoom-in mechanism for dense, high-resolution, and small-target UIs. |

[Back to top](#top)

### 3. GUI and Computer-Use Agents

| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| AppAgent: Multimodal Agents as Smartphone Users | 2023 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2312.13771) | Foundational smartphone-use framing for multimodal agents. |
| SeeAct: GPT-4V(ision) is a Generalist Web Agent, if Grounded | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.01614) | Important early argument that capable web agents depend on grounding quality as much as model scale. |
| WebVoyager: Building an End-to-End Web Agent with Large Multimodal Models | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.13919) | Early strong end-to-end visual web agent. |
| InfiGUIAgent: A Multimodal Generalist GUI Agent with Native Reasoning and Reflection | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2501.04575) | Notable for expectation-reflection and explicit multistep reasoning. |
| UI-TARS: Pioneering Automated GUI Interaction with Native Agents | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2501.12326) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/bytedance/UI-TARS) | One of the strongest open signals for where native GUI agents are heading. |
| OpenCUA: Open Foundations for Computer-Use Agents | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.09123) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OpenCUA) | Strong open data, model, and benchmark foundation for computer-use agents. |
| Magma: A Foundation Model for Multimodal AI Agents | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.13130) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/microsoft/Magma) | Important bridge between digital computer use and physical action settings. |
| Advancing Mobile GUI Agents: A Verifier-Driven Approach to Practical Deployment | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.15937) | Introduces verifier-driven mobile automation with deployment-minded latency tradeoffs. |
| Agent S | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.08164) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/simular-ai/Agent-S) | Strong open framework for hierarchical planning and experience reuse. |
| Agent S2: A Compositional Generalist-Specialist Framework for Computer Use Agents | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.00906) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/simular-ai/Agent-S) | Strong compositional upgrade with specialists for grounding and planning. |
| UItron: A Generalist GUI Agent with Advanced Perception and Planning | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.04246) | Useful reference for more capable perception-planning integration in GUI control. |
| ScaleCUA: Scaling Open-Source Computer Use Agents with Cross-Platform Data | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.15221) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OpenGVLab/ScaleCUA) | Strong data-scaling result and open training/evaluation stack across platforms. |
| EvoCUA: Evolving Computer Use Agents via Learning from Scalable Synthetic Experience | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.15876) | Important 2026 open result on synthetic experience generation and step-level policy optimization. |
| ShowUI-Aloha: Human-Taught GUI Agent | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.07181) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/showlab/ShowUI) | Demonstration-to-agent pipeline built from raw human screen recordings. |
| ActionEngine: From Reactive to Programmatic GUI Agents via State Machine Memory | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.20502) | Moves GUI agents from reactive loops toward executable plans and stateful memory. |
| UI-Copilot: Advancing Long-Horizon GUI Automation via Tool-Integrated Policy Optimization | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.13822) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/UI-Copilot) | Long-horizon automation with retrieval and calculator tools integrated into policy learning. |
| OS-Symphony: A Holistic Framework for Robust and Generalist Computer-Using Agent | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.07779) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OS-Copilot/OS-Symphony) | Strong recent system on memory, reflection, and tutorial retrieval for computer use. |

[Back to top](#top)

### 4. Embodied Vision-Language-Action Agents

| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control | 2023 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2307.15818) | Canonical VLA paper connecting web knowledge and robot control. |
| OpenVLA: An Open-Source Vision-Language-Action Model | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2406.09246) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/openvla/openvla) | Central open baseline for embodied visual-agent work. |
| Interleave-VLA | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.02152) | Extends VLA systems to interleaved image-text instruction following. |
| ChatVLA-2 | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.21906) | Interesting direction for preserving open-world reasoning in embodied agents. |
| VLA^2 | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.14902) | Highlights the value of explicit external modules in unseen-concept manipulation. |
| Magma | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.13130) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/microsoft/Magma) | Useful bridge paper spanning digital computer-use and embodied action settings. |
| StemVLA | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.23721) | Incorporates future 3D geometry and 4D historical context into action prediction. |
| World-Value-Action Model | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14732) | Worth tracking for long-horizon latent planning and implicit future evaluation. |

[Back to top](#top)

### 5. Agentic Visual Reasoning and Creation

| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| DeepEyes: Incentivizing Visual Tool-Use via Visual Reinforcement Learning | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.14362) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/Visual-Agent/DeepEyes) | Strong example of visual reasoning improving through explicit zoom and crop tool use. |
| Mind-Brush: Integrating Agentic Cognitive Search and Reasoning into Image Generation | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.01756) | Clean example of visual creation becoming a retrieval-and-reasoning workflow instead of plain decoding. |
| VisionCreator: A Native Visual-Generation Agentic Model with Understanding, Thinking, Planning and Creation | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.02681) | Explicit understanding-thinking-planning-creation loop for visual generation as an agent. |
| A Unified Agentic Framework for Evaluating Conditional Image Generation | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.07046) | Useful if you care about verifier-driven and agentic evaluation of visual outputs. |
| Visual Generation in the New Era: An Evolution from Atomic Mapping to Agentic World Modeling | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.28185) | Best conceptual map for the agentic visual-creation frontier. |

[Back to top](#top)

### 6. Safety, Robustness, and Reliability

| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| ScreenSpot-Pro: GUI Grounding for Professional High-Resolution Computer Use | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.07981) | Important if you care about professional UIs instead of toy screenshots. |
| Agent-X: Evaluating Deep Multimodal Reasoning in Vision-Centric Agentic Tasks | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.24876) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/mbzuai-oryx/Agent-X) | Valuable for step-level reasoning assessment rather than final success only. |
| VPI-Bench: Visual Prompt Injection Attacks for Computer-Use Agents | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.02456) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/boyugou/VPI-Bench) | Useful benchmark for prompt-injection-style attacks in screenshot-grounded agents. |
| UI-Evol: Automatic Knowledge Evolving for Computer Use Agents | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.21964) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/microsoft/FIVE-UI-Evol) | Tracks how external knowledge must be revised from actual execution, not only retrieved. |
| MemGUI-Bench | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.06075) | Memory is a reliability problem before it is a scaling problem; this benchmark makes that explicit. |
| GUI-Perturbed | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14262) | Strong diagnostic benchmark for perturbation robustness in GUI grounding. |
| HazardArena: Evaluating Semantic Safety in Vision-Language-Action Models | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.12447) | Safety benchmark for semantic hazards in VLA systems. |
| Benchmarking and Improving GUI Agents in High-Dynamic Environments | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.25380) | Introduces DynamicGUIBench and shows why single-frame agents fail in evolving interfaces. |

[Back to top](#top)

### 7. Data Engines, Demonstration Pipelines, and Open Foundations

| Resource | Year | Links | Notes |
| --- | --- | --- | --- |
| UI-E2I-Synth | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.11257) | Synthetic instruction generation pipeline for GUI grounding data. |
| ShowUI-Aloha | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.07181) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/showlab/ShowUI) | One of the most useful open pipelines for converting screen recordings into supervision. |
| OpenCUA | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.09123) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OpenCUA) | Open foundation stack spanning data, benchmarks, and agent development. |
| ScaleCUA | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.15221) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OpenGVLab/ScaleCUA) | Open-source data-scaling pipeline, models, training code, and evaluation environments. |
| GroundCUA / GroundNext | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.07332) | Human-demonstration-derived desktop grounding dataset and strong grounding models for agent pipelines. |
| CUA-Suite | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.24440) | Combines VideoCUA, GroundCUA, and UI-Vision style assets into one research-facing ecosystem. |
| Video2GUI | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.14747) | Converts web GUI videos into structured action trajectories for generalized agent pretraining. |
| OpenAdapt Desktop | ongoing | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OpenAdaptAI/openadapt-desktop) | Captures computer interaction traces that are useful for data collection, replay, and agent training loops. |
| OpenAdapt-ML | ongoing | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OpenAdaptAI/openadapt-ml) | OpenAdapt's model-training layer for turning captured interaction data into agent pipelines. |
| ScreenPipe | ongoing | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/screenpipe/screenpipe) | Continuous screen capture and local memory substrate useful for assistant and operator-style agents. |

[Back to top](#top)

## Skills, Tools, and Harnesses

### Core Skills and Prompt Libraries

| Resource | Type | Links | Why It Is Useful |
| --- | --- | --- | --- |
| OpenAI `skills` + `skill-installer` | skill infrastructure | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/openai/skills) | The cleanest install path for Codex-native reusable skills, including image and workflow skills relevant to visual-agent prototyping. |
| `awesome-gpt-image-2` | prompt and style skill library | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/freestylefly/awesome-gpt-image-2) | High-quality prompt-as-code and style library for agentic visual creation workflows. |
| `gpt_image_2_skill` | Codex skill | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/wuyoscar/gpt_image_2_skill) | Compact, practical skill for repeatable image generation and editing inside a coding-agent workflow. |

#### Install: `awesome-gpt-image-2` Skill

```bash
npx --yes skills@latest add freestylefly/awesome-gpt-image-2 \
  --skill gpt-image-2-style-library \
  --agent codex \
  --copy
```

#### Install: `gpt_image_2_skill` for Codex

```text
$skill-installer
Install this skill from GitHub:
https://github.com/wuyoscar/gpt_image_2_skill/tree/main/skills/gpt-image
```

[Back to top](#top)

### Perception, Parsing, and Grounding Tools

| Tool | Type | Links | Best For |
| --- | --- | --- | --- |
| OmniParser | GUI parser | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/microsoft/OmniParser) | Converting screenshots into interactable regions and semantics for vision-only GUI agents. |
| OmniMCP | OmniParser bridge | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/OpenAdaptAI/OmniMCP) | Wrapping visual parsing into a tool-friendly control surface for agent systems. |
| OpenAdapt Grounding | grounding tooling | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/OpenAdaptAI/openadapt-grounding) | Practical grounding and operator-facing automation utilities inside the OpenAdapt stack. |
| UI-Zoomer | zoom-in utility | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/UI-Zoomer) | Useful whenever small icons, dense ribbons, or high-resolution UIs break direct grounding. |
| ShowUI | VLA-style GUI model stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/showlab/ShowUI) | Useful reference implementation when you want a unified screenshot-to-action pipeline. |

[Back to top](#top)

### Agent Runtimes, Sandboxes, and Operator Stacks

| Stack | Type | Links | Best For |
| --- | --- | --- | --- |
| UI-TARS-desktop | native desktop agent stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/bytedance/UI-TARS-desktop) | End-to-end desktop operator workflows and native GUI-agent experimentation. |
| Agent-S | hierarchical operator framework | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/simular-ai/Agent-S) | Planning, memory, and experience reuse for computer-use agents. |
| OpenCUA | open foundation stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OpenCUA) | Open training and evaluation substrate for computer-use agents. |
| Cua | computer-use infrastructure | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/trycua/cua) | Open-source infrastructure, sandboxes, and SDKs for computer-use-agent development. |
| OpenAdapt | operator and desktop automation stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/OpenAdaptAI/OpenAdapt) | Desktop control, data capture, evaluation, and agent-building utilities in one ecosystem. |
| ScreenPipe | local screen-memory runtime | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/screenpipe/screenpipe) | Persistent visual memory and capture for long-running assistants and operator loops. |

[Back to top](#top)

### Harnesses, Eval Suites, and Benchmark Orchestration

| Resource | Type | Links | Best For |
| --- | --- | --- | --- |
| BrowserGym | benchmark framework | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/ServiceNow/BrowserGym) | Standardized browser-agent environments and task wrappers. |
| AgentLab | evaluation harness | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/ServiceNow/AgentLab) | Running, comparing, and analyzing browser-agent experiments on WebArena-style tasks. |
| ScreenSuite | GUI-agent benchmark suite | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/ryoungj/ScreenSuite) | Consolidated GUI-agent benchmarking across multiple perception and action tasks. |
| lmms-eval | multimodal eval toolkit | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EvolvingLMMs-Lab/lmms-eval) | Strong general-purpose evaluation toolkit with multimodal and agent-adjacent value. |
| VisualWebArena | benchmark environment | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/web-arena-x/visualwebarena) | Visually grounded browser-agent evaluation. |
| OSWorld | desktop benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OSWorld) | Flagship open benchmark for real computer-use agents across applications. |
| WindowsAgentArena | Windows benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/microsoft/WindowsAgentArena) | Scalable evaluation on Windows applications and workflows. |
| AndroidWorld | Android benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/google-research/android_world) | Dynamic Android environment with large task diversity. |
| EmbodiedBench | embodied-agent benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EmbodiedBench/EmbodiedBench) | Unified benchmark layer for embodied multimodal agents. |
| DoomArena | safety and stress benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/trycua/doom-arena) | Useful stress-testing environment for agent robustness and control. |

[Back to top](#top)

### Demonstration Capture and Data Tooling

| Resource | Type | Links | Why It Is Useful |
| --- | --- | --- | --- |
| OpenAdapt Desktop | data capture | [Project](https://github.com/OpenAdaptAI/openadapt-desktop) | Records and structures real computer-use traces for training, replay, and analysis. |
| OpenAdapt-ML | model training layer | [Project](https://github.com/OpenAdaptAI/openadapt-ml) | Turns captured interaction traces into trainable agent pipelines. |
| ShowUI-Aloha | screen-recording supervision | [Paper](https://arxiv.org/abs/2601.07181) [Code](https://github.com/showlab/ShowUI) | Human demonstration pipeline for GUI-agent training. |
| OpenCUA / AgentNet family | open agent data stack | [Project](https://github.com/xlang-ai/OpenCUA) | Useful umbrella for open datasets, models, and benchmark components. |
| GroundCUA / GroundNext | grounding data engine | [Paper](https://arxiv.org/abs/2511.07332) | Useful when desktop grounding quality is the bottleneck in a larger agent stack. |
| CUA-Suite | research suite | [Paper](https://arxiv.org/abs/2603.24440) | Useful when you need one consolidated suite for grounding, video, and UI evaluation. |
| Video2GUI | trajectory synthesis | [Paper](https://arxiv.org/abs/2605.14747) | Fresh 2026 pipeline for turning tutorial videos into large-scale pretraining trajectories. |
| ScreenPipe | continuous capture and memory | [Project](https://github.com/screenpipe/screenpipe) | Helpful for memory-heavy assistants and screen-native agents. |

[Back to top](#top)

### Embodied and Robotics Tooling

| Tool | Type | Links | Best For |
| --- | --- | --- | --- |
| OpenVLA | VLA model and training stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/openvla/openvla) | Open embodied-agent baseline with training and evaluation support. |
| LeRobot | robotics learning stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/huggingface/lerobot) | Practical robotics dataset, policy, and evaluation tooling with strong community adoption. |
| LIBERO | lifelong robot benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/Lifelong-Robot-Learning/LIBERO) | Continual and compositional robot manipulation evaluation. |
| LIBERO-plus | updated embodied benchmark | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/tylerlum/libero_plus) | Useful extension when evaluating broader VLA-style generalization. |
| RLBench | robot learning environment | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/stepjam/RLBench) | Widely used manipulation benchmark environment for embodied control research. |
| EmbodiedBench | multimodal embodied evaluation | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EmbodiedBench/EmbodiedBench) | Convenient benchmark layer for comparing embodied multimodal agents. |

[Back to top](#top)

## Benchmarks and Environments

| Area | Benchmark / Environment | Links | Why It Matters |
| --- | --- | --- | --- |
| Web | WebArena | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2307.13854) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/web-arena-x/webarena) | Foundational realistic web-agent benchmark. |
| Web | VisualWebArena | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.13649) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/web-arena-x/visualwebarena) | Adds screenshot-grounded perception to browser-agent evaluation. |
| Web | BrowserGym | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/ServiceNow/BrowserGym) | Reusable harness for browser-agent experimentation at scale. |
| Web | WorkArena | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2403.07718) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ServiceNow/WorkArena) | Enterprise workflow benchmark centered on knowledge-work tasks. |
| Web | WebArena-Verified | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/web-arena-x/webarena-verified) | Cleaner, more controlled evaluation variant for WebArena-style research. |
| Desktop | OSWorld | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2404.07972) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OSWorld) | Flagship open benchmark for real desktop computer use. |
| Desktop | UI-Vision | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.15661) | Fine-grained offline benchmark for desktop perception, layout grounding, and action prediction. |
| Desktop | OmniACT | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.17553) | Evaluates executable automation rather than only low-level action traces. |
| Desktop | WindowsAgentArena | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2409.08264) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/microsoft/WindowsAgentArena) | Scalable Windows evaluation environment. |
| Mobile | AndroidWorld | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2405.14573) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/google-research/android_world) | Dynamic Android benchmark with broad task diversity. |
| Mobile | MobileAgentBench | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2406.08184) | Efficient and practical benchmark for mobile GUI agents across open-source apps. |
| Mobile | SPA-Bench | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.15164) | Strong multilingual smartphone benchmark with plug-and-play integration. |
| Mobile | MemGUI-Bench | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.06075) | Cross-session and cross-temporal memory evaluation for GUI agents. |
| Mobile | DynamicGUIBench | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.25380) | Dynamic GUI environments rather than frozen UI snapshots. |
| Grounding | ScreenSpot-Pro | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.07981) | High-resolution professional-screen grounding benchmark. |
| Grounding | GUI-Perturbed | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14262) | Robustness diagnostics for perturbations and relational instructions. |
| Computer use | AssistantBench | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2407.15711) | Moves beyond short episodes toward realistic, time-consuming assistant tasks. |
| Computer use | VideoWebArena | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.19100) | Long-context video understanding inside web-agent workflows. |
| Computer use | CUA-Suite | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.24440) | Consolidated suite for modern computer-use-agent research. |
| Security | VPI-Bench | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.02456) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/boyugou/VPI-Bench) | Visual prompt-injection benchmark for GUI agents. |
| Safety | HazardArena | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.12447) | Semantic safety evaluation for VLA systems. |
| Embodied | EmbodiedBench | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EmbodiedBench/EmbodiedBench) | Unified embodied multimodal benchmark layer. |
| Embodied | LIBERO | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/Lifelong-Robot-Learning/LIBERO) | Continual manipulation benchmark widely used in robot learning. |
| Embodied | RLBench | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/stepjam/RLBench) | Strong manipulation environment for embodied control evaluation. |

[Back to top](#top)

## Official Docs and Engineering Notes

| Resource | Links | Why Read It |
| --- | --- | --- |
| OpenAI: Computer-Using Agent | [![Docs](https://img.shields.io/badge/Docs-Reference-2563eb?logo=readthedocs&logoColor=white)](https://openai.com/index/computer-using-agent/) | Product and research framing for modern computer-use agents. |
| OpenAI API: Computer Use Guide | [![Docs](https://img.shields.io/badge/Docs-Reference-2563eb?logo=readthedocs&logoColor=white)](https://platform.openai.com/docs/guides/tools-computer-use) | Developer-facing usage guide for building computer-use workflows. |
| Anthropic: Developing a Computer Use Model | [![Docs](https://img.shields.io/badge/Docs-Reference-2563eb?logo=readthedocs&logoColor=white)](https://www.anthropic.com/news/developing-computer-use) | One of the best public engineering writeups on GUI-agent development. |
| Anthropic: Introducing computer use | [![Docs](https://img.shields.io/badge/Docs-Reference-2563eb?logo=readthedocs&logoColor=white)](https://www.anthropic.com/news/3-5-models-and-computer-use) | Concise system framing plus deployment context. |
| Google DeepMind: Gemini Robotics brings AI into the physical world | [![Docs](https://img.shields.io/badge/Docs-Reference-2563eb?logo=readthedocs&logoColor=white)](https://deepmind.google/blog/gemini-robotics-brings-ai-into-the-physical-world/) | Frontier industry view on embodied visual agents. |
| Google DeepMind: Gemini Robotics On-Device | [![Docs](https://img.shields.io/badge/Docs-Reference-2563eb?logo=readthedocs&logoColor=white)](https://deepmind.google/discover/blog/gemini-robotics-on-device-brings-ai-to-local-robotic-devices/) | Practical view on low-latency on-device VLA deployment. |

[Back to top](#top)

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
10. [HazardArena](https://arxiv.org/abs/2604.09985)

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
2. [A Unified Agentic Framework for Evaluating Conditional Image Generation](https://arxiv.org/abs/2504.07046)
3. [Mind-Brush](https://arxiv.org/abs/2602.01756)
4. [VisionCreator](https://arxiv.org/abs/2603.02681)
5. [Visual Generation in the New Era](https://arxiv.org/abs/2604.28185)

[Back to top](#top)

## Build Paths by Workflow

| Workflow | Recommended Stack |
| --- | --- |
| Desktop and browser computer-use prototyping | `OmniParser` + `UI-TARS-desktop` + `Agent-S` + `BrowserGym` + `OSWorld` |
| Long-horizon GUI-agent research | `OpenCUA` + `Cua` + `UI-Copilot` + `OS-Symphony` + `CUA-Suite` |
| Mobile GUI agents | `Ferret-UI` + `AndroidWorld` + `MemGUI-Bench` + `DynamicGUIBench` |
| Visual-grounding and parsing research | `ScreenAI` + `SeeClick` + `UGround` + `GUI-Eyes` + `UI-Zoomer` |
| Agentic visual creation workflows | `awesome-gpt-image-2` + `gpt_image_2_skill` + `Mind-Brush` + `VisionCreator` |
| Data capture and imitation pipelines | `OpenAdapt Desktop` + `OpenAdapt-ML` + `ShowUI-Aloha` + `ScreenPipe` |
| Embodied VLA experimentation | `OpenVLA` + `LeRobot` + `LIBERO` + `RLBench` + `EmbodiedBench` |

[Back to top](#top)

## Related Awesome Repositories

| Repository | Links | Notes |
| --- | --- | --- |
| Awesome-GUI-Agents | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/Awesome-GUI-Agents) | Strong companion list focused on GUI grounding, long-horizon automation, and benchmarks. |
| GUI-Agents-Paper-List | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/OSU-NLP-Group/GUI-Agents-Paper-List) | Systematic, community-maintained paper index for GUI agents. |
| awesome-ui-agents | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/opendilab/awesome-ui-agents) | Useful neighboring list if you want extra depth on UI agents specifically. |
| acu | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/trycua/acu) | Good companion collection around computer-use-agent infrastructure and resources. |
| Awesome Multimodal Modeling | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/OpenEnvision/Awesome-Multimodal-Modeling) | Broader multimodal map beyond the stricter visual-agent boundary used here. |
| Evolving Visual Generation | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EvolvingLMMs-Lab/Evolving-Visual-Generation) | Useful adjacent list for the visual-creation side of agentic systems. |

[Back to top](#top)

## Curation Principles

- Prefer works that define a new capability, benchmark, training recipe, or systems bottleneck for agentic visual systems.
- Prefer official artifacts whenever possible: paper, code, benchmark, toolkit, or docs.
- Exclude broad multimodal or image-generation models unless they are explicitly agentic, tool-using, or benchmark-central.
- Separate `perception`, `computer use`, `embodied action`, `agentic creation`, and `evaluation` rather than collapsing them into one bucket.
- Keep builder-facing resources first-class: skills, runtimes, sandboxes, harnesses, parsers, and data pipelines matter as much as papers.
- Add recent work only when it improves the map rather than inflating it.

[Back to top](#top)

## Contributing

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

If you maintain a relevant project, benchmark, or dataset, a concise and well-scoped PR is the fastest way to improve the map. If you find the list useful, giving the repository a star is also greatly appreciated.

[Back to top](#top)

## Acknowledgments

This repository was shaped by the structure and coverage quality of several strong public resources, especially:

- [OpenEnvision/Awesome-Multimodal-Modeling](https://github.com/OpenEnvision/Awesome-Multimodal-Modeling)
- [ZJU-REAL/Awesome-GUI-Agents](https://github.com/ZJU-REAL/Awesome-GUI-Agents)
- [OSU-NLP-Group/GUI-Agents-Paper-List](https://github.com/OSU-NLP-Group/GUI-Agents-Paper-List)
- [opendilab/awesome-ui-agents](https://github.com/opendilab/awesome-ui-agents)
- [EvolvingLMMs-Lab/Evolving-Visual-Generation](https://github.com/EvolvingLMMs-Lab/Evolving-Visual-Generation)
- [freestylefly/awesome-gpt-image-2](https://github.com/freestylefly/awesome-gpt-image-2)
- [wuyoscar/gpt_image_2_skill](https://github.com/wuyoscar/gpt_image_2_skill)

The goal here is to push beyond a flat link dump and toward a research-and-building index for serious visual-agent work.

[Back to top](#top)
