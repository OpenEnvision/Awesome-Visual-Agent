&lt;p align="center"&gt;
  &lt;h1 align="center"&gt;Awesome Visual Agent&lt;/h1&gt;
  &lt;p align="center"&gt;
    &lt;b&gt;A curated research index of visual agents: perception, grounding, agentic generation, GUI automation, and embodied vision-language-action (2023–2026).&lt;/b&gt;
  &lt;/p&gt;
  &lt;p align="center"&gt;
    &lt;img src="https://img.shields.io/badge/curation-research--driven-111111?style=flat-square" alt="curation"&gt;
    &lt;img src="https://img.shields.io/badge/scope-visual%20agents-0f766e?style=flat-square" alt="scope"&gt;
    &lt;img src="https://img.shields.io/badge/coverage-2023--2026-c2410c?style=flat-square" alt="years"&gt;
    &lt;img src="https://img.shields.io/badge/last%20updated-2026--05--15-1d4ed8?style=flat-square" alt="updated"&gt;
    &lt;img src="https://img.shields.io/badge/PRs-welcome-green?style=flat-square" alt="prs"&gt;
  &lt;/p&gt;
&lt;/p&gt;

&gt; **Scope & Boundary.** This list is a professional research-and-building index, not a flat bookmark dump. We emphasize **taxonomy, official artifacts, open tooling, evaluation environments, and reading paths** around visual-agent work. Generic vision backbones, unified multimodal foundation models, and pure generation/training recipes are intentionally excluded unless they are directly agentic—i.e., they close the loop between **visual perception, reasoning, memory, tool use, generation, and action**.

---

## Table of Contents

- [Why This Repo](#why-this-repo)
- [2026 Radar](#2026-radar)
- [Taxonomy at a Glance](#taxonomy-at-a-glance)
- [Link Badge Legend](#link-badge-legend)
- [Research Map](#research-map)
  - [1. Surveys, Roadmaps, and Big-Picture Guides](#1-surveys-roadmaps-and-big-picture-guides)
  - [2. Visual Understanding, Grounding, and Screen Perception](#2-visual-understanding-grounding-and-screen-perception)
  - [3. Agentic Visual Generation](#3-agentic-visual-generation)
  - [4. GUI and Computer-Use Agents](#4-gui-and-computer-use-agents)
  - [5. Embodied Vision-Language-Action Agents](#5-embodied-vision-language-action-agents)
  - [6. Evaluation, Benchmarks, and Safety](#6-evaluation-benchmarks-and-safety)
- [Technology View](#technology-view)
- [Benchmarks and Environments](#benchmarks-and-environments)
- [Skills and Tooling](#skills-and-tooling)
  - [1. Agent Skills & Reusable Procedures](#1-agent-skills--reusable-procedures)
  - [2. Agent Harnesses & Orchestration Frameworks](#2-agent-harnesses--orchestration-frameworks)
  - [3. MCP Servers & Visual-Agent Connectivity](#3-mcp-servers--visual-agent-connectivity)
  - [4. Core Reference Repositories](#4-core-reference-repositories)
  - [5. Open-Source Toolchains](#5-open-source-toolchains)
  - [6. Tool Selection by Workflow](#6-tool-selection-by-workflow)
- [Blogs and Deep Dives](#blogs-and-deep-dives)
- [Suggested Reading Paths](#suggested-reading-paths)
- [Related Awesome Repositories](#related-awesome-repositories)
- [Curation Principles](#curation-principles)
- [Contributing](#contributing)
- [Acknowledgments](#acknowledgments)

---

## Why This Repo

Visual agents are no longer merely "VLMs that can see." The field is converging toward systems that:

- **Ground** language in pixels, screens, layouts, objects, and documents;
- **Reason** over long horizons with memory, reflection, and recovery;
- **Call tools** and operate external environments rather than only answering questions;
- **Generate** images, edits, layouts, and multimodal artifacts through planning and verification loops;
- **Act** in digital systems (GUI/web/desktop) and physical robotic environments.

We define a **visual agent** as a system that closes the loop between **visual perception → reasoning → memory → tool use → generation → action**.

To keep the boundary clean, this list prioritizes:
- Visual **understanding** agents that serve action (screen parsing, grounding, navigation);
- Visual **generation** systems that are **agentic** (planning, tool use, verification, editing workflows);
- **GUI / computer-use** agents and **embodied VLA** agents, plus their benchmarks;
- Tools and evaluations that materially help build, measure, or deploy the above.

This curation is cross-checked against major community lists, especially [Awesome-GUI-Agents](https://github.com/ZJU-REAL/Awesome-GUI-Agents), [awesome-ui-agents](https://github.com/opendilab/awesome-ui-agents), and [GUI-Agents-Paper-List](https://github.com/OSU-NLP-Group/GUI-Agents-Paper-List), with the current pass updated on **2026-05-15**.

---

## 2026 Radar

| Work | Date | Links | Why It Matters |
|------|------|-------|--------------|
| **Qwen-Image-2.0** Technical Report | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.10730) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/QwenLM/Qwen-Image) | Major upgrade for dense text rendering, infographics, editing, and 2K generation with explicit planning loops. |
| **InterLV-Search** | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.07510) | Benchmarks interleaved language-vision search with visual evidence reused across multiple search decisions. |
| **MMSkills** | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.13527) | Multimodal skill library for general visual agents across GUI, desktop, and game tasks. |
| **VeriGUI** (ACL 2026) | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.05477) | TVAE framework with robust SFT and GRPO for verification-driven GUI automation and self-correction. |
| **UI-Zoomer** | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14113) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/UI-Zoomer) | Training-free zoom-in method for small icons and dense GUI grounding. |
| **UI-Copilot** | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.13822) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/UI-Copilot) | Long-horizon GUI automation with retrieval and calculator tools. |
| **OmniActor** (ICLR 2026) | 2026-09 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.XXXXX) | Generalist agent for both GUI-based 2D and embodied 3D worlds via layer-heterogeneous MoE and unified action space. |
| **Vision-Language-Action Safety** | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.23775) | Timely survey on safety, attacks, evaluation, and deployment of embodied VLA systems. |
| **VLA Datasets & Data Engines** | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.23001) | Data-centric view: VLA progress is increasingly limited by infrastructure, not only architecture. |
| **World-Value-Action Model** | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14732) | Pushes VLA systems toward latent-space planning and implicit future evaluation. |
| **Visual Generation in the New Era** | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.28185) | Roadmap from atomic mapping to agentic world modeling in visual generation. |
| **LaRA-VLA** (ICML 2026) | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.01166) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/LoveJu1y/LaRA-VLA) | Latent reasoning and prediction for VLAs. |
| **LLaVA-VLA** (ICRA 2026) | 2026-02 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.22663) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OpenHelix-Team/LLaVA-VLA) | Simple yet powerful VLA baseline with comprehensive benchmark. |
| **MAGNET** | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.19199) | Adaptive GUI agents with memory-driven knowledge evolution. |
| **RoboClaw** | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.11558) | Agentic framework for scalable long-horizon robotic tasks. |
| **FAEA** | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.20334) | Demonstration-free robotic control via frontier LLM agents (Claude Agent SDK). |
| **GameWorld** | 2026-04 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.07429) | Standardized and verifiable evaluation of multimodal game agents. |
| **GenAgent** | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.18543) | Scaling text-to-image generation via agentic multimodal reasoning. |
| **GEMS** | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.28088) | Agent-native multimodal generation with memory and skills. |
| **VisionCreator** | 2026-03 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.02681) | Native visual-generation agentic model that unifies understanding, planning, and creation. |
| **DuoGen** | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.00508) | General-purpose interleaved image-text generation for agentic trajectories. |
| **ShowUI-Aloha** | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.07181) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/showlab/ShowUI) | Human-demonstration pipeline for teaching GUI agents from screen recordings. |
| **OS-Symphony** | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.07779) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OS-Copilot/OS-Symphony) | Holistic framework for memory, reflection, and retrieval-aware computer use. |
| **AgentProg** | 2026-05 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.10371) | Program-guided context management for long-horizon GUI agents. |
| **Evocua** | 2026-01 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.15876) | Evolving computer-use agents via learning from scalable synthetic experience. |

---

## Taxonomy at a Glance

| Track | Core Question | Typical Outputs | Representative Starting Points |
|-------|-------------|---------------|------------------------------|
| **Visual Understanding Agents** | Can the agent perceive, localize, parse, and reason over visual inputs to enable action? | boxes, structured extraction, grounded summaries, parse trees | ScreenAI, CogAgent, SeeClick, OmniParser |
| **Agentic Visual Generation** | Can the agent plan, verify, and render images/edits/layouts through reasoning loops? | images, edits, posters, diagrams, slides | Qwen-Image-2.0, VisionCreator, GenAgent, GEMS |
| **GUI / Computer-Use Agents** | Can the agent operate websites, desktops, and mobile apps from screenshots and action history? | clicks, typing, navigation, task trajectories, code | SeeClick, UI-TARS, Agent S2, Cradle, OSWorld |
| **Embodied VLA Agents** | Can the agent turn visual observations and language into physical actions with planning/memory? | robot trajectories, manipulation plans, embodied traces | RT-2, OpenVLA, π₀, RoboClaw, World-Value-Action |
| **Evaluation / Tooling** | How do we benchmark and operationalize agentic perception, action, and safety? | environments, leaderboards, eval stacks, skills | VisualWebArena, OSWorld, AndroidWorld, GameWorld |

---

## Link Badge Legend

- Paper: [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/)
- Code: [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/)
- Project / living list / toolkit: [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/)

---

## Research Map

### 1. Surveys, Roadmaps, and Big-Picture Guides

| Work | Year | Links | Notes |
|------|------|-------|-------|
| Visual Generation in the New Era: An Evolution from Atomic Mapping to Agentic World Modeling | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.28185) | Cleanest recent roadmap for modern visual generation and agentic world modeling. |
| A Survey on (M)LLM-Based GUI Agents | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.13865) | Strong entry point for GUI-agent architectures, planning, grounding, and evaluation. |
| GUI Agents: A Survey | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2412.13501) | Broad overview of task settings, model classes, and protocols for GUI agents. |
| Towards Trustworthy GUI Agents: A Survey | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.23434) | Robustness, reliability, and deployment risk for GUI agents. |
| Securing Computer-Use Agents: A Unified Architecture–Lifecycle Framework | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.07110) | Security and reliability across the full lifecycle of computer-use agents. |
| Survey of Vision-Language-Action Models for Embodied Manipulation | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.15201) | Practical survey of VLA structures, datasets, post-training, and evaluation. |
| A Survey on Vision-Language-Action Models: An Action Tokenization Perspective | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.01925) | Why VLA systems differ in how they express action. |
| Vision-Language-Action in Robotics: A Survey of Datasets, Benchmarks, and Data Engines | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.23001) | Data-centric view: VLA progress is increasingly limited by infrastructure, not only architecture. |
| Adaptation of Agentic AI: A Survey of Post-Training, Memory, and Skills | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.16301) | Systematic view of memory, skill discovery, and continual adaptation in agents. |
| A Survey of WebAgents | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.23350) | Web automation agents with foundation models. |

---

### 2. Visual Understanding, Grounding, and Screen Perception

| Work | Year | Links | Notes |
|------|------|-------|-------|
| ScreenAI: A Vision-Language Model for UI and Infographics Understanding | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.04615) | Key work for UI, infographic, and visually structured understanding as agent inputs. |
| CogAgent: A Visual Language Model for GUI Agents | 2023 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2312.08914) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/THUDM/CogAgent) | Early strong open model for screenshot-driven GUI understanding and navigation. |
| SeeClick: Harnessing GUI Grounding for Advanced Visual GUI Agents | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.10935) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/njucckevin/SeeClick) | Foundational if grounding is the bottleneck you care about most. |
| UGround: Universal Visual Grounding for GUI Agents | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.05243) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OSU-NLP-Group/UGround) | Argues for fully visual human-like GUI perception without textual trees. |
| OS-ATLAS: A Foundation Action Model for Generalist GUI Agents | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.23218) | Strong action-grounding model and large cross-platform GUI corpus. |
| UI-E2I-Synth: Advancing GUI Grounding with Large-Scale Instruction Synthesis | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.11257) | Synthetic-data direction for scaling GUI grounding quality and instruction diversity. |
| Ferret-UI: Grounded Mobile UI Understanding with Multimodal LLMs | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2404.05719) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/apple/ml-ferret) | Mobile-UI grounding with explicit region-aware training for agent perception. |
| ShowUI: One Vision-Language-Action Model for GUI Visual Agent | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2411.17465) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/showlab/ShowUI) | Unified VLA-style GUI agent with screenshot-conditioned action modeling. |
| OmniParser for Pure Vision Based GUI Agent | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2408.00203) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/microsoft/OmniParser) | Practical tool for parsing screenshots into reliable interactable regions for agents. |
| Aguvis: Unified Pure Vision Agents for Autonomous GUI Interaction | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2412.04454) | Important pure-vision GUI agent without dependence on textual trees. |
| InfiGUIAgent: A Multimodal Generalist GUI Agent with Native Reasoning and Reflection | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2501.04575) | Expectation-reflection and explicit multi-step reasoning for GUI automation. |
| UI-Zoomer: Uncertainty-Driven Adaptive Zoom-In for GUI Grounding | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14113) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/UI-Zoomer) | Training-free zoom-in framework for small targets and dense layouts. |
| Test-Time Reinforcement Learning for GUI Grounding via Region Consistency | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.05615) | Test-time RL optimizing GUI grounding through region-consistency rewards. |
| ScreenSpot-Pro: GUI Grounding for Professional High-Resolution Computer Use | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.07981) | High-resolution professional-screen grounding benchmark and method. |
| Enhancing GUI Grounding via Fast and Slow Systems | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.06470) | Dual-system cognitive-inspired grounding for GUI agents. |

---

### 3. Agentic Visual Generation

&gt; **Boundary note.** This section excludes generic text-to-image models and pure training recipes. It includes only systems that plan, verify, search, or otherwise reason to produce or edit visual content.

| Work | Year | Links | Notes |
|------|------|-------|-------|
| Qwen-Image Technical Report | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.02324) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/QwenLM/Qwen-Image) | Open image generation and editing system with strong text rendering and agentic editing loops. |
| Qwen-Image-2.0 Technical Report | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.10730) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/QwenLM/Qwen-Image) | Major upgrade for dense text rendering, infographics, editing, and 2K generation with planning. |
| Mind-Brush: Integrating Agentic Cognitive Search and Reasoning into Image Generation | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.01756) | Image generation as a retrieval-and-reasoning workflow rather than static decoding. |
| VisionCreator: A Native Visual-Generation Agentic Model | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.02681) | End-to-end agentic visual creation with understanding-thinking-planning-creation loop. |
| GenAgent: Scaling Text-to-Image Generation via Agentic Multimodal Reasoning | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.18543) | Agentic scaling of T2I via multimodal reasoning chains and subgoal decomposition. |
| GEMS: Agent-Native Multimodal Generation with Memory and Skills | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.28088) | Memory-augmented and skill-conditioned multimodal generation agent. |
| SCOPE: Structured Decomposition and Conditional Skill Orchestration for Complex Image Generation | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.08043) | Skill-orchestrated decomposition for complex image generation via agentic planning. |
| ImAgent: Unified Multimodal Agent for Test-Time Scalable Image Generation | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.11483) | Training-free unified agent integrating reasoning, generation, and self-evaluation. |
| GenSearcher: Reinforcing Agentic Search for Image Generation | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.28767) | Agentic search augmented image generation via RL. |
| Unify-Agent: Unified Multimodal Agent for World-Grounded Image Synthesis | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.29620) | World-grounded image synthesis via unified multimodal agent. |
| A Unified Agentic Framework for Evaluating Conditional Image Generation | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.07046) | Agentic evaluation for conditional image generation rather than only static metrics. |
| Visual Generation in the New Era | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.28185) | Best recent roadmap for understanding visual generation as an increasingly agentic process. |
| Evolving Visual Generation | living repo | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EvolvingLMMs-Lab/Evolving-Visual-Generation) | Strongest continuously updated hub for visual generation papers and trends. |

---

### 4. GUI and Computer-Use Agents

| Work | Year | Links | Notes |
|------|------|-------|-------|
| AppAgent: Multimodal Agents as Smartphone Users | 2023 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2312.13771) | Foundational smartphone-use agent with visual perception. |
| AutoWebGLM: A Large Language Model-based Web Navigating Agent | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2404.03648) | Bootstrap and RL for web navigation with tool use. |
| WebVoyager: Building an End-to-End Web Agent with Large Multimodal Models | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.13919) | Early strong end-to-end web agent with visual grounding. |
| Cradle: Empowering Foundation Agents Towards General Computer Control | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2403.03186) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/BAAI-Agents/Cradle) | Generalist computer control via foundation agents; covers games, OS, and professional software. |
| OS-Copilot: Towards Generalist Computer Agents with Self-Improvement | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.07456) | Self-improving generalist computer agent with automatic tool creation. |
| AutoGLM: Autonomous Foundation Agents for GUIs | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2411.00820) | Autonomous GUI agent with intermediate thought graphs and online RL. |
| DigiRL: Training In-the-Wild Device-Control Agents with Autonomous RL | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2406.11896) | Autonomous RL pipeline for training device-control agents without human demonstrations. |
| Digi-Q: Learning Q-Value Functions for Training Device-Control Agents | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.XXXXX) | Q-learning framework for sample-efficient training of GUI automation agents. |
| VisualWebArena | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.13649) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/web-arena-x/visualwebarena) | Central benchmark for visually grounded browser agents. |
| OmniACT: A Dataset and Benchmark for Enabling Multimodal Generalist Autonomous Agents for Desktop and Web | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.17553) | Evaluates executable automation rather than only low-level control traces. |
| WorkArena | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2403.07718) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ServiceNow/WorkArena) | Practical knowledge-work benchmark around enterprise workflows. |
| OSWorld | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2404.07972) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OSWorld) | Flagship open benchmark for real computer-use agents. |
| Windows Agent Arena | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2409.08264) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/microsoft/WindowsAgentArena) | Scalable Windows benchmark with cloud-scale evaluation support. |
| AndroidWorld | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2405.14573) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/google-research/android_world) | Dynamic Android environment with millions of task variations. |
| Mobile-Agent / V2 / V3 | 2024–2025 | [![arXiv](https://img.shields.io/badge/arXiv-V1-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.16158) [![arXiv](https://img.shields.io/badge/arXiv-V2-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.16158) [![arXiv](https://img.shields.io/badge/arXiv-V3-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.15144) | Progressive mobile-device agent series with visual perception and multi-agent collaboration. |
| UFO: A UI-Focused Agent for Windows OS Interaction | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.07939) | UI-focused Windows agent leveraging OS-level accessibility APIs. |
| ScreenAgent: A Vision Language Model-Driven Computer Control Agent | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.07945) | VLM-driven direct computer control with screen understanding. |
| ScaleCUA: Scaling Open-Source Computer Use Agents with Cross-Platform Data | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.15221) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OpenGVLab/ScaleCUA) | Cross-platform data scaling for open computer-use agents. |
| Advancing Mobile GUI Agents: A Verifier-Driven Approach to Practical Deployment | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.15937) | V-Droid: verifier-driven mobile GUI agent emphasizing latency and deployment. |
| UI-TARS: Pioneering Automated GUI Interaction with Native Agents | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2501.12326) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/bytedance/UI-TARS) | End-to-end native GUI agent; clear signal of where the field is heading. |
| Agent S | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.08164) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/simular-ai/Agent-S) | Hierarchical planning and experience reuse for computer use. |
| Agent S2: A Compositional Generalist-Specialist Framework | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.00906) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/simular-ai/Agent-S) | Compositional upgrade with grounding specialists and proactive planning. |
| AssistantBench: Can Web Agents Solve Realistic and Time-Consuming Tasks? | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2407.15711) | Moving beyond short benchmark episodes toward realistic long-horizon web assistance. |
| ShowUI-Aloha: Human-Taught GUI Agent | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.07181) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/showlab/ShowUI) | Pipeline for turning raw human screen recordings into structured GUI-agent supervision. |
| UI-Copilot: Advancing Long-Horizon GUI Automation via Tool-Integrated Policy Optimization | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.13822) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/UI-Copilot) | Long-horizon GUI tasks with explicit retrieval and calculator assistance. |
| ActionEngine: From Reactive to Programmatic GUI Agents via State Machine Memory | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.20502) | Memory-and-program-synthesis direction moving GUI agents from reactive loops to executable plans. |
| OS-Symphony: A Holistic Framework for Robust and Generalist Computer-Using Agent | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.07779) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OS-Copilot/OS-Symphony) | Memory, reflection, and visual-aware tutorial retrieval. |
| MAGNET: Towards Adaptive GUI Agents with Memory-Driven Knowledge Evolution | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.19199) | Adaptive GUI agent with evolving procedural memory. |
| AgentProg: Empowering Long-Horizon GUI Agents with Program-Guided Context Management | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.10371) | Program-guided context compression for long-horizon GUI tasks. |
| Evocua: Evolving Computer Use Agents via Learning from Scalable Synthetic Experience | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.15876) | Synthetic experience evolution for computer-use agents. |
| SEA: Self-Evolution Agent with Step-wise Reward for Computer Use | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.04037) | Step-wise reward modeling for self-evolving computer-use agents. |
| CoAct-1: Computer-Using Agents with Coding as Actions | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.03923) | Using executable code as the action space for computer-use agents. |
| SkillDroid: Compile Once, Reuse Forever | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14872) | Hierarchical skill compilation and reuse for Android agents. |
| Mirage-1: Augmenting and Updating GUI Agent with Hierarchical Multimodal Skills | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.10387) | Skill augmentation and updating for GUI agents. |
| AgentStore: Scalable Integration of Heterogeneous Agents | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.15845) | Scalable integration of heterogeneous agents as a specialized generalist assistant. |
| GTAL: GUI Test-Time Scaling Agent | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.05791) | Test-time scaling for GUI agents via search and verification. |
| UI-R1 / GUI-R1: Enhancing Action Prediction of GUI Agents by Reinforcement Learning | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-UI--R1-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.21620) [![arXiv](https://img.shields.io/badge/arXiv-GUI--R1-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.10458) | R1-style RL for GUI action prediction. |
| VeriGUI: Robust GUI Automation via Action-Effect Verification and Self-Correction (ACL 2026) | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.05477) | TVAE framework with robust SFT and asymmetric verification rewards for self-correction. |
| OmniActor: A Generalist GUI and Embodied Agent for 2D&3D Worlds (ICLR 2026) | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.XXXXX) | Single agent acting in both GUI 2D and embodied 3D via unified action spaces. |
| SWE-agent: Agent-Computer Interfaces Enable Automated Software Engineering | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2405.15793) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/princeton-nlp/SWE-agent) | Agent-computer interfaces for code-based environment control; relevant to computer-use agent design. |
| NNetNav: Unsupervised Learning of Browser Agents Through Environment Interaction in the Wild | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.02907) | Unsupervised browser agent learning from live web interaction. |
| VideoWebArena | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.19100) | Long-context video understanding inside web-agent workflows. |

---

### 5. Embodied Vision-Language-Action Agents

&gt; **Boundary note.** This section excludes pure model-architecture papers, efficiency-only work, and quantization recipes. It retains systems with explicit planning, memory, reasoning, world models, long-horizon decomposition, or safety/evaluation contributions.

| Work | Year | Links | Notes |
|------|------|-------|-------|
| RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control | 2023 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2307.15818) | Canonical VLA paper that transferred web knowledge into robot action. |
| OpenVLA: An Open-Source Vision-Language-Action Model | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2406.09246) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/openvla/openvla) | Central open baseline for robot-facing VLA work. |
| π₀ / π₀.5: Vision-Language-Action Flow Model for General Robot Control | 2024–2025 | [![arXiv](https://img.shields.io/badge/arXiv-π0-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.24164) [![arXiv](https://img.shields.io/badge/arXiv-π0.5-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.16054) | Flow-based VLA from Physical Intelligence with strong open-world generalization. |
| Interleave-VLA | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.02152) | Extends VLA systems to interleaved image-text instructions. |
| ChatVLA-2 | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.21906) | Preserving open-world reasoning in embodied VLA systems. |
| VLA² | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.14902) | Agentic external modules for unseen concept manipulation. |
| StemVLA | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.23721) | Future 3D geometry and 4D historical representation for action prediction. |
| World-Value-Action Model | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14732) | Long-horizon latent planning under physical constraints. |
| LLaVA-VLA: A Simple Yet Powerful Vision-Language-Action Model (ICRA 2026) | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.22663) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OpenHelix-Team/LLaVA-VLA) | Comprehensive benchmark and improved baseline. |
| LaRA-VLA: Latent Reasoning and Prediction for Vision-Language-Action Models (ICML 2026) | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.01166) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/LoveJu1y/LaRA-VLA) | Latent thinking and prediction for VLAs. |
| DualVLA: Building a Generalizable Embodied Agent via Partial Decoupling of Reasoning and Action | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.22134) | Decouples reasoning and action for better generalization. |
| DexVLA: Vision-Language Model with Plug-in Diffusion Expert for General Robot Control | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.05855) | Plug-in diffusion expert for robot control with agentic action generation. |
| MemoryVLA: Perceptual-Cognitive Memory in VLAs for Robotic Manipulation | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.19236) | Perceptual-cognitive memory for manipulation agents. |
| Motus: A Unified Latent Action World Model | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.13030) | Unified latent action world model for planning and future evaluation. |
| RoboClaw: An Agentic Framework for Scalable Long-Horizon Robotic Tasks | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.11558) | Scalable agentic framework for long-horizon robotics. |
| FAEA: Demonstration-Free Robotic Control via LLM Agents | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.20334) | Frontier LLM agents (Claude SDK) for embodied manipulation without demonstrations. |
| Long-VLA: Unleashing Long-Horizon Capability of Vision Language Action Model | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.19958) | Long-horizon VLA for robot manipulation. |
| LoHoVLA: A Unified Vision-Language-Action Model for Long-Horizon Embodied Tasks | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.00411) | Unified VLA for long-horizon embodied tasks. |
| LiLo-VLA: Compositional Long-Horizon Manipulation via Linked Object-Centric Policies | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.21531) | Compositional manipulation via linked object-centric policies. |
| AtomVLA: Scalable Post-Training for Robotic Manipulation via Predictive Latent World Models | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.08519) | Predictive latent world models for scalable VLA post-training. |
| AtomicVLA: Unlocking the Potential of Atomic Skill Learning in Robots | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.07648) | Atomic skill learning for compositional robot agents. |
| PALM: Progress-Aware Policy Learning via Affordance Reasoning for Long-Horizon Robotic Manipulation | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.07060) | Progress-aware policy learning with affordance reasoning. |
| Agentic Robot: A Brain-Inspired Framework for Vision-Language-Action Models in Embodied Agents | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.23450) | Brain-inspired agentic framework for VLA embodied agents. |
| Hi Robot: Open-Ended Instruction Following with Hierarchical Vision-Language-Action Models | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.19417) | Hierarchical VLA for open-ended instruction following. |
| RoboReward: General-Purpose Vision-Language Reward Models for Robotics | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.00675) | General-purpose VL reward models for robotics agents. |
| HapticVLA: Vision-Language-Action Models with Tactile Sensing for Contact-Rich Manipulation | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.15257) | Tactile-enhanced VLA for contact-rich manipulation agents. |

---

### 6. Evaluation, Benchmarks, and Safety

| Work | Year | Links | Notes |
|------|------|-------|-------|
| InterLV-Search | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.07510) | Agentic search with repeatedly reused visual evidence. |
| Agent-X: Evaluating Deep Multimodal Reasoning in Vision-Centric Agentic Tasks | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.24876) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/mbzuai-oryx/Agent-X) | Step-level reasoning quality instead of only final success. |
| GameWorld | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.07429) | Standardized, verifiable evaluation of multimodal game agents. |
| MMSkills | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.13527) | Multimodal skill evaluation for general visual agents. |
| AgentVista | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.12056) | Ultra-challenging comprehensive benchmark combining tool use and complex search. |
| PSPA-Bench | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.29318) | Personalized benchmark for smartphone GUI agents. |
| GUI-360° | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.04307) | Comprehensive dataset and benchmark for computer-using agents. |
| GUI-Perturbed | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14262) | Brittleness in GUI grounding under perturbations and relational instructions. |
| MemGUI-Bench | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.06075) | Cross-session and cross-temporal memory in mobile GUI agents. |
| RiOSWorld | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.00618) | Risk and safety benchmarking for multimodal computer-use agents. |
| MobileWorld | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.16196) | Long-horizon and cross-app mobile workflows. |
| AndroidLab | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.14228) | Systematic benchmark for mobile agents with reproducible evaluation. |
| UINavBench: A Framework for Comprehensive Evaluation of Interactive Digital Agents | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.XXXXX) | ICCV 2025 benchmark for interactive digital agents across GUI and web. |
| AgentRewardBench: Evaluating Automatic Evaluations of Web Agent Trajectories | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.08942) | Automatic reward modeling and evaluation for web agent trajectories. |
| VLABench | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2412.18194) | Large-scale benchmark for language-conditioned robotics manipulation with long-horizon reasoning. |
| LIBERO-plus: In-Depth Robustness Analysis of Vision-Language-Action Models | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.13626) | Robustness evaluation of VLAs under distribution shift. |
| RoboTwin: Dual-Arm Robot Benchmark with Generative Digital Twins | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.13059) | Generative digital twins for dual-arm robot manipulation benchmarks. |
| Terminal-Bench | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.11868) | Hard, realistic tasks in command-line interfaces for agents. |
| Claw-Eval / ClawsBench | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Claw--Eval-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.06132) [![arXiv](https://img.shields.io/badge/arXiv-ClawsBench-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.05172) | Trustworthy evaluation and capability-safety assessment of autonomous agents. |
| MCP-Bench / MCPMark | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-MCP--Bench-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.20453) [![arXiv](https://img.shields.io/badge/arXiv-MCPMark-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.24002) | Benchmarking tool-using LLM agents via MCP servers. |
| When Vision Overrides Language: Evaluating and Mitigating Counterfactual Failures in VLAs | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.17659) | Safety analysis of counterfactual reasoning failures in embodied VLAs. |
| Vision-Language-Action Safety | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.23775) | Survey on safety, attacks, evaluation, and deployment of embodied VLA systems. |

---

## Technology View

| Technical Theme | Why It Matters | Representative Works |
|-----------------|----------------|----------------------|
| **Grounding and screen parsing** | Agents fail if they cannot point to the right region, button, or object. | SeeClick, UGround, OmniParser, UI-Zoomer, ScreenSpot-Pro |
| **Long-horizon planning** | Real tasks need subgoals, recovery, and temporal abstraction. | Agent S, Agent S2, UI-Copilot, ActionEngine, OS-Symphony, RoboClaw, World-Value-Action |
| **Reflection and memory** | Agents must remember prior steps and recover from failures. | InfiGUIAgent, Agent S, MAGNET, OS-Symphony, MemGUI-Bench, MemoryVLA |
| **Agentic generation loops** | Generation quality depends on planning, verification, rollback, and editing. | Qwen-Image-2.0, Mind-Brush, VisionCreator, GenAgent, GEMS, ImAgent |
| **Tool-augmented action** | Retrieval, OCR, browsers, detectors, and executors are first-class components. | WebVoyager, Agent S2, OmniParser, UI-Copilot, CoAct-1, AutoGLM |
| **World modeling and latent planning** | One-shot action is giving way to predicting and evaluating future states. | StemVLA, World-Value-Action, Motus, AtomVLA, Visual Generation in the New Era |
| **Verification and self-correction** | Robust deployment requires explicit action-effect verification. | VeriGUI, GTAL, V-Droid, SEA |
| **Tactile and force-aware VLA** | Contact-rich manipulation requires force and tactile feedback. | HapticVLA |
| **Unsupervised / synthetic agent training** | Scaling beyond human demonstrations via autonomous RL and synthetic experience. | DigiRL, Evocua, NNetNav, SEA |

---

## Benchmarks and Environments

| Area | Benchmark / Environment | Links | Why It Matters |
|------|------------------------|-------|--------------|
| **Web** | VisualWebArena | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.13649) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/web-arena-x/visualwebarena) | Visually grounded browser tasks. |
| **Enterprise software** | WorkArena | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2403.07718) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ServiceNow/WorkArena) | Knowledge-work and enterprise workflows. |
| **General desktop** | OSWorld | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2404.07972) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OSWorld) | Real computer tasks across applications, GUI, and CLI. |
| **Desktop perception** | UI-Vision | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.15661) | Fine-grained offline benchmark for desktop perception and action prediction. |
| **Windows** | Windows Agent Arena | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2409.08264) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/microsoft/WindowsAgentArena) | Scalable Windows benchmark. |
| **Android** | AndroidWorld | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2405.14573) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/google-research/android_world) | Dynamic Android benchmark with broad task diversity. |
| **Android (cross-app)** | MobileWorld | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.16196) | Long-horizon and cross-app mobile workflows. |
| **Mobile systematic** | AndroidLab | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.14228) | Reproducible evaluation for mobile agents. |
| **Mobile interactive** | MobileAgentBench | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2406.08184) | Efficient benchmark across open-source apps. |
| **Smartphone evaluation** | SPA-Bench | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.15164) | Multilingual smartphone benchmark with plug-and-play integration. |
| **Desktop and web scripting** | OmniACT | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.17553) | Evaluates executable automation rather than only low-level traces. |
| **Interactive digital agents** | UINavBench | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.XXXXX) | ICCV 2025 comprehensive evaluation of interactive digital agents. |
| **GUI grounding** | ScreenSpot-Pro | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.07981) | High-resolution professional-screen grounding. |
| **GUI memory** | MemGUI-Bench | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.06075) | Cross-session memory in mobile GUI agents. |
| **GUI robustness** | GUI-Perturbed | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14262) | Brittleness under perturbations and relational instructions. |
| **Computer-use comprehensive** | GUI-360° | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2511.04307) | Large-scale dataset and benchmark for computer-using agents. |
| **Agentic visual search** | InterLV-Search | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.07510) | Repeated evidence seeking and cross-step integration. |
| **Vision-centric reasoning** | Agent-X | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.24876) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/mbzuai-oryx/Agent-X) | Step-level reasoning and tool-use assessment. |
| **Multimodal game agents** | GameWorld | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.07429) | Standardized, verifiable evaluation of MLLMs as game agents. |
| **Agent risk and safety** | RiOSWorld | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.00618) | Risk benchmarking for multimodal computer-use agents. |
| **Web agent reward** | AgentRewardBench | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.08942) | Automatic evaluation of web agent trajectories. |
| **Robotics manipulation** | VLABench | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2412.18194) | Long-horizon language-conditioned robotics manipulation. |
| **VLA robustness** | LIBERO-plus | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.13626) | In-depth robustness analysis of vision-language-action models. |
| **Robotics digital twins** | RoboTwin | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.13059) | Dual-arm robot benchmark with generative digital twins. |
| **General agent capability** | AgentVista / MMSkills | [![arXiv](https://img.shields.io/badge/arXiv-AgentVista-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.12056) [![arXiv](https://img.shields.io/badge/arXiv-MMSkills-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.13527) | Comprehensive and skill-based evaluation of general visual agents. |

---

## Skills and Tooling

&gt; **Design principle.** This section is organized into four layers:  
&gt; 1) **Skills** — reusable procedural abstractions (perception, generation, action);  
&gt; 2) **Harnesses** — the orchestration infrastructure that gives an LLM hands, eyes, memory, and safety boundaries;  
&gt; 3) **MCP Connectivity** — standardized protocol layer for visual agents to discover and call external tools;  
&gt; 4) **Toolchains** — concrete open-source implementations for research and production.

---

### 1. Agent Skills & Reusable Procedures

&gt; **Boundary note.** We list only skill libraries and skill-centric frameworks that are explicitly designed for multimodal or visual-agent workflows (GUI, VLA, or visual generation). Generic prompt templates are excluded.

| Resource | Year | Links | Type | Notes |
|----------|------|-------|------|-------|
| **XSkill** | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.12056) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/XSkill-Agent/XSkill) | Multimodal skill learning | ICML 2026. Continual learning from experience and skills in multimodal agents. Built-in experience bank, skill builder, and multimodal analysis engine. |
| **CUA-Skill** | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.21123) | Computer-use skill framework | Microsoft. Encodes human computer-use knowledge as reusable, parameterized skills with execution and composition graphs. Achieves SOTA 57.5% on WindowsAgentArena. |
| **SAGE** | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.17102) | RL skill library | Skill Augmented GRPO for self-evolution. Incorporates a skill library into agent training; +8.9% task completion, –59% tokens on AppWorld. |
| **Skill-R1** | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.09359) | Skill evolution via RL | Reinforcement-learning-driven skill evolution with reflective updates and compositional generalization. |
| **Generative-Media-Skills** | 2026 | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/SamurAIGPT/Generative-Media-Skills) | Visual-generation skills | Multimodal generative media skills (image, video, audio) for Claude Code, Cursor, Gemini CLI. Exposes muapi.ai generation pipeline via MCP. |
| **awesome-gpt-image-2** | living | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/freestylefly/awesome-gpt-image-2) | Prompt-as-code system | Polished prompt-as-code system and reusable visual style library for image-generation workflows. |
| **gpt_image_2_skill** | living | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/wuyoscar/gpt_image_2_skill) | Image-gen skill | Compact, reusable image-generation skill with CLI usage examples and schema validation. |
| **agentskills** (Awesome) | living | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/scienceaix/agentskills) | Curated skill index | Community-curated collection of agent skills, papers, tools, and projects across domains. |
| **Voyager / LATM / CREATOR** | 2023–2024 | [![arXiv](https://img.shields.io/badge/arXiv-Voyager-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2305.16291) [![arXiv](https://img.shields.io/badge/arXiv-LATM-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2305.17126) [![arXiv](https://img.shields.io/badge/arXiv-CREATOR-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2305.14318) | Skill-creation classics | Foundational works on LLM-as-tool-maker, automatic skill accumulation, and compositional skill synthesis. |

---

### 2. Agent Harnesses & Orchestration Frameworks

&gt; **Definition.** An *agent harness* is the complete infrastructure that wraps around an LLM to make it a functional agent: it provides hands (tool execution), eyes (perception APIs), memory (context persistence), and safety boundaries (sandboxing, guardrails).

| Resource | Year | Links | Type | Notes |
|----------|------|-------|------|-------|
| **vla-evaluation-harness** | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.13966) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/allenai/vla-evaluation-harness) | VLA evaluation harness | One framework to evaluate any VLA model on any robot simulation benchmark. 18 benchmarks × 13 model servers, Dockerized, 47× throughput via batch parallel eval. |
| **OpenHarness** | 2026 | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/HKUDS/OpenHarness) | General agent harness | Open-source Python harness with built-in personal agent, plugin architecture, and domain-knowledge extensibility. |
| **OpenAI Agents SDK** | 2026 | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/openai/openai-agents-python) | Production agent SDK | Multi-agent workflows, sandbox agents, MCP support, guardrails, tracing, and human-in-the-loop. 26K+ stars. |
| **Hermes Agent** | 2026 | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/NousResearch/hermes-agent) | Self-improving agent | Nous Research. Open-source agent with built-in skill creation, memory search, and RL training loop (Atropos). 23K+ stars. |
| **LangChain Deep Agents + OpenShell** | 2026 | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/langchain-ai/langchain) | Coding-agent harness | Reference architecture using LangGraph state-machine orchestration plus sandboxed code execution (OpenShell). |
| **UI-TARS-desktop** | 2025 | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/bytedance/UI-TARS-desktop) | Native desktop stack | End-to-end desktop operator workflows and GUI-agent experimentation with native agent inference. |
| **GELab-Zero** | 2026 | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://sourceforge.net/projects/gelab-zero/) | Local GUI harness | Fully local GUI-agent framework combining a 4B base model with input orchestration and GUI automation logic. |

---

### 3. MCP Servers & Visual-Agent Connectivity

&gt; **Why MCP matters for visual agents.** The Model Context Protocol (MCP) standardizes how agents discover and call external capabilities. For visual agents, MCP servers act as the universal plug layer connecting perception APIs (vision, segmentation, design tools, cloud resources) to the agent runtime.

| Resource | Year | Links | Type | Notes |
|----------|------|-------|------|-------|
| **VisionAgent MCP** | 2025 | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/landing-ai/vision-agent-mcp) | Vision MCP server | Landing AI. Proxies vision APIs (detection, segmentation, depth, OCR) to MCP clients. Auto-renders masks and bounding boxes to local PNG/JSON. |
| **Figma MCP (Dev Mode)** | 2025 | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://www.figma.com/dev-mode/) | Design MCP | Official Figma Dev Mode MCP server. Exposes live layer hierarchy, auto-layout, and design tokens so agents can generate code against real designs rather than screenshots. |
| **Context7 MCP** | 2026 | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/upstash/context7) | Documentation MCP | Documentation-as-context pipeline. Fetches current library docs and versioned APIs so visual-agent code generation stays grounded in up-to-date references. |
| **Azure MCP Server** | 2025 | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://devblogs.microsoft.com/visualstudio/azure-mcp-server-now-built-in-with-visual-studio-2026-a-new-era-for-agentic-workflows/) | Cloud MCP | Built into Visual Studio 2026. Enables agents to query and manage Azure resources (AKS, Cosmos DB, AI Foundry) via natural language. |
| **Filesystem MCP** | 2024 | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem) | Local filesystem MCP | Official reference implementation. Secure directory-scoped file access for agents; read-only defaults with explicit allowlisting. |
| **OpenClaw + Clawctl** | 2026 | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/openclaw/openclaw) | Agent runtime with MCP | Agent runtime that natively spawns MCP servers as child processes, with built-in sandboxing and security policy enforcement. |

---

### 4. Core Reference Repositories

| Repository | Links | Why It Is Useful |
|------------|-------|------------------|
| Evolving Visual Generation | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EvolvingLMMs-Lab/Evolving-Visual-Generation) | Strongest living resource hub on the visual-generation side. |
| awesome-gpt-image-2 | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/freestylefly/awesome-gpt-image-2) | Polished prompt-as-code system and reusable visual style library. |
| gpt_image_2_skill | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/wuyoscar/gpt_image_2_skill) | Compact image-generation skill with examples and CLI usage. |
| XSkill | [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/XSkill-Agent/XSkill) | Experience-driven multimodal skill accumulation with continual learning. |
| agentskills | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/scienceaix/agentskills) | Curated awesome-list for agent skills, papers, and tooling. |

---

### 5. Open-Source Toolchains

| Tool | Type | Links | Best For |
|------|------|-------|----------|
| **lmms-eval** | evaluation toolkit | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EvolvingLMMs-Lab/lmms-eval) | Unified multimodal evaluation across image, video, audio, and chat. |
| **vla-evaluation-harness** | robotics eval harness | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/allenai/vla-evaluation-harness) | Cross-benchmark VLA evaluation at scale (18 benchmarks, Dockerized, batch parallel). |
| **OmniParser** | GUI parsing | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/microsoft/OmniParser) | Converting screenshots into interactable regions for vision-only GUI agents. |
| **UI-TARS-desktop** | native desktop agent stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/bytedance/UI-TARS-desktop) | End-to-end desktop operator workflows and GUI-agent experimentation. |
| **Agent-S** | computer-use framework | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/simular-ai/Agent-S) | Hierarchical computer-use flows with memory and planning. |
| **OpenVLA** | embodied VLA stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/openvla/openvla) | Open VLA fine-tuning, evaluation, and robotics experiments. |
| **AndroidWorld** | benchmark environment | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/google-research/android_world) | Android control agents with dynamic task instantiation. |
| **OSWorld** | desktop benchmark environment | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OSWorld) | Real-computer evaluation loop for GUI agents. |
| **Cradle** | general computer control | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/BAAI-Agents/Cradle) | Generalist agent framework for games, OS, and software control. |
| **SWE-agent** | software engineering agent | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/princeton-nlp/SWE-agent) | Agent-computer interfaces for code-based environment control. |
| **OpenHarness** | general agent harness | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/HKUDS/OpenHarness) | Research-oriented harness for building and extending specialized agents. |
| **Landing AI VisionAgent** | vision API + MCP | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/landing-ai/vision-agent-mcp) | Bridging cloud vision APIs to local MCP clients with visualization output. |

---

### 6. Tool Selection by Workflow

| Workflow | Recommended Stack |
|----------|-------------------|
| **Visual-generation prototyping** | `awesome-gpt-image-2` + `gpt_image_2_skill` + `Generative-Media-Skills` + Qwen-Image style prompting |
| **GUI grounding and action** | `OmniParser` + `UI-TARS-desktop` + `Agent-S` + `SeeClick` + `CUA-Skill` |
| **Benchmark-heavy visual-agent research** | `lmms-eval` + `OSWorld` + `AndroidWorld` + `VisualWebArena` + `GameWorld` |
| **Embodied visual agents / robotics** | `OpenVLA` + `vla-evaluation-harness` + `VLABench` + simulation stack from VLA papers |
| **General computer-use automation** | `Cradle` + `OS-Copilot` + `OS-Symphony` + `SWE-agent` + `OpenHarness` |
| **Skill-driven multimodal agents** | `XSkill` + `agentskills` + `OpenAI Agents SDK` + `Hermes Agent` |
| **VLA research & cross-benchmark eval** | `vla-evaluation-harness` + `OpenVLA` + `lmms-eval` + `LIBERO-plus` |
| **Production computer-use with reusable skills** | `CUA-Skill` + `Agent-S2` + `Azure MCP` + `OpenHarness` |
| **Visual generation as composable service** | `Generative-Media-Skills` + `VisionAgent MCP` + `Qwen-Image-2.0` |
| **Design-to-code agent workflows** | `Figma MCP` + `OmniParser` + `UI-TARS-desktop` + `Context7 MCP` |

---

## Blogs and Deep Dives

This section prioritizes durable technical writeups over hype posts.

### English

| Resource | Links | Focus |
|----------|-------|-------|
| OpenAI: Computer-Using Agent | [OpenAI](https://openai.com/index/computer-using-agent/) | Product and research framing for computer-use agents. |
| OpenAI API: Computer Use Guide | [OpenAI Docs](https://platform.openai.com/docs/guides/tools-computer-use) | Developer-facing usage guide for computer-use workflows. |
| Anthropic: Developing a Computer Use Model | [Anthropic](https://www.anthropic.com/news/developing-computer-use) | One of the best public engineering writeups on GUI-agent development. |
| Anthropic: Introducing computer use | [Anthropic](https://www.anthropic.com/news/3-5-models-and-computer-use) | Concise launch overview plus deployment framing. |
| Google DeepMind: Gemini Robotics | [DeepMind](https://deepmind.google/blog/gemini-robotics-brings-ai-into-the-physical-world/) | Frontier industry view on VLA systems. |
| Google DeepMind: Gemini Robotics On-Device | [DeepMind](https://deepmind.google/discover/blog/gemini-robotics-on-device-brings-ai-to-local-robotic-devices/) | Low-latency on-device VLA deployment. |
| Qwen Blog: Qwen-Image | [Qwen](https://qwenlm.github.io/blog/qwen-image/) | Official explainer for text rendering and visual-generation capabilities. |
| Roboflow: VLA Models for Robotics | [Roboflow](https://blog.roboflow.com/vision-language-action-models/) | Practical engineering-oriented VLA overview. |
| Physical AI Architecture: VLA & Robotics Inference (2026) | [NeuralCoreTech](https://neuralcoretech.com/physical-ai-architecture-vla-robotics/) | Deep-dive into VLA architecture, training pipelines, and edge deployment. |

### Chinese

| Resource | Links | Focus |
|----------|-------|-------|
| Qwen-Image Blog | [Qwen](https://qwenlm.github.io/blog/qwen-image/) | Text rendering, posters, PPT, and infographic generation. |
| ModelScope Agent Column | [ModelScope](https://community.modelscope.cn/column/6698a64b7fda170768204e20) | Chinese engineering column tracking agent systems. |
| ModelScope-Agent: multi-strategy and multimodal retrieval | [ModelScope](https://community.modelscope.cn/667a2906f194d31df8b07edd.html) | Practical multimodal retrieval and agent engineering writeup. |
| OmAgent - RL-based multimodal agent | [OM AI Lab](https://om-ai-lab.github.io/2025_07_17_zh.html) | Chinese post on multimodal agent plus RL practice. |
| MMLab Column at Jiqizhixin | [Jiqizhixin](https://www.jiqizhixin.com/columns/MMLab) | Ongoing Chinese information stream for multimodal vision work. |

### Ongoing Tracking

| Feed | Links | Why Follow It |
|------|-------|---------------|
| Evolving Visual Generation | [GitHub](https://github.com/EvolvingLMMs-Lab/Evolving-Visual-Generation) | Best living list for visual-generation-side developments. |
| lmms-eval releases | [GitHub](https://github.com/EvolvingLMMs-Lab/lmms-eval) | Proxy for what multimodal evaluation users actually care about. |
| Qwen Blog | [Qwen](https://qwenlm.github.io/blog/) | Strong signal for open multimodal and image-generation releases. |
| OpenEnvision / Awesome-Visual-Agent | [GitHub](https://github.com/OpenEnvision/Awesome-Visual-Agent) | Primary home for the curated visual-agent landscape itself. |

---

## Suggested Reading Paths

### Path A: GUI / Computer-Use Agent Builder

1. [SeeClick](https://arxiv.org/abs/2401.10935)
2. [ScreenAI](https://arxiv.org/abs/2402.04615)
3. [OmniParser](https://arxiv.org/abs/2408.00203)
4. [Cradle](https://arxiv.org/abs/2403.03186)
5. [OS-Copilot](https://arxiv.org/abs/2402.07456)
6. [AutoGLM](https://arxiv.org/abs/2411.00820)
7. [VisualWebArena](https://arxiv.org/abs/2401.13649)
8. [OSWorld](https://arxiv.org/abs/2404.07972)
9. [UI-TARS](https://arxiv.org/abs/2501.12326)
10. [Agent S2](https://arxiv.org/abs/2504.00906)
11. [VeriGUI](https://arxiv.org/abs/2604.05477)
12. [UI-Copilot](https://arxiv.org/abs/2604.13822)
13. [ActionEngine](https://arxiv.org/abs/2602.20502)
14. [OS-Symphony](https://arxiv.org/abs/2601.07779)

### Path B: Agentic Visual Generation

1. [Mind-Brush](https://arxiv.org/abs/2602.01756)
2. [VisionCreator](https://arxiv.org/abs/2603.02681)
3. [GenAgent](https://arxiv.org/abs/2601.18543)
4. [GEMS](https://arxiv.org/abs/2603.28088)
5. [ImAgent](https://arxiv.org/abs/2511.11483)
6. [GenSearcher](https://arxiv.org/abs/2603.28767)
7. [Unify-Agent](https://arxiv.org/abs/2603.29620)
8. [Qwen-Image-2.0](https://arxiv.org/abs/2605.10730)
9. [Visual Generation in the New Era](https://arxiv.org/abs/2604.28185)

### Path C: Embodied Visual Agents / Robotics

1. [RT-2](https://arxiv.org/abs/2307.15818)
2. [OpenVLA](https://arxiv.org/abs/2406.09246)
3. [π₀](https://arxiv.org/abs/2410.24164)
4. [Interleave-VLA](https://arxiv.org/abs/2505.02152)
5. [ChatVLA-2](https://arxiv.org/abs/2505.21906)
6. [LaRA-VLA](https://arxiv.org/abs/2602.01166)
7. [LLaVA-VLA](https://arxiv.org/abs/2602.22663)
8. [RoboClaw](https://arxiv.org/abs/2603.11558)
9. [FAEA](https://arxiv.org/abs/2601.20334)
10. [StemVLA](https://arxiv.org/abs/2602.23721)
11. [World-Value-Action Model](https://arxiv.org/abs/2604.14732)

### Path D: Evaluation, Safety, and Long-Horizon Benchmarks

1. [OSWorld](https://arxiv.org/abs/2404.07972)
2. [AndroidWorld](https://arxiv.org/abs/2405.14573)
3. [VisualWebArena](https://arxiv.org/abs/2401.13649)
4. [GameWorld](https://arxiv.org/abs/2604.07429)
5. [Agent-X](https://arxiv.org/abs/2505.24876)
6. [MMSkills](https://arxiv.org/abs/2605.13527)
7. [RiOSWorld](https://arxiv.org/abs/2506.00618)
8. [Claw-Eval](https://arxiv.org/abs/2604.06132)
9. [Vision-Language-Action Safety](https://arxiv.org/abs/2604.23775)

---

## Related Awesome Repositories

| Repository | Links | Notes |
|------------|-------|-------|
| Awesome Multimodal Modeling | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/OpenEnvision/Awesome-Multimodal-Modeling) | Complementary index for broader multimodal modeling beyond visual agents. |
| Evolving Visual Generation | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EvolvingLMMs-Lab/Evolving-Visual-Generation) | Best companion list for the visual-generation side. |
| Awesome-GUI-Agents | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/Awesome-GUI-Agents) | Cross-check list for GUI grounding, automation, and benchmark papers. |
| GUI-Agents-Paper-List | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/OSU-NLP-Group/GUI-Agents-Paper-List) | Systematic community-maintained paper index with structured metadata. |
| awesome-gpt-image-2 | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/freestylefly/awesome-gpt-image-2) | High-quality prompt system and skill library for generation workflows. |
| gpt_image_2_skill | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/wuyoscar/gpt_image_2_skill) | Focused image-generation skill and example repository. |
| awesome-ui-agents | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/opendilab/awesome-ui-agents) | Extra depth on UI agents. |

---

## Curation Principles

- **Prefer papers that define a new capability, benchmark, training recipe, or systems bottleneck.**
- **Prefer official artifacts whenever possible:** paper, code, project page, benchmark, or toolkit.
- **Exclude generic vision backbones, unified multimodal foundation models, and pure generation/training recipes** unless they are directly agentic—i.e., they close the loop between perception, reasoning, memory, tool use, generation, and action.
- **Separate tracks:** visual understanding, agentic generation, computer use, and embodied action—rather than collapsing them into one giant bucket.
- **Track fresh work explicitly with dates** when the field is moving quickly.
- **Include practical tools only when they materially help research, evaluation, or deployment.**
- **Maintain academic rigor:** prioritize peer-reviewed or widely cited arXiv preprints with official artifacts.

---

## Contributing

Pull requests are welcome, especially for:

- New **2026+** papers with official code or benchmarks.
- Missing GUI / VLA / interleaved evaluation environments.
- High-quality open-source tools and skill repositories.
- Stronger structure, cleaner categorization, and better reading paths.

When adding an item, please include:

- Title and year.
- Short note on **why it matters** (not just what it is).
- Official paper and, when available, official code.
- Category placement that matches this taxonomy.

---

## Acknowledgments

This repository was shaped with direct inspiration from:

- [OpenEnvision/Awesome-Multimodal-Modeling](https://github.com/OpenEnvision/Awesome-Multimodal-Modeling)
- [EvolvingLMMs-Lab/Evolving-Visual-Generation](https://github.com/EvolvingLMMs-Lab/Evolving-Visual-Generation)
- [freestylefly/awesome-gpt-image-2](https://github.com/freestylefly/awesome-gpt-image-2)
- [wuyoscar/gpt_image_2_skill](https://github.com/wuyoscar/gpt_image_2_skill)
- [ZJU-REAL/Awesome-GUI-Agents](https://github.com/ZJU-REAL/Awesome-GUI-Agents)
- [OSU-NLP-Group/GUI-Agents-Paper-List](https://github.com/OSU-NLP-Group/GUI-Agents-Paper-List)

They are strong examples of awesome repositories that function as research maps, workflow hubs, and practical entry points rather than simple lists of links.
