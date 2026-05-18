<a id="top"></a>

# Awesome Visual Agent

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
![Scope](https://img.shields.io/badge/scope-visual%20agents-0f766e)
![Curated](https://img.shields.io/badge/style-curated%2C%20not%20exhaustive-111827)
![Last Checked](https://img.shields.io/badge/checked-2026--05--18-2563eb)

A curated map of visual agents: systems that use visual observations to ground, plan, act, create, or evaluate inside GUIs, browsers, desktops, phones, robots, videos, 3D worlds, or visual-generation workflows.

This list is intentionally selective. It favors papers, benchmarks, and open systems that introduce a concrete agent loop, action space, evaluation environment, data engine, or reliability finding. It does not try to collect every multimodal model, OCR system, captioning model, or prompt-in/image-out generator.

Last checked: 2026-05-18.

## Contents

- [Scope](#scope)
- [Taxonomy](#taxonomy)
- [Curation Rubric](#curation-rubric)
- [Fast Reading Paths](#fast-reading-paths)
- [Recent Highlights](#recent-highlights)
- [Papers](#papers)
  - [Surveys and Landscape](#surveys-and-landscape)
  - [GUI Grounding and Screen Perception](#gui-grounding-and-screen-perception)
  - [Computer-Use Agents and Environments](#computer-use-agents-and-environments)
  - [Embodied Vision-Language-Action Agents](#embodied-vision-language-action-agents)
  - [Agentic Visual Reasoning, Generation, and World Building](#agentic-visual-reasoning-generation-and-world-building)
  - [Safety, Robustness, and Evaluation](#safety-robustness-and-evaluation)
- [Benchmarks and Environments](#benchmarks-and-environments)
- [Builder Resources](#builder-resources)
- [Related Lists](#related-lists)
- [Contributing](#contributing)
- [Curation Notes](#curation-notes)
- [Citation](#citation)

## Scope

Included:

- GUI, web, desktop, and mobile agents that perceive screens and produce executable actions.
- Visual grounding work that is clearly tied to downstream agent control.
- Embodied vision-language-action systems for robot manipulation, navigation, and physical-world interaction.
- Agentic visual reasoning and generation systems with search, planning, memory, tools, critique, or iterative refinement.
- Benchmarks, data engines, simulators, safety suites, and toolchains that make visual agents easier to build or evaluate.

Excluded by default:

- Broad multimodal foundation models with no visual-agent evaluation.
- Generic OCR, captioning, visual question answering, or layout parsing without an action or agent setting.
- Image, video, or 3D generators that are only prompt-in/artifact-out.
- Unverified arXiv IDs, placeholder-looking entries, product rumors, and duplicate rows.

[Back to top](#top)

## Taxonomy

| Track | Core question | Representative starting points |
| --- | --- | --- |
| Screen grounding | Can the model localize text, widgets, controls, and regions well enough to act? | SeeClick, OmniParser, UGround, ScreenSpot-Pro, GUI-Eyes |
| Computer use | Can the agent complete tasks in real websites, desktops, or phones over multiple steps? | WebArena, VisualWebArena, OSWorld, AndroidWorld, Agent S, UI-TARS |
| Embodied VLA | Can visual observations and language be converted into safe physical actions? | RT-2, Open X-Embodiment, OpenVLA, Pi-Zero, Magma |
| Agentic creation | Can the system plan, search, critique, edit, or generate visual artifacts through a loop? | GenArtist, DeepEyes, Agent Banana, VisionCreator, GEMS |
| Reliability and safety | Can we measure brittleness, privacy risk, prompt injection, unsafe actions, and deployment readiness? | VPI-Bench, OpenAgentSafety, OS-BLIND, HazardArena, UI-CUBE |
| Infrastructure | What should builders actually install to train, run, or evaluate visual agents? | BrowserGym, Agent S, Cua, OpenCUA, ScaleCUA, LeRobot |

[Back to top](#top)

## Curation Rubric

An item should usually satisfy at least one of these conditions:

- It defines a new visual-agent capability, benchmark, data engine, training recipe, runtime, or safety evaluation.
- It evaluates closed-loop behavior rather than only static recognition or one-shot generation.
- It is widely used as a baseline, benchmark, dataset, environment, or builder tool.
- It has a stable paper, official code, project page, or documentation that readers can inspect.

An item is removed or left out when the visual-agent connection is weak, the link is unverifiable, the arXiv ID is wrong, the row duplicates a better entry, or the contribution is mostly a product announcement without enough technical detail.

[Back to top](#top)

## Fast Reading Paths

**GUI and computer use.** Start with [SeeClick](https://arxiv.org/abs/2401.10935), [OmniParser](https://arxiv.org/abs/2408.00203), [OSWorld](https://arxiv.org/abs/2404.07972), [UI-TARS](https://arxiv.org/abs/2501.12326), [Agent S2](https://arxiv.org/abs/2504.00906), [OpenCUA](https://arxiv.org/abs/2508.09123), and [UI-Copilot](https://arxiv.org/abs/2604.13822).

**Grounding and perception.** Read [ScreenAI](https://arxiv.org/abs/2402.04615), [Ferret-UI](https://arxiv.org/abs/2404.05719), [UGround](https://arxiv.org/abs/2410.05243), [ScreenSpot-Pro](https://arxiv.org/abs/2504.07981), [GUI-Actor](https://arxiv.org/abs/2506.03143), [Phi-Ground](https://arxiv.org/abs/2507.23779), [GUI-Eyes](https://arxiv.org/abs/2601.09770), and [UI-Zoomer](https://arxiv.org/abs/2604.14113).

**Embodied VLA.** Start with [PaLM-E](https://arxiv.org/abs/2303.03378), [RT-2](https://arxiv.org/abs/2307.15818), [Open X-Embodiment](https://arxiv.org/abs/2310.08864), [OpenVLA](https://arxiv.org/abs/2406.09246), [Pi-Zero](https://arxiv.org/abs/2410.24164), [Magma](https://arxiv.org/abs/2502.13130), and [World-Value-Action](https://arxiv.org/abs/2604.14732).

**Agentic visual creation.** Read [GenArtist](https://arxiv.org/abs/2407.05600), [CIGEval](https://arxiv.org/abs/2504.07046), [DeepEyes](https://arxiv.org/abs/2505.14362), [ImAgent](https://arxiv.org/abs/2511.11483), [GenAgent](https://arxiv.org/abs/2601.18543), [Agent Banana](https://arxiv.org/abs/2602.09084), [VisionCreator](https://arxiv.org/abs/2603.02681), and [GEMS](https://arxiv.org/abs/2603.28088).

[Back to top](#top)

## Recent Highlights

| Work | Date | Why keep it |
| --- | --- | --- |
| [GUI-Eyes](https://arxiv.org/abs/2601.09770) | 2026-01 | Active visual perception for GUI grounding with learned crop/zoom tool use. |
| [ShowUI-Aloha](https://arxiv.org/abs/2601.07181) | 2026-01 | Converts human screen recordings into structured GUI-agent supervision. |
| [OS-Symphony](https://arxiv.org/abs/2601.07779) | 2026-01 | Holistic framework for robust computer-using agents. |
| [ActionEngine](https://arxiv.org/abs/2602.20502) | 2026-02 | Uses state-machine memory to make GUI agents more programmatic and recoverable. |
| [Agent Banana](https://arxiv.org/abs/2602.09084) | 2026-02 | Agentic image editing with planning and tool execution rather than one-shot editing. |
| [SAGE](https://arxiv.org/abs/2602.10116) | 2026-02 | Agentic 3D scene generation for embodied-AI policy training. |
| [CUA-Suite](https://arxiv.org/abs/2603.24440) | 2026-03 | Large human-annotated video demonstrations for computer-use agents. |
| [GEMS](https://arxiv.org/abs/2603.28088) | 2026-03 | Multimodal generation loop with memory, skills, and iterative agent refinement. |
| [UI-Copilot](https://arxiv.org/abs/2604.13822) | 2026-04 | Long-horizon GUI automation with tool-integrated policy optimization. |
| [UI-Zoomer](https://arxiv.org/abs/2604.14113) | 2026-04 | Uncertainty-driven zoom-in for hard GUI grounding cases. |
| [DynamicGUIBench](https://arxiv.org/abs/2604.25380) | 2026-04 | Evaluates GUI agents in high-dynamic interfaces rather than static screenshots. |
| [Video2GUI](https://arxiv.org/abs/2605.14747) | 2026-05 | Synthesizes GUI interaction trajectories from instructional videos. |
| [UI-Verse](https://arxiv.org/abs/2605.02729) | 2026-05 | Studies interface design heuristics that improve computer-use-agent reliability. |
| [Securing Computer-Use Agents](https://arxiv.org/abs/2605.07110) | 2026-05 | Connects CUA architecture, lifecycle, permission scope, and runtime reliability. |

[Back to top](#top)

## Papers

### Surveys and Landscape

| Work | Year | Links | Why keep it |
| --- | --- | --- | --- |
| A Comprehensive Survey of Agents for Computer Use | 2025 | [paper](https://arxiv.org/abs/2501.16150) | Broad map of computer-use-agent domains, agent loops, and evaluation bottlenecks. |
| GUI Agents: A Survey | 2024 | [paper](https://arxiv.org/abs/2412.13501) | Practical survey of GUI-agent architectures, datasets, benchmarks, and failure modes. |
| A Survey on (M)LLM-Based GUI Agents | 2025 | [paper](https://arxiv.org/abs/2504.13865) | Focused entry point for planning, grounding, memory, and GUI-agent evaluation. |
| Towards Trustworthy GUI Agents | 2025 | [paper](https://arxiv.org/abs/2503.23434) | Reliability and safety framing for deployment-facing GUI agents. |
| Large Multimodal Agents: A Survey | 2024 | [paper](https://arxiv.org/abs/2402.15116) | Useful background on LLM-driven multimodal agent components. |
| A Survey on Vision-Language-Action Models for Embodied AI | 2024 | [paper](https://arxiv.org/abs/2405.14093) | Early VLA survey covering embodied perception, planning, and action. |
| Vision-Language-Action in Robotics | 2026 | [paper](https://arxiv.org/abs/2604.23001) | Data-centric survey of VLA datasets, benchmarks, and data engines. |
| Vision-Language-Action Safety | 2026 | [paper](https://arxiv.org/abs/2604.23775) | Focused taxonomy of threats, evaluations, and defenses for VLA systems. |
| Safety in Embodied AI | 2026 | [paper](https://arxiv.org/abs/2605.02900) | Wider safety survey across perception, planning, action, and interaction. |
| Visual Generation in the New Era | 2026 | [paper](https://arxiv.org/abs/2604.28185) | Useful lens for when visual generation becomes agentic world modeling. |
| Securing Computer-Use Agents | 2026 | [paper](https://arxiv.org/abs/2605.07110) | Deployment-grounded view of CUA reliability across architecture, lifecycle, permissions, and oversight. |

[Back to top](#top)

### GUI Grounding and Screen Perception

| Work | Year | Links | Why keep it |
| --- | --- | --- | --- |
| CogAgent | 2023 | [paper](https://arxiv.org/abs/2312.08914), [code](https://github.com/THUDM/CogAgent) | Early high-resolution VLM built explicitly for GUI understanding and navigation. |
| SeeClick | 2024 | [paper](https://arxiv.org/abs/2401.10935), [code](https://github.com/njucckevin/SeeClick) | Shows that GUI grounding is a core bottleneck for visual GUI agents. |
| ScreenAI | 2024 | [paper](https://arxiv.org/abs/2402.04615) | Strong foundation for screen, document, infographic, and layout-heavy visual understanding. |
| Ferret-UI | 2024 | [paper](https://arxiv.org/abs/2404.05719), [code](https://github.com/apple/ml-ferret) | Region-aware mobile UI understanding with explicit grounding. |
| OmniParser | 2024 | [paper](https://arxiv.org/abs/2408.00203), [code](https://github.com/microsoft/OmniParser) | Practical screenshot-to-interactable-region parser for pure-vision GUI agents. |
| UGround | 2024 | [paper](https://arxiv.org/abs/2410.05243), [code](https://github.com/OSU-NLP-Group/UGround) | Strong pure-vision grounding baseline without relying on accessibility trees. |
| OS-ATLAS | 2024 | [paper](https://arxiv.org/abs/2410.23218) | Foundation action model for generalist GUI agents. |
| ShowUI | 2024 | [paper](https://arxiv.org/abs/2411.17465), [code](https://github.com/showlab/ShowUI) | Unifies screenshot-conditioned GUI perception and action modeling. |
| Aguvis | 2024 | [paper](https://arxiv.org/abs/2412.04454) | Pure-vision GUI agent direction with autonomous interface interaction. |
| UI-E2I-Synth | 2025 | [paper](https://arxiv.org/abs/2504.11257) | Synthetic instruction pipeline for scaling GUI grounding supervision. |
| ScreenSpot-Pro | 2025 | [paper](https://arxiv.org/abs/2504.07981) | Hard high-resolution grounding benchmark for professional computer-use screens. |
| GUI-G1 | 2025 | [paper](https://arxiv.org/abs/2505.15810), [code](https://github.com/Yuqi-Zhou/GUI-G1) | Careful analysis of RL pitfalls in GUI grounding. |
| Enhancing Visual Grounding via Self-Evolutionary RL | 2025 | [paper](https://arxiv.org/abs/2505.12370) | Data-efficient RL recipe for high-resolution GUI grounding. |
| GUI-Actor | 2025 | [paper](https://arxiv.org/abs/2506.03143) | Coordinate-free grounding with an action head and verifier. |
| Phi-Ground | 2025 | [paper](https://arxiv.org/abs/2507.23779) | Strong empirical report on training compact GUI grounding models. |
| Test-Time RL for GUI Grounding | 2025 | [paper](https://arxiv.org/abs/2508.05615) | Test-time adaptation using region consistency. |
| Explicit Position-to-Coordinate Mapping | 2025 | [paper](https://arxiv.org/abs/2510.03230) | Addresses coordinate generation as a concrete grounding bottleneck. |
| GUI-Eyes | 2026 | [paper](https://arxiv.org/abs/2601.09770) | Learns when and how to call visual tools such as crop and zoom. |
| UI-Zoomer | 2026 | [paper](https://arxiv.org/abs/2604.14113), [code](https://github.com/ZJU-REAL/UI-Zoomer) | Uses uncertainty to decide where to zoom for GUI grounding. |

[Back to top](#top)

### Computer-Use Agents and Environments

| Work | Year | Links | Why keep it |
| --- | --- | --- | --- |
| Mind2Web | 2023 | [paper](https://arxiv.org/abs/2306.06070) | Foundational benchmark for generalist web agents. |
| Android in the Wild | 2023 | [paper](https://arxiv.org/abs/2307.10088) | Large-scale Android device-control dataset with realistic gestures. |
| WebArena | 2023 | [paper](https://arxiv.org/abs/2307.13854), [code](https://github.com/web-arena-x/webarena) | Realistic web-agent environment with execution-based tasks. |
| SeeAct | 2024 | [paper](https://arxiv.org/abs/2401.01614) | Web agent showing why grounding matters for GPT-4V-style agents. |
| VisualWebArena | 2024 | [paper](https://arxiv.org/abs/2401.13649), [code](https://github.com/web-arena-x/visualwebarena) | Adds visually grounded tasks to realistic web-agent evaluation. |
| WebVoyager | 2024 | [paper](https://arxiv.org/abs/2401.13919) | End-to-end multimodal web agent evaluated on live websites. |
| OmniACT | 2024 | [paper](https://arxiv.org/abs/2402.17553) | Desktop and web benchmark where agents generate executable automation scripts. |
| WorkArena | 2024 | [paper](https://arxiv.org/abs/2403.07718), [code](https://github.com/ServiceNow/WorkArena) | Enterprise workflow benchmark for knowledge-work agents. |
| B-MoCA | 2024 | [paper](https://arxiv.org/abs/2404.16660) | Mobile device-control benchmark across diverse configurations. |
| OSWorld | 2024 | [paper](https://arxiv.org/abs/2404.07972), [code](https://github.com/xlang-ai/OSWorld) | Flagship benchmark for open-ended tasks in real desktop environments. |
| AndroidWorld | 2024 | [paper](https://arxiv.org/abs/2405.14573), [code](https://github.com/google-research/android_world) | Dynamic Android benchmark with broad task diversity. |
| MobileAgentBench | 2024 | [paper](https://arxiv.org/abs/2406.08184) | Practical benchmark for mobile LLM agents. |
| Agent S | 2024 | [paper](https://arxiv.org/abs/2410.08164), [code](https://github.com/simular-ai/Agent-S) | Open agentic framework for using computers through GUI actions. |
| Windows Agent Arena | 2024 | [paper](https://arxiv.org/abs/2409.08264), [code](https://github.com/microsoft/WindowsAgentArena) | Scalable evaluation environment for Windows OS agents. |
| SPA-Bench | 2024 | [paper](https://arxiv.org/abs/2410.15164) | Comprehensive smartphone-agent evaluation benchmark. |
| VideoWebArena | 2024 | [paper](https://arxiv.org/abs/2410.19100) | Long-context video understanding inside web-agent workflows. |
| UI-TARS | 2025 | [paper](https://arxiv.org/abs/2501.12326) | Native GUI-agent model trained for perception, grounding, and action. |
| Agent S2 | 2025 | [paper](https://arxiv.org/abs/2504.00906), [code](https://github.com/simular-ai/Agent-S) | Generalist-specialist framework for computer-use agents. |
| UI-Evol | 2025 | [paper](https://arxiv.org/abs/2505.21964) | Plug-in knowledge-evolution module that improves OSWorld execution reliability for CUAs. |
| ZeroGUI | 2025 | [paper](https://arxiv.org/abs/2505.23762) | Online GUI-agent learning with task generation and reward estimation. |
| OpenCUA | 2025 | [paper](https://arxiv.org/abs/2508.09123), [code](https://github.com/xlang-ai/OpenCUA) | Open foundation stack for computer-use agents. |
| ScaleCUA | 2025 | [paper](https://arxiv.org/abs/2509.15221), [code](https://github.com/OpenGVLab/ScaleCUA) | Cross-platform data scaling for open-source computer-use agents. |
| OmegaUse | 2026 | [paper](https://arxiv.org/abs/2601.20380) | General-purpose GUI agent for autonomous task execution. |
| MemGUI-Bench | 2026 | [paper](https://arxiv.org/abs/2602.06075) | Evaluates memory across mobile GUI sessions and changing environments. |
| OS-Symphony | 2026 | [paper](https://arxiv.org/abs/2601.07779), [code](https://github.com/OS-Copilot/OS-Symphony) | Framework for robust and generalist computer-use agents. |
| ActionEngine | 2026 | [paper](https://arxiv.org/abs/2602.20502) | State-machine memory for more structured GUI automation. |
| UI-Copilot | 2026 | [paper](https://arxiv.org/abs/2604.13822), [code](https://github.com/ZJU-REAL/UI-Copilot) | Long-horizon GUI automation with tool-integrated policy optimization. |
| ClawGUI | 2026 | [paper](https://arxiv.org/abs/2604.11784) | Unified framework for training, evaluating, and deploying GUI agents. |
| DynamicGUIBench | 2026 | [paper](https://arxiv.org/abs/2604.25380) | Stress-tests agents in dynamic, evolving GUI environments. |
| UI-Verse | 2026 | [paper](https://arxiv.org/abs/2605.02729) | Interface-design perspective on making CUAs more reliable. |

[Back to top](#top)

### Embodied Vision-Language-Action Agents

| Work | Year | Links | Why keep it |
| --- | --- | --- | --- |
| PaLM-E | 2023 | [paper](https://arxiv.org/abs/2303.03378) | Embodied multimodal language model connecting visual input to robot tasks. |
| RT-2 | 2023 | [paper](https://arxiv.org/abs/2307.15818) | Canonical VLA model transferring web-scale vision-language knowledge to robot control. |
| Open X-Embodiment / RT-X | 2023 | [paper](https://arxiv.org/abs/2310.08864) | Large robot-learning dataset and RT-X model family. |
| Octo | 2024 | [paper](https://arxiv.org/abs/2405.12213) | Open-source generalist robot policy. |
| OpenVLA | 2024 | [paper](https://arxiv.org/abs/2406.09246), [code](https://github.com/openvla/openvla) | Open-source VLA model and a common baseline for robot manipulation. |
| Pi-Zero | 2024 | [paper](https://arxiv.org/abs/2410.24164) | Flow-based VLA model for general robot control. |
| Magma | 2025 | [paper](https://arxiv.org/abs/2502.13130), [code](https://github.com/microsoft/Magma) | Bridges multimodal agents across digital and physical actions. |
| SafeVLA | 2025 | [paper](https://arxiv.org/abs/2503.03480) | Safety alignment for VLA models via constrained learning. |
| Interleave-VLA | 2025 | [paper](https://arxiv.org/abs/2505.02152) | Robot manipulation with interleaved image-text instructions. |
| ChatVLA-2 | 2025 | [paper](https://arxiv.org/abs/2505.21906) | Open-world embodied reasoning from pretrained knowledge. |
| VLA^2 | 2025 | [paper](https://arxiv.org/abs/2510.14902) | Agentic framework for unseen-concept manipulation. |
| World-Value-Action | 2026 | [paper](https://arxiv.org/abs/2604.14732) | Uses implicit planning and future-state value estimation for VLA systems. |
| SAGE | 2026 | [paper](https://arxiv.org/abs/2602.10116), [code](https://github.com/NVlabs/sage) | Agentically generates simulator-ready 3D scenes for embodied policy training. |

[Back to top](#top)

### Agentic Visual Reasoning, Generation, and World Building

| Work | Year | Links | Why keep it |
| --- | --- | --- | --- |
| GenArtist | 2024 | [paper](https://arxiv.org/abs/2407.05600), [code](https://github.com/zhenyuw16/GenArtist) | MLLM-as-agent for image generation and editing through planning and tool use. |
| CIGEval | 2025 | [paper](https://arxiv.org/abs/2504.07046) | Agentic evaluation framework for conditional image generation. |
| DeepEyes | 2025 | [paper](https://arxiv.org/abs/2505.14362) | Reinforcement learning for active visual reasoning, grounding, and "thinking with images." |
| ImAgent | 2025 | [paper](https://arxiv.org/abs/2511.11483) | Test-time scalable multimodal agent framework for image generation. |
| GenAgent | 2026 | [paper](https://arxiv.org/abs/2601.18543) | Scales text-to-image generation through agentic multimodal reasoning. |
| Mind-Brush | 2026 | [paper](https://arxiv.org/abs/2602.01756) | Adds cognitive search and reasoning loops to image generation. |
| Agent Banana | 2026 | [paper](https://arxiv.org/abs/2602.09084), [code](https://github.com/taco-group/agent-banana) | High-fidelity image editing with planner-executor tooling. |
| M3 | 2026 | [paper](https://arxiv.org/abs/2602.06166) | Multi-modal, multi-agent, multi-round reasoning for high-fidelity text-to-image generation. |
| VisionCreator | 2026 | [paper](https://arxiv.org/abs/2603.02681) | Native visual-generation agentic model with understanding, planning, and creation. |
| Gen-Searcher | 2026 | [paper](https://arxiv.org/abs/2603.28767), [project](https://gen-searcher.vercel.app/) | Reinforces agentic search for image generation. |
| GEMS | 2026 | [paper](https://arxiv.org/abs/2603.28088), [project](https://gems-gen.github.io/) | Multimodal generation with memory, skills, and iterative agent loops. |
| Visual Generation in the New Era | 2026 | [paper](https://arxiv.org/abs/2604.28185) | Helpful taxonomy for agentic world modeling and generation. |

[Back to top](#top)

### Safety, Robustness, and Evaluation

| Work | Year | Links | Why keep it |
| --- | --- | --- | --- |
| AGENTSAFE | 2025 | [paper](https://arxiv.org/abs/2506.14697) | Safety benchmark for embodied agents under hazardous instructions. |
| IS-Bench | 2025 | [paper](https://arxiv.org/abs/2506.16402) | Interactive safety benchmark for VLM-driven household agents. |
| VPI-Bench | 2025 | [paper](https://arxiv.org/abs/2506.02456), [code](https://github.com/boyugou/VPI-Bench) | Visual prompt-injection benchmark for computer-use agents. |
| OpenAgentSafety | 2025 | [paper](https://arxiv.org/abs/2507.06134) | Framework for evaluating real-world agent safety across risk categories. |
| OS-Sentinel | 2025 | [paper](https://arxiv.org/abs/2510.24411) | Hybrid validation for safer mobile GUI agents. |
| UI-CUBE | 2025 | [paper](https://arxiv.org/abs/2511.17131) | Enterprise CUA benchmark that measures operational reliability beyond task accuracy. |
| GUIGuard-Bench | 2026 | [paper](https://arxiv.org/abs/2601.18842) | Privacy-preserving GUI-agent evaluation. |
| CUAAudit | 2026 | [paper](https://arxiv.org/abs/2603.10577) | Tests whether VLMs can audit autonomous computer-use agents. |
| OS-BLIND | 2026 | [paper](https://arxiv.org/abs/2604.10577) | Shows how benign-looking user instructions expose CUA vulnerabilities. |
| HazardArena | 2026 | [paper](https://arxiv.org/abs/2604.12447) | Semantic safety evaluation for VLA systems. |
| RedVLA | 2026 | [paper](https://arxiv.org/abs/2604.22591) | Physical red-teaming benchmark for VLA models. |
| GUI-Perturbed | 2026 | [paper](https://arxiv.org/abs/2604.14262) | Domain-randomization study exposing GUI-grounding brittleness. |
| OS-SPEAR | 2026 | [paper](https://arxiv.org/abs/2604.24348) | Toolkit for safety, performance, efficiency, and robustness analysis of OS agents. |
| ProjGuard | 2026 | [paper](https://arxiv.org/abs/2605.13631) | Safety monitoring for computer-use agents via low-dimensional projections. |

[Back to top](#top)

## Benchmarks and Environments

| Area | Resource | Link | Best used for |
| --- | --- | --- | --- |
| Web | WebArena | [paper](https://arxiv.org/abs/2307.13854), [code](https://github.com/web-arena-x/webarena) | Realistic web navigation with execution-based grading. |
| Web | VisualWebArena | [paper](https://arxiv.org/abs/2401.13649), [code](https://github.com/web-arena-x/visualwebarena) | Visually grounded web tasks where screenshots matter. |
| Web | WorkArena | [paper](https://arxiv.org/abs/2403.07718), [code](https://github.com/ServiceNow/WorkArena) | Enterprise workflow automation in ServiceNow-style environments. |
| Desktop | OSWorld | [paper](https://arxiv.org/abs/2404.07972), [code](https://github.com/xlang-ai/OSWorld) | Open-ended desktop tasks in real operating systems. |
| Desktop | Windows Agent Arena | [paper](https://arxiv.org/abs/2409.08264), [code](https://github.com/microsoft/WindowsAgentArena) | Windows-specific scaling and reproducible OS-agent evaluation. |
| Desktop | OmniACT | [paper](https://arxiv.org/abs/2402.17553) | Evaluating executable automation rather than only low-level clicks. |
| Mobile | AndroidWorld | [paper](https://arxiv.org/abs/2405.14573), [code](https://github.com/google-research/android_world) | Dynamic Android tasks with broad app coverage. |
| Mobile | B-MoCA | [paper](https://arxiv.org/abs/2404.16660) | Mobile control across diverse device configurations. |
| Mobile | MobileAgentBench | [paper](https://arxiv.org/abs/2406.08184) | Efficient mobile-agent evaluation across open-source apps. |
| Mobile | SPA-Bench | [paper](https://arxiv.org/abs/2410.15164) | Smartphone-agent testing with comprehensive task coverage. |
| Grounding | ScreenSpot-Pro | [paper](https://arxiv.org/abs/2504.07981) | High-resolution professional-screen grounding. |
| Memory | MemGUI-Bench | [paper](https://arxiv.org/abs/2602.06075) | Cross-session and cross-temporal mobile GUI memory. |
| Dynamic GUI | DynamicGUIBench | [paper](https://arxiv.org/abs/2604.25380) | Robustness under evolving interfaces and dynamic UI changes. |
| Enterprise reliability | UI-CUBE | [paper](https://arxiv.org/abs/2511.17131) | Deployment-readiness diagnostics beyond simple task success. |
| Security | VPI-Bench | [paper](https://arxiv.org/abs/2506.02456), [code](https://github.com/boyugou/VPI-Bench) | Visual prompt injection for GUI and computer-use agents. |
| Safety | AGENTSAFE | [paper](https://arxiv.org/abs/2506.14697) | Hazardous-instruction safety for embodied agents. |
| Safety | HazardArena | [paper](https://arxiv.org/abs/2604.12447) | Semantic safety evaluation for VLA systems. |
| Embodied | LIBERO | [code](https://github.com/Lifelong-Robot-Learning/LIBERO) | Lifelong robot manipulation tasks. |
| Embodied | RLBench | [code](https://github.com/stepjam/RLBench) | Simulation-based manipulation benchmark. |

[Back to top](#top)

## Builder Resources

### Models, Parsers, and Agent Runtimes

| Resource | Type | Link | Why it is useful |
| --- | --- | --- | --- |
| OmniParser | parser | [GitHub](https://github.com/microsoft/OmniParser) | Converts screenshots into candidate regions for pure-vision GUI agents. |
| ShowUI | GUI model | [GitHub](https://github.com/showlab/ShowUI) | Useful open baseline for screenshot-conditioned GUI action modeling. |
| UI-TARS Desktop | desktop agent | [GitHub](https://github.com/bytedance/UI-TARS-desktop) | Open-source desktop stack for multimodal computer use. |
| Agent S | runtime | [GitHub](https://github.com/simular-ai/Agent-S) | Practical open framework for computer-use agents. |
| BrowserGym | harness | [GitHub](https://github.com/ServiceNow/BrowserGym) | Reusable benchmark and experimentation harness for browser agents. |
| Cua | operator stack | [GitHub](https://github.com/trycua/cua) | Open infrastructure around computer-use-agent execution. |

### Data, Training, and Evaluation Stacks

| Resource | Type | Link | Why it is useful |
| --- | --- | --- | --- |
| OSWorld | environment | [GitHub](https://github.com/xlang-ai/OSWorld) | Standard desktop benchmark and environment. |
| AndroidWorld | environment | [GitHub](https://github.com/google-research/android_world) | Dynamic Android environment for mobile agents. |
| OpenCUA | stack | [GitHub](https://github.com/xlang-ai/OpenCUA) | Open data, models, and evaluation foundations for computer-use agents. |
| ScaleCUA | stack | [GitHub](https://github.com/OpenGVLab/ScaleCUA) | Cross-platform data scaling for open CUA research. |
| CUA-Suite | data suite | [paper](https://arxiv.org/abs/2603.24440) | Large-scale human-annotated video demonstrations for CUA research. |
| ShowUI-Aloha | data pipeline | [paper](https://arxiv.org/abs/2601.07181), [code](https://github.com/showlab/ShowUI) | Converts screen recordings into GUI-agent training data. |
| Video2GUI | data pipeline | [paper](https://arxiv.org/abs/2605.14747) | Synthesizes GUI trajectories from instructional videos. |

### Robotics Tooling

| Resource | Type | Link | Why it is useful |
| --- | --- | --- | --- |
| OpenVLA | model | [GitHub](https://github.com/openvla/openvla) | Common open baseline for VLA robot manipulation. |
| LeRobot | robotics toolkit | [GitHub](https://github.com/huggingface/lerobot) | Practical tooling for robot-learning datasets, training, and policies. |
| LIBERO | robotics benchmark | [GitHub](https://github.com/Lifelong-Robot-Learning/LIBERO) | Widely used manipulation benchmark for lifelong robot learning. |
| RLBench | robotics benchmark | [GitHub](https://github.com/stepjam/RLBench) | Strong simulator benchmark for embodied manipulation. |

[Back to top](#top)

## Related Lists

| Repository | Link | Notes |
| --- | --- | --- |
| Awesome-GUI-Agents | [GitHub](https://github.com/ZJU-REAL/Awesome-GUI-Agents) | Strong companion list for GUI grounding and automation papers. |
| GUI-Agents-Paper-List | [GitHub](https://github.com/OSU-NLP-Group/GUI-Agents-Paper-List) | Systematic paper index focused on GUI agents. |
| awesome-ui-agents | [GitHub](https://github.com/opendilab/awesome-ui-agents) | Useful neighboring list for UI-agent papers and projects. |
| Evolving Visual Generation | [GitHub](https://github.com/EvolvingLMMs-Lab/Evolving-Visual-Generation) | Good adjacent map for visual-generation systems. |
| Awesome Multimodal Modeling | [GitHub](https://github.com/OpenEnvision/Awesome-Multimodal-Modeling) | Broader multimodal modeling list beyond the stricter agent boundary here. |

[Back to top](#top)

## Contributing

Pull requests are welcome when they improve precision rather than volume.

Please include:

- The paper title or project name.
- Official paper, code, project page, or documentation link.
- The best category for the item.
- One sentence explaining the visual-agent loop, benchmark role, or builder value.

Please avoid:

- Generic multimodal model releases with no visual-agent evaluation.
- One-shot generation papers without planning, tools, search, critique, or interaction.
- Duplicate benchmark rows unless the new row adds a distinct environment or protocol.
- Unverified arXiv IDs, placeholder links, and marketing-only announcements.

[Back to top](#top)

## Curation Notes

This repository is curated to stay useful rather than exhaustive:

- Removed rows whose arXiv links resolved to unrelated papers or looked like generated placeholders.
- Removed duplicate tool and benchmark sections that repeated the same entries.
- Removed product-name-only entries without public papers, official technical notes, or stable builder value.
- Removed broad multimodal, OCR, captioning, layout, and image-generation entries unless the work clearly participates in a visual-agent loop.
- Corrected several IDs that were wrong in the previous draft, including Android in the Wild, GUI-G1, and B-MoCA.
- Added higher-fit entries that were missing or underrepresented, including Phi-Ground, Agent S, UI-Evol, ZeroGUI, ScaleCUA, ClawGUI, UI-CUBE, UI-Verse, and several safety benchmarks.

[Back to top](#top)

## Citation

If this list helps your research or engineering work, you can cite it as:

```bibtex
@misc{awesome-visual-agent,
  title        = {Awesome Visual Agent},
  author       = {OpenEnvision and contributors},
  year         = {2026},
  howpublished = {\url{https://github.com/OpenEnvision/Awesome-Visual-Agent}},
  note         = {Curated list of visual-agent papers, benchmarks, and tooling}
}
```

[Back to top](#top)
