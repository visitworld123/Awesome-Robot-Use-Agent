# Awesome-Robot-Use-Agent

<p align="center">
  <img src="Assets/wordmark-dark.png" alt="Awesome Robot Use Agent" width="500">
</p>

A curated list of research on general-purpose AI agents that perceive, program, and operate robots through tools, interfaces, and reusable skills.

Inspired by Phillip Isola's [Robot-Use Agents](https://web.mit.edu/phillipi/www/writing/robot-use-agents.html). The emphasis is on how general-purpose intelligence can be connected to different robots and how improvements can spread through models, software interfaces, and reusable capabilities.


<p align="center">
  <img src="Assets/architecture.png" alt="High-level architecture of Robot Use Agents: generalist agents, robot interfaces, the physical world, and self-evolution." width="1100">
</p>

## Contents

- [General-Purpose Robot-Use Agents](#general-purpose-robot-use-agents)
- [Self-Evolving Robot Agents](#self-evolving-robot-agents)
- [Embodied Agent Operating Systems and Runtimes](#embodied-agent-operating-systems-and-runtimes)
- [Programming and Spatial Action Interfaces](#programming-and-spatial-action-interfaces)
- [Planning, Skill Orchestration and Memory](#planning-skill-orchestration-and-memory)
- [Language-Native Actions and Cross-Embodiment Transfer](#language-native-actions-and-cross-embodiment-transfer)
- [Infrastructure and Benchmarks](#infrastructure-and-benchmarks)
- [Perspectives and Reports](#perspectives-and-reports)

### General-Purpose Robot-Use Agents

General-purpose models operating robots through reusable harnesses, tools, and visual interfaces.

- Show-Harness: Just a VLM Agent Can Play Robots
  <a href="https://arxiv.org/abs/2609.10522"><img src="https://img.shields.io/badge/arxiv-2609.10522-silver" alt="Paper"></a>
  <a href="https://github.com/showlab/Show-Harness"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/showlab/Show-Harness"><img src="https://img.shields.io/github/stars/showlab/Show-Harness" alt="stars"></a>
  <a href="https://huggingface.co/showlab/Show-Harness-VLMs"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
- VIA: Visual Interface Agent for Robot Control
  <a href="https://arxiv.org/abs/2607.11119"><img src="https://img.shields.io/badge/arxiv-2607.11119-silver" alt="Paper"></a>
- CaP-X: A Framework for Benchmarking and Improving Coding Agents for Robot Manipulation
  <a href="https://arxiv.org/abs/2603.22435"><img src="https://img.shields.io/badge/arxiv-2603.22435-silver" alt="Paper"></a>
  <a href="https://github.com/capgym/cap-x"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/capgym/cap-x"><img src="https://img.shields.io/github/stars/capgym/cap-x" alt="stars"></a>
- Guava: An Effective and Universal Harness for Embodied Manipulation
  <a href="https://arxiv.org/abs/2606.18363"><img src="https://img.shields.io/badge/arxiv-2606.18363-silver" alt="Paper"></a>
- ETA: A New Agentic Paradigm for Embodied Tasks
  <a href="https://arxiv.org/abs/2608.03924"><img src="https://img.shields.io/badge/arxiv-2608.03924-silver" alt="Paper"></a>
  <a href="https://github.com/OpenMOSS/OpenETA"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/OpenMOSS/OpenETA"><img src="https://img.shields.io/github/stars/OpenMOSS/OpenETA" alt="stars"></a>
- Maestro: Orchestrating Robotics Modules with Vision-Language Models for Zero-Shot Generalist Robots
  <a href="https://arxiv.org/abs/2511.00917"><img src="https://img.shields.io/badge/arxiv-2511.00917-silver" alt="Paper"></a>

### Self-Evolving Robot Agents

Systems that turn experience into reusable knowledge, skill programs, improved policies, or validated capability upgrades. Includes human-guided methods and learned-policy precursors where noted.

#### Memory and Knowledge Evolution

- Robo-Cortex: A Self-Evolving Embodied Agent via Dual-Grain Cognitive Memory and Autonomous Knowledge Induction
  <a href="https://arxiv.org/abs/2605.18729"><img src="https://img.shields.io/badge/arxiv-2605.18729-silver" alt="Paper"></a>
- Distilling and Retrieving Generalizable Knowledge for Robot Manipulation via Language Corrections
  <a href="https://arxiv.org/abs/2311.10678"><img src="https://img.shields.io/badge/arxiv-2311.10678-silver" alt="Paper"></a>
  <a href="https://github.com/Stanford-ILIAD/droc"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/Stanford-ILIAD/droc"><img src="https://img.shields.io/github/stars/Stanford-ILIAD/droc" alt="stars"></a>

#### Skill and Program Evolution

- ASPIRE: Agentic /Skills Discovery for Robotics
  <a href="https://arxiv.org/abs/2607.00272"><img src="https://img.shields.io/badge/arxiv-2607.00272-silver" alt="Paper"></a>
  <a href="https://github.com/NVlabs/ASPIRE"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/NVlabs/ASPIRE"><img src="https://img.shields.io/github/stars/NVlabs/ASPIRE" alt="stars"></a>
- Lifelong Robot Library Learning: Bootstrapping Composable and Generalizable Skills for Embodied Control with Language Models
  <a href="https://arxiv.org/abs/2406.18746"><img src="https://img.shields.io/badge/arxiv-2406.18746-silver" alt="Paper"></a>
- Eureka: Human-Level Reward Design via Coding Large Language Models
  <a href="https://arxiv.org/abs/2310.12931"><img src="https://img.shields.io/badge/arxiv-2310.12931-silver" alt="Paper"></a>
  <a href="https://github.com/eureka-research/Eureka"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/eureka-research/Eureka"><img src="https://img.shields.io/github/stars/eureka-research/Eureka" alt="stars"></a>
- DrEureka: Language Model Guided Sim-To-Real Transfer
  <a href="https://arxiv.org/abs/2406.01967"><img src="https://img.shields.io/badge/arxiv-2406.01967-silver" alt="Paper"></a>
  <a href="https://github.com/eureka-research/DrEureka"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/eureka-research/DrEureka"><img src="https://img.shields.io/github/stars/eureka-research/DrEureka" alt="stars"></a>

#### Autonomous Data Collection and Policy Improvement

- RoboClaw: An Agentic Framework for Scalable Long-Horizon Robotic Tasks
  <a href="https://arxiv.org/abs/2603.11558"><img src="https://img.shields.io/badge/arxiv-2603.11558-silver" alt="Paper"></a>
  <a href="https://github.com/RoboClaw-Robotics/RoboClaw"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/RoboClaw-Robotics/RoboClaw"><img src="https://img.shields.io/github/stars/RoboClaw-Robotics/RoboClaw" alt="stars"></a>
- Zero2Skill: Bootstrapping Robot Skills through Autonomous Data Collection, Training, and Deployment
  <a href="https://arxiv.org/abs/2607.14047"><img src="https://img.shields.io/badge/arxiv-2607.14047-silver" alt="Paper"></a>
  <a href="https://github.com/open-gigaai/Zero2Skill"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/open-gigaai/Zero2Skill"><img src="https://img.shields.io/github/stars/open-gigaai/Zero2Skill" alt="stars"></a>
- ENPIRE: Agentic Robot Policy Self-Improvement in the Real World
  <a href="https://arxiv.org/abs/2606.19980"><img src="https://img.shields.io/badge/arxiv-2606.19980-silver" alt="Paper"></a>
- HARBOR: A Harness Framework for Agentic Robot Reinforcement Learning
  <a href="https://arxiv.org/abs/2606.08610"><img src="https://img.shields.io/badge/arxiv-2606.08610-silver" alt="Paper"></a>
- AutoRT: Embodied Foundation Models for Large Scale Orchestration of Robotic Agents
  <a href="https://arxiv.org/abs/2401.12963"><img src="https://img.shields.io/badge/arxiv-2401.12963-silver" alt="Paper"></a>
- Autonomous Improvement of Instruction Following Skills via Foundation Models
  <a href="https://arxiv.org/abs/2407.20635"><img src="https://img.shields.io/badge/arxiv-2407.20635-silver" alt="Paper"></a>
  <a href="https://github.com/rail-berkeley/soar"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/rail-berkeley/soar"><img src="https://img.shields.io/github/stars/rail-berkeley/soar" alt="stars"></a>
- RoboCat: A Self-Improving Generalist Agent for Robotic Manipulation
  <a href="https://arxiv.org/abs/2306.11706"><img src="https://img.shields.io/badge/arxiv-2306.11706-silver" alt="Paper"></a>
- RISE: Self-Improving Robot Policy with Compositional World Model
  <a href="https://arxiv.org/abs/2602.11075"><img src="https://img.shields.io/badge/arxiv-2602.11075-silver" alt="Paper"></a>
  <a href="https://github.com/OpenDriveLab/RISE"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/OpenDriveLab/RISE"><img src="https://img.shields.io/github/stars/OpenDriveLab/RISE" alt="stars"></a>
- AllDayNav: Lifelong Navigation via Real-World Reinforcement Learning
  <a href="https://arxiv.org/abs/2606.10927"><img src="https://img.shields.io/badge/arxiv-2606.10927-silver" alt="Paper"></a>

#### Capability Upgrades and Regression Control

- Learning Without Losing Identity: Capability Evolution for Embodied Agents
  <a href="https://arxiv.org/abs/2604.07799"><img src="https://img.shields.io/badge/arxiv-2604.07799-silver" alt="Paper"></a>
  <a href="https://github.com/s20sc/capability-evolution"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/s20sc/capability-evolution"><img src="https://img.shields.io/github/stars/s20sc/capability-evolution" alt="stars"></a>
- Governed Capability Evolution: Lifecycle-Time Compatibility Checking and Rollback for AI-Component-Based Systems, with Embodied Agents as Case Study
  <a href="https://arxiv.org/abs/2604.08059"><img src="https://img.shields.io/badge/arxiv-2604.08059-silver" alt="Paper"></a>
  <a href="https://github.com/s20sc/governed-capability-evolution"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/s20sc/governed-capability-evolution"><img src="https://img.shields.io/github/stars/s20sc/governed-capability-evolution" alt="stars"></a>

Related system-level memory and learning mechanisms: [PhyAgentOS, ABot-Claw, and WCM](#embodied-agent-operating-systems-and-runtimes). Execution-time recovery methods are listed under [Planning, Skill Orchestration and Memory](#planning-skill-orchestration-and-memory).

### Embodied Agent Operating Systems and Runtimes

Persistent embodied-agent systems that organize robot capabilities, state, resources, execution checks, and feedback across tasks or robots.

- PhyAgentOS: A Self-Evolving Operating System for Embodied Agents with Decoupled Cognitive Planning and Physical Execution
  <a href="https://arxiv.org/abs/2607.16636"><img src="https://img.shields.io/badge/arxiv-2607.16636-silver" alt="Paper"></a>
  <a href="https://github.com/PhyAgentOS/PhyAgentOS-core"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/PhyAgentOS/PhyAgentOS-core"><img src="https://img.shields.io/github/stars/PhyAgentOS/PhyAgentOS-core" alt="stars"></a>
- RoboOS: A Hierarchical Embodied Framework for Cross-Embodiment and Multi-Agent Collaboration
  <a href="https://arxiv.org/abs/2505.03673"><img src="https://img.shields.io/badge/arxiv-2505.03673-silver" alt="Paper"></a>
  <a href="https://github.com/FlagOpen/RoboOS"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/FlagOpen/RoboOS"><img src="https://img.shields.io/github/stars/FlagOpen/RoboOS" alt="stars"></a>
- ROSClaw: An OpenClaw ROS 2 Framework for Agentic Robot Control and Interaction
  <a href="https://arxiv.org/abs/2603.26997"><img src="https://img.shields.io/badge/arxiv-2603.26997-silver" alt="Paper"></a>
- ABot-Claw: A Foundation for Persistent, Cooperative, and Self-Evolving Robotic Agents
  <a href="https://arxiv.org/abs/2604.10096"><img src="https://img.shields.io/badge/arxiv-2604.10096-silver" alt="Paper"></a>
  <a href="https://github.com/amap-cvlab/ABot-Claw"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/amap-cvlab/ABot-Claw"><img src="https://img.shields.io/github/stars/amap-cvlab/ABot-Claw" alt="stars"></a>
- AEROS: A Single-Agent Operating Architecture with Embodied Capability Modules
  <a href="https://arxiv.org/abs/2604.07039"><img src="https://img.shields.io/badge/arxiv-2604.07039-silver" alt="Paper"></a>
  <a href="https://github.com/s20sc/aeros"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/s20sc/aeros"><img src="https://img.shields.io/github/stars/s20sc/aeros" alt="stars"></a>
- HoloAgent-0: A Unified Embodied Agent Framework with 3D Spatial Memory
  <a href="https://arxiv.org/abs/2606.23565"><img src="https://img.shields.io/badge/arxiv-2606.23565-silver" alt="Paper"></a>
  <a href="https://github.com/HorizonRobotics/HoloAgent"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/HorizonRobotics/HoloAgent"><img src="https://img.shields.io/github/stars/HorizonRobotics/HoloAgent" alt="stars"></a>
- EmbodiedSkills: A Unified Framework for Orchestrating, Training, and Deploying VLA Agents
  <a href="https://arxiv.org/abs/2609.01281"><img src="https://img.shields.io/badge/arxiv-2609.01281-silver" alt="Paper"></a>
- WCM: World-Cognition Model for Generalizable Human-Robot Interaction
  <a href="https://arxiv.org/abs/2607.22999"><img src="https://img.shields.io/badge/arxiv-2607.22999-silver" alt="Paper"></a>
- EMOS: Embodiment-aware Heterogeneous Multi-robot Operating System with LLM Agents
  <a href="https://arxiv.org/abs/2410.22662"><img src="https://img.shields.io/badge/arxiv-2410.22662-silver" alt="Paper"></a>
  <a href="https://github.com/SgtVincent/EMOS"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/SgtVincent/EMOS"><img src="https://img.shields.io/github/stars/SgtVincent/EMOS" alt="stars"></a>

### Programming and Spatial Action Interfaces

Code, visual prompts, geometric constraints, and other interfaces that connect model reasoning to robot execution.

- Code as Policies: Language Model Programs for Embodied Control
  <a href="https://arxiv.org/abs/2209.07753"><img src="https://img.shields.io/badge/arxiv-2209.07753-silver" alt="Paper"></a>
- ProgPrompt: Generating Situated Robot Task Plans using Large Language Models
  <a href="https://arxiv.org/abs/2209.11302"><img src="https://img.shields.io/badge/arxiv-2209.11302-silver" alt="Paper"></a>
  <a href="https://github.com/NVlabs/progprompt-vh"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/NVlabs/progprompt-vh"><img src="https://img.shields.io/github/stars/NVlabs/progprompt-vh" alt="stars"></a>
- ChatGPT for Robotics: Design Principles and Model Abilities
  <a href="https://arxiv.org/abs/2306.17582"><img src="https://img.shields.io/badge/arxiv-2306.17582-silver" alt="Paper"></a>
- VoxPoser: Composable 3D Value Maps for Robotic Manipulation with Language Models
  <a href="https://arxiv.org/abs/2307.05973"><img src="https://img.shields.io/badge/arxiv-2307.05973-silver" alt="Paper"></a>
  <a href="https://github.com/huangwl18/VoxPoser"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/huangwl18/VoxPoser"><img src="https://img.shields.io/github/stars/huangwl18/VoxPoser" alt="stars"></a>
- ReKep: Spatio-Temporal Reasoning of Relational Keypoint Constraints for Robotic Manipulation
  <a href="https://arxiv.org/abs/2409.01652"><img src="https://img.shields.io/badge/arxiv-2409.01652-silver" alt="Paper"></a>
  <a href="https://github.com/huangwl18/ReKep"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/huangwl18/ReKep"><img src="https://img.shields.io/github/stars/huangwl18/ReKep" alt="stars"></a>
- PIVOT: Iterative Visual Prompting Elicits Actionable Knowledge for VLMs
  <a href="https://arxiv.org/abs/2402.07872"><img src="https://img.shields.io/badge/arxiv-2402.07872-silver" alt="Paper"></a>
- MOKA: Open-World Robotic Manipulation through Mark-Based Visual Prompting
  <a href="https://arxiv.org/abs/2403.03174"><img src="https://img.shields.io/badge/arxiv-2403.03174-silver" alt="Paper"></a>
  <a href="https://github.com/moka-manipulation/moka"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/moka-manipulation/moka"><img src="https://img.shields.io/github/stars/moka-manipulation/moka" alt="stars"></a>
- SoFar: Language-Grounded Orientation Bridges Spatial Reasoning and Object Manipulation
  <a href="https://arxiv.org/abs/2502.13143"><img src="https://img.shields.io/badge/arxiv-2502.13143-silver" alt="Paper"></a>
  <a href="https://github.com/qizekun/SoFar"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/qizekun/SoFar"><img src="https://img.shields.io/github/stars/qizekun/SoFar" alt="stars"></a>
- LangNav: Language as a Perceptual Representation for Navigation
  <a href="https://arxiv.org/abs/2310.07889"><img src="https://img.shields.io/badge/arxiv-2310.07889-silver" alt="Paper"></a>
  <a href="https://github.com/pbw-Berwin/LangNav"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/pbw-Berwin/LangNav"><img src="https://img.shields.io/github/stars/pbw-Berwin/LangNav" alt="stars"></a>
- LM-Nav: Robotic Navigation with Large Pre-Trained Models of Language, Vision, and Action
  <a href="https://arxiv.org/abs/2207.04429"><img src="https://img.shields.io/badge/arxiv-2207.04429-silver" alt="Paper"></a>
- Language to Rewards for Robotic Skill Synthesis
  <a href="https://arxiv.org/abs/2306.08647"><img src="https://img.shields.io/badge/arxiv-2306.08647-silver" alt="Paper"></a>
- Trust the PRoC3S: Solving Long-Horizon Robotics Problems with LLMs and Constraint Satisfaction
  <a href="https://arxiv.org/abs/2406.05572"><img src="https://img.shields.io/badge/arxiv-2406.05572-silver" alt="Paper"></a>

### Planning, Skill Orchestration and Memory

Agents that select and coordinate robot capabilities, track state, verify outcomes, and recover from failures.

- Do As I Can, Not As I Say: Grounding Language in Robotic Affordances
  <a href="https://arxiv.org/abs/2204.01691"><img src="https://img.shields.io/badge/arxiv-2204.01691-silver" alt="Paper"></a>
- Inner Monologue: Embodied Reasoning through Planning with Language Models
  <a href="https://arxiv.org/abs/2207.05608"><img src="https://img.shields.io/badge/arxiv-2207.05608-silver" alt="Paper"></a>
- SayPlan: Grounding Large Language Models using 3D Scene Graphs for Scalable Robot Task Planning
  <a href="https://arxiv.org/abs/2307.06135"><img src="https://img.shields.io/badge/arxiv-2307.06135-silver" alt="Paper"></a>
- CoPAL: Corrective Planning of Robot Actions with Large Language Models
  <a href="https://arxiv.org/abs/2310.07263"><img src="https://img.shields.io/badge/arxiv-2310.07263-silver" alt="Paper"></a>
- RoboStream: Weaving Spatio-Temporal Reasoning with Memory in Vision-Language Models for Robotics
  <a href="https://arxiv.org/abs/2603.12939"><img src="https://img.shields.io/badge/arxiv-2603.12939-silver" alt="Paper"></a>
- Towards the Harness of Embodied Agents
  <a href="https://arxiv.org/abs/2608.11246"><img src="https://img.shields.io/badge/arxiv-2608.11246-silver" alt="Paper"></a>
  <a href="https://github.com/EIT-HAI/Thea"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/EIT-HAI/Thea"><img src="https://img.shields.io/github/stars/EIT-HAI/Thea" alt="stars"></a>
- Harness VLA: Steering Frozen VLAs into Reliable Manipulation Primitives via Memory-Guided Agents
  <a href="https://arxiv.org/abs/2607.08448"><img src="https://img.shields.io/badge/arxiv-2607.08448-silver" alt="Paper"></a>
- Hi Robot: Open-Ended Instruction Following with Hierarchical Vision-Language-Action Models
  <a href="https://arxiv.org/abs/2502.19417"><img src="https://img.shields.io/badge/arxiv-2502.19417-silver" alt="Paper"></a>
- Being-0: A Humanoid Robotic Agent with Vision-Language Models and Modular Skills
  <a href="https://arxiv.org/abs/2503.12533"><img src="https://img.shields.io/badge/arxiv-2503.12533-silver" alt="Paper"></a>
- Agentic Robot: A Brain-Inspired Framework for Vision-Language-Action Models in Embodied Agents
  <a href="https://arxiv.org/abs/2505.23450"><img src="https://img.shields.io/badge/arxiv-2505.23450-silver" alt="Paper"></a>
- RoCo: Dialectic Multi-Robot Collaboration with Large Language Models
  <a href="https://arxiv.org/abs/2307.04738"><img src="https://img.shields.io/badge/arxiv-2307.04738-silver" alt="Paper"></a>
  <a href="https://github.com/MandiZhao/robot-collab"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/MandiZhao/robot-collab"><img src="https://img.shields.io/github/stars/MandiZhao/robot-collab" alt="stars"></a>
- SMART-LLM: Smart Multi-Agent Robot Task Planning using Large Language Models
  <a href="https://arxiv.org/abs/2309.10062"><img src="https://img.shields.io/badge/arxiv-2309.10062-silver" alt="Paper"></a>
  <a href="https://github.com/SMARTlab-Purdue/SMART-LLM"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/SMARTlab-Purdue/SMART-LLM"><img src="https://img.shields.io/github/stars/SMARTlab-Purdue/SMART-LLM" alt="stars"></a>
- MOSAIC: Modular Foundation Models for Assistive and Interactive Cooking
  <a href="https://arxiv.org/abs/2402.18796"><img src="https://img.shields.io/badge/arxiv-2402.18796-silver" alt="Paper"></a>
- REFLECT: Summarizing Robot Experiences for Failure Explanation and Correction
  <a href="https://arxiv.org/abs/2306.15724"><img src="https://img.shields.io/badge/arxiv-2306.15724-silver" alt="Paper"></a>
  <a href="https://github.com/real-stanford/reflect"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/real-stanford/reflect"><img src="https://img.shields.io/github/stars/real-stanford/reflect" alt="stars"></a>
- DoReMi: Grounding Language Model by Detecting and Recovering from Plan-Execution Misalignment
  <a href="https://arxiv.org/abs/2307.00329"><img src="https://img.shields.io/badge/arxiv-2307.00329-silver" alt="Paper"></a>
- AHA: A Vision-Language-Model for Detecting and Reasoning Over Failures in Robotic Manipulation
  <a href="https://arxiv.org/abs/2410.00371"><img src="https://img.shields.io/badge/arxiv-2410.00371-silver" alt="Paper"></a>
  <a href="https://github.com/NVlabs/AHA"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/NVlabs/AHA"><img src="https://img.shields.io/github/stars/NVlabs/AHA" alt="stars"></a>


### Language-Native Actions and Cross-Embodiment Transfer

Related learned-policy methods that preserve language interfaces or reduce adaptation to new embodiments; these generally involve robotics training.

- Actions as Language: Fine-Tuning VLMs into VLAs Without Catastrophic Forgetting
  <a href="https://arxiv.org/abs/2509.22195"><img src="https://img.shields.io/badge/arxiv-2509.22195-silver" alt="Paper"></a>
- LAP: Language-Action Pre-Training Enables Zero-shot Cross-Embodiment Transfer
  <a href="https://arxiv.org/abs/2602.10556"><img src="https://img.shields.io/badge/arxiv-2602.10556-silver" alt="Paper"></a>
  <a href="https://github.com/lihzha/lap"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/lihzha/lap"><img src="https://img.shields.io/github/stars/lihzha/lap" alt="stars"></a>
  <a href="https://huggingface.co/lihzha/LAP-3B"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
- VLA-0: Building State-of-the-Art VLAs with Zero Modification
  <a href="https://arxiv.org/abs/2510.13054"><img src="https://img.shields.io/badge/arxiv-2510.13054-silver" alt="Paper"></a>
  <a href="https://github.com/NVlabs/vla0"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/NVlabs/vla0"><img src="https://img.shields.io/github/stars/NVlabs/vla0" alt="stars"></a>
- LLARVA: Vision-Action Instruction Tuning Enhances Robot Learning
  <a href="https://arxiv.org/abs/2406.11815"><img src="https://img.shields.io/badge/arxiv-2406.11815-silver" alt="Paper"></a>
  <a href="https://github.com/Dantong88/LLARVA"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/Dantong88/LLARVA"><img src="https://img.shields.io/github/stars/Dantong88/LLARVA" alt="stars"></a>
- LLaRA: Supercharging Robot Learning Data for Vision-Language Policy
  <a href="https://arxiv.org/abs/2406.20095"><img src="https://img.shields.io/badge/arxiv-2406.20095-silver" alt="Paper"></a>
  <a href="https://github.com/LostXine/LLaRA"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/LostXine/LLaRA"><img src="https://img.shields.io/github/stars/LostXine/LLaRA" alt="stars"></a>
- CLAP: Direct VLM-to-VLA Adaptation via Language-Action Grounding
  <a href="https://arxiv.org/abs/2607.08974"><img src="https://img.shields.io/badge/arxiv-2607.08974-silver" alt="Paper"></a>
- RT-H: Action Hierarchies Using Language
  <a href="https://arxiv.org/abs/2403.01823"><img src="https://img.shields.io/badge/arxiv-2403.01823-silver" alt="Paper"></a>
- RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control
  <a href="https://arxiv.org/abs/2307.15818"><img src="https://img.shields.io/badge/arxiv-2307.15818-silver" alt="Paper"></a>
- In-Context World Modeling for Robotic Control
  <a href="https://arxiv.org/abs/2606.26025"><img src="https://img.shields.io/badge/arxiv-2606.26025-silver" alt="Paper"></a>

### Infrastructure and Benchmarks

Robot integration, deployment, latency, runtime reliability, and evaluation of model-plus-interface systems.

- Enabling Novel Mission Operations and Interactions with ROSA: The Robot Operating System Agent
  <a href="https://arxiv.org/abs/2410.06472"><img src="https://img.shields.io/badge/arxiv-2410.06472-silver" alt="Paper"></a>
  <a href="https://github.com/nasa-jpl/rosa"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/nasa-jpl/rosa"><img src="https://img.shields.io/github/stars/nasa-jpl/rosa" alt="stars"></a>
- SPINE: Bridging the Cyber-Physical Gap with Agentic AI
  <a href="https://arxiv.org/abs/2607.13049"><img src="https://img.shields.io/badge/arxiv-2607.13049-silver" alt="Paper"></a>
- Harness Engineering for Physical AI: Robot Middleware Is the Harness Layer
  <a href="https://arxiv.org/abs/2606.09416"><img src="https://img.shields.io/badge/arxiv-2606.09416-silver" alt="Paper"></a>
- Reducing Latency in LLM-Based Natural Language Commands Processing for Robot Navigation
  <a href="https://arxiv.org/abs/2506.00075"><img src="https://img.shields.io/badge/arxiv-2506.00075-silver" alt="Paper"></a>
- EmbodiedBench: Comprehensive Benchmarking Multi-modal Large Language Models for Vision-Driven Embodied Agents
  <a href="https://arxiv.org/abs/2502.09560"><img src="https://img.shields.io/badge/arxiv-2502.09560-silver" alt="Paper"></a>
  <a href="https://github.com/EmbodiedBench/EmbodiedBench"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/EmbodiedBench/EmbodiedBench"><img src="https://img.shields.io/github/stars/EmbodiedBench/EmbodiedBench" alt="stars"></a>
  <a href="https://huggingface.co/EmbodiedBench"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
- Embodied Agent Interface: Benchmarking LLMs for Embodied Decision Making
  <a href="https://arxiv.org/abs/2410.07166"><img src="https://img.shields.io/badge/arxiv-2410.07166-silver" alt="Paper"></a>
  <a href="https://github.com/embodied-agent-interface/embodied-agent-interface"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/embodied-agent-interface/embodied-agent-interface"><img src="https://img.shields.io/github/stars/embodied-agent-interface/embodied-agent-interface" alt="stars"></a>
  <a href="https://huggingface.co/datasets/Inevitablevalor/EmbodiedAgentInterface"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
- PARTNR: A Benchmark for Planning and Reasoning in Embodied Multi-agent Tasks
  <a href="https://arxiv.org/abs/2411.00081"><img src="https://img.shields.io/badge/arxiv-2411.00081-silver" alt="Paper"></a>
  <a href="https://github.com/facebookresearch/partnr-planner"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/facebookresearch/partnr-planner"><img src="https://img.shields.io/github/stars/facebookresearch/partnr-planner" alt="stars"></a>
  <a href="https://huggingface.co/datasets/ai-habitat/partnr_episodes"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>

### Perspectives and Reports

These are essays, research blogs, and evaluations; they are listed separately from papers.

- Robot-Use Agents — Phillip Isola, 2026. *Perspective.*
  <a href="https://web.mit.edu/phillipi/www/writing/robot-use-agents.html"><img src="https://img.shields.io/badge/-article-blue" alt="Article"></a>
- Claude plays robotics — Anthropic, 2026. *Research report.*
  <a href="https://www.anthropic.com/research/claude-plays-robotics"><img src="https://img.shields.io/badge/-article-blue" alt="Article"></a>
- Introducing Waddle: agents that control robots — Waddle Labs, 2026. *Research blog / demo.*
  <a href="https://www.waddlelabs.ai/research/introducing-waddle"><img src="https://img.shields.io/badge/-article-blue" alt="Article"></a>
- GPT-6 Astra on robotic manipulation — Robocurve, 2026. *Independent evaluation.*
  <a href="https://openai.robocurve.org/gpt-6-astra/"><img src="https://img.shields.io/badge/-article-blue" alt="Article"></a>
