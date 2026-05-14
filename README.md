<a id="top"></a>

# Awesome Visual Agent

<div align="center">

<p>
  <strong>A carefully curated map of visual agents across understanding, generation, interleaved multimodality, GUI/computer use, and embodied vision-language-action systems.</strong>
</p>

<p>
  <a href="https://github.com/OpenEnvision/Awesome-Visual-Agent">Repository</a> |
  <a href="https://github.com/EvolvingLMMs-Lab/Evolving-Visual-Generation">Evolving Visual Generation</a> |
  <a href="https://github.com/OpenEnvision/Awesome-Multimodal-Modeling">Awesome Multimodal Modeling</a> |
  <a href="https://github.com/freestylefly/awesome-gpt-image-2">awesome-gpt-image-2</a> |
  <a href="https://github.com/wuyoscar/gpt_image_2_skill">gpt_image_2_skill</a>
</p>

<p>
  <img alt="curation" src="https://img.shields.io/badge/curation-research--driven-111111?style=for-the-badge">
  <img alt="scope" src="https://img.shields.io/badge/scope-visual%20agents-0f766e?style=for-the-badge">
  <img alt="years" src="https://img.shields.io/badge/coverage-2023--2026-c2410c?style=for-the-badge">
  <img alt="updated" src="https://img.shields.io/badge/updated-2026--05--14-1d4ed8?style=for-the-badge">
</p>

</div>

> [!IMPORTANT]
> This repository is designed as a professional research-and-building index, not a flat bookmark dump. It emphasizes taxonomy, official artifacts, open tooling, evaluation environments, and reading paths around visual-agent work. Generic vision models and broad multimodal foundation models are intentionally excluded unless they are directly agentic, interleaved, or central to a visual-agent workflow.

## Table of Contents

- [Why This Repo](#why-this-repo)
- [2026 Radar](#2026-radar)
- [Taxonomy at a Glance](#taxonomy-at-a-glance)
- [Application View](#application-view)
- [Link Badge Legend](#link-badge-legend)
- [Research Map](#research-map)
  - [1. Surveys, Roadmaps, and Big-Picture Guides](#1-surveys-roadmaps-and-big-picture-guides)
  - [2. Visual Understanding, Grounding, and Screen Perception](#2-visual-understanding-grounding-and-screen-perception)
  - [3. Visual Generation and Agentic Generation](#3-visual-generation-and-agentic-generation)
  - [4. Interleaved and Unified Understanding-Generation Models](#4-interleaved-and-unified-understanding-generation-models)
  - [5. GUI and Computer-Use Agents](#5-gui-and-computer-use-agents)
  - [6. Embodied Vision-Language-Action Agents](#6-embodied-vision-language-action-agents)
  - [7. Interleaved and Agentic Evaluation](#7-interleaved-and-agentic-evaluation)
- [Technology View](#technology-view)
- [Benchmarks and Environments](#benchmarks-and-environments)
- [Skills and Tooling](#skills-and-tooling)
  - [Core Reference Repositories](#core-reference-repositories)
  - [Install: `awesome-gpt-image-2` Skill](#install-awesome-gpt-image-2-skill)
  - [Install: `gpt_image_2_skill` for Codex](#install-gpt_image_2_skill-for-codex)
  - [Open-Source Toolchains Worth Installing](#open-source-toolchains-worth-installing)
  - [Tool Selection by Workflow](#tool-selection-by-workflow)
- [Blogs and Deep Dives](#blogs-and-deep-dives)
  - [English](#english)
  - [Chinese](#chinese)
  - [Ongoing Tracking](#ongoing-tracking)
- [Suggested Reading Paths](#suggested-reading-paths)
- [Related Awesome Repositories](#related-awesome-repositories)
- [Curation Principles](#curation-principles)
- [Contributing](#contributing)
- [Acknowledgments](#acknowledgments)

## Link Badge Legend

- Paper: [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/)
- Code: [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/)
- Project / living list / toolkit: [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/)

[Back to top](#top)

## Why This Repo

Visual agents are no longer just "VLMs that can see." The field is rapidly converging toward systems that can:

- ground language in pixels, screens, layouts, objects, and documents
- reason over long horizons with memory, reflection, and recovery
- call tools and use external environments instead of only answering
- generate images, edits, layouts, and multimodal artifacts
- interleave text and image as both input and output
- act in digital systems and physical robotic environments

This list treats a `visual agent` as a system that closes the loop between `visual perception`, `reasoning`, `memory`, `tool use`, `generation`, and `action`.

To keep the boundary clean, this list prioritizes:

- visual understanding agents instead of generic VLMs
- visual generation systems that are agentic, workflow-oriented, or central to agentic creation
- interleaved multimodal systems that mix image and text across a trajectory
- GUI / computer-use agents, embodied VLA agents, and their benchmarks
- tools that are directly useful for building or evaluating visual agents

[Back to top](#top)

## 2026 Radar

| Work | Date | Links | Why It Matters |
| --- | --- | --- | --- |
| Qwen-Image-2.0 Technical Report | 2026-05-11 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.10730) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/QwenLM/Qwen-Image) | Stronger typography-heavy generation and editing for posters, slides, infographics, and multilingual text rendering. |
| InterLV-Search | 2026-05-08 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.07510) | Benchmarks interleaved language-vision search with visual evidence reused across multiple search decisions. |
| UI-Zoomer | 2026-04-15 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14113) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/UI-Zoomer) | Strong new training-free zoom-in method for small icons and dense GUI grounding. |
| UI-Copilot | 2026-04-15 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.13822) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/UI-Copilot) | Directly targets long-horizon GUI automation with retrieval and calculator tools. |
| Vision-Language-Action Safety | 2026-04-26 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.23775) | Timely survey on safety, attacks, evaluation, and deployment of embodied VLA systems. |
| Vision-Language-Action in Robotics: A Survey of Datasets, Benchmarks, and Data Engines | 2026-04-24 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.23001) | Strong data-centric view of why VLA progress is increasingly limited by infrastructure, not only architecture. |
| World-Value-Action Model | 2026-04-16 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14732) | Pushes VLA systems toward latent-space planning and implicit future evaluation. |
| Visual Generation in the New Era | 2026-04-11 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.28185) | Excellent roadmap from atomic mapping to agentic world modeling in visual generation. |
| VisionCreator | 2026-03-03 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.02681) | Native visual-generation agentic model that unifies understanding, planning, and creation. |
| UniM | 2026-03-05 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.05075) | Any-to-any interleaved multimodal benchmark with agentic baseline. |
| DuoGen | 2026-01-31 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.00508) | Strong open direction for general-purpose interleaved image-text generation. |
| ShowUI-Aloha | 2026-01-12 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.07181) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/showlab/ShowUI) | Important human-demonstration pipeline for teaching GUI agents from screen recordings. |
| OS-Symphony | 2026-01-12 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.07779) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OS-Copilot/OS-Symphony) | One of the strongest recent frameworks for memory, reflection, and retrieval-aware computer use. |

[Back to top](#top)

## Taxonomy at a Glance

| Track | Core Question | Typical Outputs | Representative Starting Points |
| --- | --- | --- | --- |
| Visual Understanding Agents | Can the agent perceive, localize, parse, and reason over visual inputs? | answers, boxes, structured extraction, grounded summaries | ScreenAI, CogAgent, SeeClick, OmniParser |
| Visual Generation Agents | Can the agent plan and render images, edits, layouts, and visual documents? | images, edits, posters, diagrams, slides | Qwen-Image, Qwen-Image-2.0, Evolving Visual Generation |
| Interleaved Agents | Can the system mix text and image as both inputs and outputs over a coherent trajectory? | illustrated reasoning, mixed-modal reports, visual tutorials | MiniGPT-5, Emu3, Show-o, Janus, DuoGen |
| GUI / Computer-Use Agents | Can the agent operate websites, desktops, and mobile apps from screenshots and action history? | clicks, typing, navigation, task trajectories | SeeClick, UI-TARS, Agent S2, OSWorld |
| Embodied VLA Agents | Can the agent turn visual observations and language into physical actions? | robot trajectories, manipulation plans, embodied traces | RT-2, OpenVLA, Magma, World-Value-Action |
| Evaluation / Tooling | How do we benchmark and operationalize all of the above? | environments, leaderboards, eval stacks, skills | VisualWebArena, AndroidWorld, lmms-eval |

[Back to top](#top)

## Application View

| Application Area | What the Agent Needs | Representative Building Blocks |
| --- | --- | --- |
| Visual QA, documents, charts, infographics | OCR, layout parsing, grounding, structured extraction, long-context reasoning | ScreenAI, CogAgent, SeeClick, OmniParser |
| Image generation and editing | planning, controllability, typography, reference preservation, verifier loops | Qwen-Image, Qwen-Image-2.0, Evolving Visual Generation, generation skills |
| Interleaved tutorials and illustrated reports | mixed-modal decoding, narrative control, long context | MiniGPT-5, Emu3, Show-o, Janus, DuoGen, UniM |
| Browser, desktop, and mobile automation | screenshot grounding, memory, reflection, environment APIs | SeeClick, OmniParser, UI-TARS, Agent S2, OSWorld, AndroidWorld |
| Embodied manipulation and robot control | VLM priors, action tokenization, temporal modeling, planning under dynamics | RT-2, OpenVLA, Interleave-VLA, StemVLA, World-Value-Action |

[Back to top](#top)

## Research Map

### 1. Surveys, Roadmaps, and Big-Picture Guides

| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| Visual Generation in the New Era: An Evolution from Atomic Mapping to Agentic World Modeling | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.28185) | The cleanest recent roadmap for modern visual generation and agentic world modeling. |
| A Survey on (M)LLM-Based GUI Agents | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.13865) | Strong entry point for GUI-agent architectures, planning, grounding, and evaluation. |
| GUI Agents: A Survey | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2412.13501) | Broad overview of task settings, model classes, and protocols for GUI agents. |
| Towards Trustworthy GUI Agents: A Survey | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.23434) | Useful for robustness, reliability, and deployment risk. |
| Survey of Vision-Language-Action Models for Embodied Manipulation | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.15201) | Practical survey of VLA structures, datasets, post-training, and evaluation. |
| A Survey on Vision-Language-Action Models: An Action Tokenization Perspective | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.01925) | Helpful for understanding why VLA systems differ in how they express action. |

[Back to top](#top)

### 2. Visual Understanding, Grounding, and Screen Perception

| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| ScreenAI: A Vision-Language Model for UI and Infographics Understanding | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.04615) | Key work for UI, infographic, and visually structured understanding. |
| CogAgent: A Visual Language Model for GUI Agents | 2023 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2312.08914) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/THUDM/CogAgent) | Early strong open model for screenshot-driven GUI understanding and navigation. |
| SeeClick: Harnessing GUI Grounding for Advanced Visual GUI Agents | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.10935) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/njucckevin/SeeClick) | Foundational if grounding is the bottleneck you care about most. |
| UGround: Universal Visual Grounding for GUI Agents | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.05243) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OSU-NLP-Group/UGround) | One of the strongest 2024 grounding papers, arguing for fully visual human-like GUI perception. |
| OS-ATLAS: A Foundation Action Model for Generalist GUI Agents | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.23218) | Strong action-grounding model and large cross-platform GUI corpus for open GUI agents. |
| Ferret-UI: Grounded Mobile UI Understanding with Multimodal LLMs | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2404.05719) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/apple/ml-ferret) | Strong mobile-UI grounding work with explicit region-aware training. |
| ShowUI: One Vision-Language-Action Model for GUI Visual Agent | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2411.17465) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/showlab/ShowUI) | Unified VLA-style GUI agent with screenshot-conditioned action modeling. |
| OmniParser for Pure Vision Based GUI Agent | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2408.00203) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/microsoft/OmniParser) | One of the most practical tools for parsing screenshots into reliable interactable regions. |
| Aguvis: Unified Pure Vision Agents for Autonomous GUI Interaction | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2412.04454) | Important pure-vision GUI agent without dependence on textual trees. |
| InfiGUIAgent: A Multimodal Generalist GUI Agent with Native Reasoning and Reflection | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2501.04575) | Notable for expectation-reflection and explicit multi-step reasoning. |
| UI-Zoomer: Uncertainty-Driven Adaptive Zoom-In for GUI Grounding | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14113) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/UI-Zoomer) | Strong training-free zoom-in framework for small targets and dense layouts. |

[Back to top](#top)

### 3. Visual Generation and Agentic Generation

| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| Qwen-Image Technical Report | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2508.02324) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/QwenLM/Qwen-Image) | Strong open image generation and editing system with excellent text rendering. |
| Qwen-Image-2.0 Technical Report | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.10730) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/QwenLM/Qwen-Image) | Major upgrade for dense text rendering, infographics, editing, and 2K generation. |
| X-Omni: Reinforcement Learning Makes Discrete Autoregressive Image Generative Models Great Again | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2507.22058) | Useful if you care about RL-enhanced image generation systems. |
| Mind-Brush: Integrating Agentic Cognitive Search and Reasoning into Image Generation | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.01756) | A clean example of image generation becoming a retrieval-and-reasoning workflow rather than static decoding. |
| VisionCreator: A Native Visual-Generation Agentic Model with Understanding, Thinking, Planning and Creation | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.02681) | End-to-end agentic visual creation model with an explicit understanding-thinking-planning-creation loop. |
| A Unified Agentic Framework for Evaluating Conditional Image Generation | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.07046) | Helpful if you want agentic evaluation for conditional image generation rather than only static metrics. |
| Visual Generation in the New Era: An Evolution from Atomic Mapping to Agentic World Modeling | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.28185) | The best recent roadmap for understanding visual generation as an increasingly agentic process. |
| Evolving Visual Generation | living repo | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EvolvingLMMs-Lab/Evolving-Visual-Generation) | One of the strongest continuously updated hubs for visual generation papers and trends. |

[Back to top](#top)

### 4. Interleaved and Unified Understanding-Generation Models

| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| MiniGPT-5: Interleaved Vision-and-Language Generation via Generative Vokens | 2023 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2310.02239) | Early milestone for interleaved multimodal generation. |
| ARMOR v0.1: Empowering Autoregressive Multimodal Understanding Model with Interleaved Multimodal Generation via Asymmetric Synergy | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.06542) | One of the cleaner 2025 attempts to retrofit interleaved generation into autoregressive multimodal models. |
| Emu3: Next-Token Prediction is All You Need | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2409.18869) | Major token-unification paper across image, video, and text. |
| Show-o: One Single Transformer to Unify Multimodal Understanding and Generation | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2408.12528) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/showlab/show-o) | Clean and influential unified model framing. |
| Janus: Decoupling Visual Encoding for Unified Multimodal Understanding and Generation | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.13848) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/deepseek-ai/Janus) | Useful for understanding why separate visual encoders still matter. |
| Janus-Pro | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2501.17811) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/deepseek-ai/Janus) | Scaled-up Janus direction with stronger multimodal capabilities. |
| Show-o2 | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2506.15564) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/showlab/show-o) | Extends unified modeling further into image and video. |
| DuoGen: Towards General Purpose Interleaved Multimodal Generation | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.00508) | One of the newest strong open references for general-purpose interleaved generation. |
| Unified Multimodal Model as Auto-Encoder | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2509.09666) | Useful if you want to track auto-encoding formulations for unified multimodal systems. |

[Back to top](#top)

### 5. GUI and Computer-Use Agents

| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| AppAgent: Multimodal Agents as Smartphone Users | 2023 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2312.13771) | Foundational smartphone-use agent. |
| WebVoyager: Building an End-to-End Web Agent with Large Multimodal Models | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.13919) | Early strong end-to-end web agent. |
| VisualWebArena | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.13649) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/web-arena-x/visualwebarena) | Central benchmark for visually grounded browser agents. |
| OmniACT: A Dataset and Benchmark for Enabling Multimodal Generalist Autonomous Agents for Desktop and Web | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.17553) | Useful benchmark when executable scripts matter more than raw low-level actions. |
| WorkArena | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2403.07718) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ServiceNow/WorkArena) | Practical knowledge-work benchmark around enterprise workflows. |
| OSWorld | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2404.07972) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OSWorld) | The flagship open benchmark for real computer-use agents. |
| Windows Agent Arena | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2409.08264) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/microsoft/WindowsAgentArena) | Strong scalable Windows benchmark with cloud-scale evaluation support. |
| AndroidWorld | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2405.14573) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/google-research/android_world) | Dynamic Android environment with millions of task variations. |
| Magma: A Foundation Model for Multimodal AI Agents | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2502.13130) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/microsoft/Magma) | Important bridge paper spanning digital and physical agent settings. |
| Advancing Mobile GUI Agents: A Verifier-Driven Approach to Practical Deployment | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.15937) | Introduces V-Droid, a verifier-driven mobile GUI agent that emphasizes practical deployment and latency. |
| UI-TARS: Pioneering Automated GUI Interaction with Native Agents | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2501.12326) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/bytedance/UI-TARS) | End-to-end native GUI agent and one of the clearest signals of where the field is heading. |
| Agent S | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.08164) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/simular-ai/Agent-S) | Strong open framework for hierarchical planning and experience reuse. |
| Agent S2: A Compositional Generalist-Specialist Framework for Computer Use Agents | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.00906) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/simular-ai/Agent-S) | Strong compositional upgrade focused on grounding specialists and proactive planning. |
| ScreenSpot-Pro: GUI Grounding for Professional High-Resolution Computer Use | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.07981) | Important if you care about real professional interfaces instead of toy screenshots. |
| ShowUI-Aloha: Human-Taught GUI Agent | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.07181) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/showlab/ShowUI) | Valuable pipeline for turning raw human screen recordings into structured GUI-agent supervision. |
| UI-Copilot: Advancing Long-Horizon GUI Automation via Tool-Integrated Policy Optimization | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.13822) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/UI-Copilot) | Strong recent result for long-horizon GUI tasks with explicit retrieval and calculator assistance. |
| OS-Symphony: A Holistic Framework for Robust and Generalist Computer-Using Agent | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2601.07779) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/OS-Copilot/OS-Symphony) | Strong recent result on memory, reflection, and visual-aware tutorial retrieval. |
| VideoWebArena | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.19100) | Useful for long-context video understanding inside web-agent workflows. |

[Back to top](#top)

### 6. Embodied Vision-Language-Action Agents

| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control | 2023 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2307.15818) | Canonical VLA paper that transferred web knowledge into robot action. |
| OpenVLA: An Open-Source Vision-Language-Action Model | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2406.09246) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/openvla/openvla) | Central open baseline for robot-facing VLA work. |
| Interleave-VLA | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.02152) | Extends VLA systems to interleaved image-text instructions. |
| ChatVLA-2 | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.21906) | Interesting direction for preserving open-world reasoning in embodied VLA systems. |
| VLA^2 | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2510.14902) | Highlights the role of agentic external modules for unseen concept manipulation. |
| StemVLA | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.23721) | Adds future 3D geometry and 4D historical representation into action prediction. |
| World-Value-Action Model | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14732) | Worth tracking for long-horizon latent planning under physical constraints. |

[Back to top](#top)

### 7. Interleaved and Agentic Evaluation

| Work | Year | Links | Notes |
| --- | --- | --- | --- |
| MMIE | 2024 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.10139) | Strong benchmark for interleaved multimodal comprehension and generation. |
| UniM | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.05075) | Any-to-any benchmark across seven modalities. |
| InterLV-Search | 2026 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.07510) | Useful for agentic search with repeatedly reused visual evidence. |
| Agent-X: Evaluating Deep Multimodal Reasoning in Vision-Centric Agentic Tasks | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.24876) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/mbzuai-oryx/Agent-X) | Valuable when you care about step-level reasoning quality instead of only final success. |
| FysicsWorld | 2025 | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2512.12756) | Larger full-modality any-to-any evaluation view. |

[Back to top](#top)

## Technology View

| Technical Theme | Why It Matters | Representative Works |
| --- | --- | --- |
| Grounding and screen parsing | Agents fail if they cannot point to the right region, button, token, or object | SeeClick, UGround, OmniParser, UI-Zoomer, ScreenSpot-Pro |
| Long-horizon planning | Real tasks need subgoals, recovery, and temporal abstraction | Agent S, Agent S2, OS-Symphony, World-Value-Action |
| Reflection and memory | Agents need to remember prior steps and recover from failures | InfiGUIAgent, Agent S, UI-Copilot, OS-Symphony, MemGUI-Bench |
| Unified tokenization and interleaving | Interleaved systems benefit from text and image sharing a common trajectory space | Emu3, MiniGPT-5, Show-o, DuoGen |
| Unified understanding plus generation | Modern systems increasingly need to analyze and create visuals in one coherent loop | Show-o, Janus, Qwen-Image, Qwen-Image-2.0, VisionCreator |
| Agentic generation loops | Generation quality increasingly depends on planning, verification, rollback, and editing | Qwen-Image-2.0, Mind-Brush, VisionCreator, X-Omni, Evolving Visual Generation |
| Tool-augmented action | Retrieval, OCR, browsers, detectors, and executors are becoming first-class components | WebVoyager, Agent S2, OmniParser |
| World modeling | One-shot action is giving way to predicting and evaluating future states | StemVLA, World-Value-Action, Visual Generation in the New Era |

[Back to top](#top)

## Benchmarks and Environments

| Area | Benchmark / Environment | Links | Why It Matters |
| --- | --- | --- | --- |
| Web | VisualWebArena | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2401.13649) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/web-arena-x/visualwebarena) | Visually grounded browser tasks. |
| Enterprise software | WorkArena | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2403.07718) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/ServiceNow/WorkArena) | Knowledge-work and enterprise workflows. |
| General desktop | OSWorld | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2404.07972) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OSWorld) | Real computer tasks across applications, GUI, and CLI. |
| Desktop perception and interaction | UI-Vision | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2503.15661) | Fine-grained offline benchmark for desktop perception, layout grounding, and action prediction. |
| Windows | Windows Agent Arena | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2409.08264) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/microsoft/WindowsAgentArena) | Scalable Windows benchmark. |
| Android | AndroidWorld | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2405.14573) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/google-research/android_world) | Dynamic Android benchmark with broad task diversity. |
| Desktop and web scripting | OmniACT | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2402.17553) | Evaluates executable automation rather than only low-level control traces. |
| GUI grounding | ScreenSpot-Pro | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2504.07981) | High-resolution professional-screen grounding benchmark. |
| GUI memory | MemGUI-Bench | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2602.06075) | Strong new benchmark for cross-session and cross-temporal memory in mobile GUI agents. |
| GUI robustness diagnostics | GUI-Perturbed | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.14262) | Reveals brittleness in GUI grounding under perturbations and relational instructions. |
| Interleaved multimodal | MMIE / UniM | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2410.10139) [![arXiv](https://img.shields.io/badge/arXiv-UniM-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2603.05075) | Structured evaluation beyond text-only outputs. |
| Agentic visual search | InterLV-Search | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2605.07510) | Repeated evidence seeking and cross-step integration. |
| Vision-centric deep reasoning | Agent-X | [![arXiv](https://img.shields.io/badge/arXiv-Paper-B31B1B?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2505.24876) [![GitHub](https://img.shields.io/badge/GitHub-Code-181717?logo=github&logoColor=white)](https://github.com/mbzuai-oryx/Agent-X) | Step-level reasoning and tool-use assessment. |

[Back to top](#top)

## Skills and Tooling

### Core Reference Repositories

| Repository | Links | Why It Is Useful |
| --- | --- | --- |
| Evolving Visual Generation | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EvolvingLMMs-Lab/Evolving-Visual-Generation) | Strongest living resource hub on the visual-generation side. |
| awesome-gpt-image-2 | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/freestylefly/awesome-gpt-image-2) | Polished prompt-as-code system and reusable visual style library. |
| gpt_image_2_skill | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/wuyoscar/gpt_image_2_skill) | Compact image-generation skill with examples and CLI usage. |

### Install: `awesome-gpt-image-2` Skill

```bash
npx --yes skills@latest add freestylefly/awesome-gpt-image-2 \
  --skill gpt-image-2-style-library \
  --agent codex \
  --copy
```

### Install: `gpt_image_2_skill` for Codex

```text
$skill-installer
Install this skill from GitHub:
https://github.com/wuyoscar/gpt_image_2_skill/tree/main/skills/gpt-image
```

### Open-Source Toolchains Worth Installing

| Tool | Type | Links | Best For |
| --- | --- | --- | --- |
| lmms-eval | evaluation toolkit | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EvolvingLMMs-Lab/lmms-eval) | Unified multimodal evaluation across image, video, audio, and chat-style interfaces. |
| OmniParser | GUI parsing | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/microsoft/OmniParser) | Converting screenshots into interactable regions and semantics for vision-only GUI agents. |
| UI-TARS-desktop | native desktop agent stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/bytedance/UI-TARS-desktop) | End-to-end desktop operator workflows and GUI-agent experimentation. |
| Agent-S | computer-use framework | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/simular-ai/Agent-S) | Hierarchical computer-use flows with memory and planning. |
| OpenVLA | embodied VLA stack | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/openvla/openvla) | Open VLA fine-tuning, evaluation, and robotics experiments. |
| AndroidWorld | benchmark environment | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/google-research/android_world) | Android control agents with dynamic task instantiation. |
| OSWorld | desktop benchmark environment | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/xlang-ai/OSWorld) | Real-computer evaluation loop for GUI agents and operator-style systems. |

### Tool Selection by Workflow

| Workflow | Recommended Stack |
| --- | --- |
| Visual-generation prototyping | `awesome-gpt-image-2` + `gpt_image_2_skill` + `Qwen-Image` style prompting |
| GUI grounding and action | `OmniParser` + `UI-TARS-desktop` + `Agent-S` |
| Benchmark-heavy visual-agent research | `lmms-eval` + `OSWorld` + `AndroidWorld` + `VisualWebArena` |
| Embodied visual agents | `OpenVLA` + simulation / benchmark stack from the relevant VLA papers |

[Back to top](#top)

## Blogs and Deep Dives

This section prioritizes durable technical writeups over hype posts.

### English

| Resource | Links | Focus |
| --- | --- | --- |
| OpenAI: Computer-Using Agent | [OpenAI](https://openai.com/index/computer-using-agent/) | Product and research framing for computer-use agents. |
| OpenAI API: Computer Use Guide | [OpenAI Docs](https://platform.openai.com/docs/guides/tools-computer-use) | Developer-facing usage guide for computer-use workflows. |
| Anthropic: Developing a Computer Use Model | [Anthropic](https://www.anthropic.com/news/developing-computer-use) | One of the best public engineering writeups on GUI-agent development. |
| Anthropic: Introducing computer use | [Anthropic](https://www.anthropic.com/news/3-5-models-and-computer-use) | Concise launch overview plus deployment framing. |
| Google DeepMind: Gemini Robotics brings AI into the physical world | [DeepMind](https://deepmind.google/blog/gemini-robotics-brings-ai-into-the-physical-world/) | Frontier industry view on VLA systems. |
| Google DeepMind: Gemini Robotics On-Device | [DeepMind](https://deepmind.google/discover/blog/gemini-robotics-on-device-brings-ai-to-local-robotic-devices/) | Practical view on low-latency on-device VLA deployment. |
| Qwen Blog: Qwen-Image | [Qwen](https://qwenlm.github.io/blog/qwen-image/) | Official explainer for text rendering and visual-generation capabilities. |
| Roboflow: Vision-Language-Action Models for Robotics | [Roboflow](https://blog.roboflow.com/vision-language-action-models/) | Practical engineering-oriented VLA overview. |

### Chinese

| Resource | Links | Focus |
| --- | --- | --- |
| Qwen-Image Blog | [Qwen](https://qwenlm.github.io/blog/qwen-image/) | Text rendering, posters, PPT, and infographic generation. |
| ModelScope Agent Column | [ModelScope](https://community.modelscope.cn/column/6698a64b7fda170768204e20) | Useful Chinese engineering column tracking agent systems. |
| ModelScope-Agent: multi-strategy and multimodal retrieval | [ModelScope](https://community.modelscope.cn/667a2906f194d31df8b07edd.html) | Practical multimodal retrieval and agent engineering writeup. |
| OmAgent - reinforcement-learning-based multimodal agent | [OM AI Lab](https://om-ai-lab.github.io/2025_07_17_zh.html) | One of the rarer Chinese posts on multimodal agent plus RL practice. |
| MMLab Column at Jiqizhixin | [Jiqizhixin](https://www.jiqizhixin.com/columns/MMLab) | Ongoing Chinese information stream for multimodal vision work. |

### Ongoing Tracking

| Feed | Links | Why Follow It |
| --- | --- | --- |
| Evolving Visual Generation | [GitHub](https://github.com/EvolvingLMMs-Lab/Evolving-Visual-Generation) | Best living list for visual-generation-side developments. |
| lmms-eval releases | [GitHub](https://github.com/EvolvingLMMs-Lab/lmms-eval/blob/main/docs/releases/lmms-eval-0.7.md) | Good proxy for what multimodal evaluation users actually care about. |
| Qwen Blog | [Qwen](https://qwenlm.github.io/blog/) | Strong signal for open multimodal and image-generation releases. |
| OpenEnvision / Awesome-Visual-Agent | [GitHub](https://github.com/OpenEnvision/Awesome-Visual-Agent) | Primary home for the curated visual-agent landscape itself. |

[Back to top](#top)

## Suggested Reading Paths

### Path A: GUI / Computer-Use Agent Builder

1. [SeeClick](https://arxiv.org/abs/2401.10935)
2. [ScreenAI](https://arxiv.org/abs/2402.04615)
3. [Ferret-UI](https://arxiv.org/abs/2404.05719)
4. [OmniParser](https://arxiv.org/abs/2408.00203)
5. [VisualWebArena](https://arxiv.org/abs/2401.13649)
6. [OSWorld](https://arxiv.org/abs/2404.07972)
7. [UI-TARS](https://arxiv.org/abs/2501.12326)
8. [Agent S2](https://arxiv.org/abs/2504.00906)
9. [UI-Copilot](https://arxiv.org/abs/2604.13822)
10. [OS-Symphony](https://arxiv.org/abs/2601.07779)

### Path B: Visual Generation and Interleaved Multimodality

1. [MiniGPT-5](https://arxiv.org/abs/2310.02239)
2. [Show-o](https://arxiv.org/abs/2408.12528)
3. [Janus](https://arxiv.org/abs/2410.13848)
4. [Emu3](https://arxiv.org/abs/2409.18869)
5. [ARMOR v0.1](https://arxiv.org/abs/2503.06542)
6. [DuoGen](https://arxiv.org/abs/2602.00508)
7. [VisionCreator](https://arxiv.org/abs/2603.02681)
8. [Qwen-Image-2.0](https://arxiv.org/abs/2605.10730)
9. [Visual Generation in the New Era](https://arxiv.org/abs/2604.28185)

### Path C: Embodied Visual Agents / Robotics

1. [RT-2](https://arxiv.org/abs/2307.15818)
2. [OpenVLA](https://arxiv.org/abs/2406.09246)
3. [Magma](https://arxiv.org/abs/2502.13130)
4. [Interleave-VLA](https://arxiv.org/abs/2505.02152)
5. [ChatVLA-2](https://arxiv.org/abs/2505.21906)
6. [StemVLA](https://arxiv.org/abs/2602.23721)
7. [World-Value-Action Model](https://arxiv.org/abs/2604.14732)

[Back to top](#top)

## Related Awesome Repositories

| Repository | Links | Notes |
| --- | --- | --- |
| Awesome Multimodal Modeling | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/OpenEnvision/Awesome-Multimodal-Modeling) | Strong complementary index for broader multimodal modeling beyond visual agents. |
| Evolving Visual Generation | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/EvolvingLMMs-Lab/Evolving-Visual-Generation) | Best companion list for the visual-generation side. |
| Awesome-GUI-Agents | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/ZJU-REAL/Awesome-GUI-Agents) | Very useful cross-check list for fresh GUI grounding, long-horizon automation, and benchmark papers. |
| awesome-gpt-image-2 | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/freestylefly/awesome-gpt-image-2) | High-quality prompt system and skill library for generation workflows. |
| gpt_image_2_skill | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/wuyoscar/gpt_image_2_skill) | Focused image-generation skill and example repository. |
| awesome-ui-agents | [![GitHub](https://img.shields.io/badge/GitHub-Project-181717?logo=github&logoColor=white)](https://github.com/opendilab/awesome-ui-agents) | Useful neighboring list if you want extra depth on UI agents. |

[Back to top](#top)

## Curation Principles

- Prefer papers that define a new capability, benchmark, training recipe, or systems bottleneck.
- Prefer official artifacts whenever possible: paper, code, project page, benchmark, or toolkit.
- Exclude generic vision backbones and broad multimodal foundation models unless they are directly agentic, interleaved, or central to visual-agent workflows.
- Separate `visual understanding`, `visual generation`, `interleaved generation`, `computer use`, and `embodied action` rather than collapsing them into one giant bucket.
- Track fresh work explicitly with dates when the field is moving quickly.
- Include practical tools only when they materially help research, evaluation, or deployment.

[Back to top](#top)

## Contributing

Pull requests are welcome, especially for:

- new `2026+` papers with official code or benchmarks
- missing GUI / VLA / interleaved evaluation environments
- high-quality open-source tools and skill repositories
- stronger structure, cleaner categorization, and better reading paths

When adding an item, please include:

- title
- year
- short note on why it matters
- official paper and, when available, official code
- category placement that matches this taxonomy

[Back to top](#top)

## Acknowledgments

This repository was shaped with direct inspiration from:

- [OpenEnvision/Awesome-Multimodal-Modeling](https://github.com/OpenEnvision/Awesome-Multimodal-Modeling)
- [EvolvingLMMs-Lab/Evolving-Visual-Generation](https://github.com/EvolvingLMMs-Lab/Evolving-Visual-Generation)
- [freestylefly/awesome-gpt-image-2](https://github.com/freestylefly/awesome-gpt-image-2)
- [wuyoscar/gpt_image_2_skill](https://github.com/wuyoscar/gpt_image_2_skill)

They are strong examples of awesome repositories that function as research maps, workflow hubs, and practical entry points rather than simple lists of links.

[Back to top](#top)
