# Awesome-Robot-Use-Agent

A curated list of research on general-purpose AI agents that perceive, program, and operate robots through tools, interfaces, and reusable skills.

Inspired by Phillip Isola's [Robot-Use Agents](https://web.mit.edu/phillipi/www/writing/robot-use-agents.html). The emphasis is on how general-purpose intelligence can be connected to different robots and how improvements can spread through models, software interfaces, and reusable capabilities.


## Contents

- [General-Purpose Robot-Use Agents](#general-purpose-robot-use-agents)
- [Programming and Spatial Action Interfaces](#programming-and-spatial-action-interfaces)
- [Planning, Skill Orchestration and Memory](#planning-skill-orchestration-and-memory)
- [Agentic Data Collection and Self-Improvement](#agentic-data-collection-and-self-improvement)
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

### Agentic Data Collection and Self-Improvement

Agents that collect data, discover reusable skills, improve programs, or automate robot policy learning.

- RoboClaw: An Agentic Framework for Scalable Long-Horizon Robotic Tasks
  <a href="https://arxiv.org/abs/2603.11558"><img src="https://img.shields.io/badge/arxiv-2603.11558-silver" alt="Paper"></a>
  <a href="https://github.com/RoboClaw-Robotics/RoboClaw"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/RoboClaw-Robotics/RoboClaw"><img src="https://img.shields.io/github/stars/RoboClaw-Robotics/RoboClaw" alt="stars"></a>
- Zero2Skill: Bootstrapping Robot Skills through Autonomous Data Collection, Training, and Deployment
  <a href="https://arxiv.org/abs/2607.14047"><img src="https://img.shields.io/badge/arxiv-2607.14047-silver" alt="Paper"></a>
  <a href="https://github.com/open-gigaai/Zero2Skill"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/open-gigaai/Zero2Skill"><img src="https://img.shields.io/github/stars/open-gigaai/Zero2Skill" alt="stars"></a>
- ASPIRE: Agentic /Skills Discovery for Robotics
  <a href="https://arxiv.org/abs/2607.00272"><img src="https://img.shields.io/badge/arxiv-2607.00272-silver" alt="Paper"></a>
  <a href="https://github.com/NVlabs/ASPIRE"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/NVlabs/ASPIRE"><img src="https://img.shields.io/github/stars/NVlabs/ASPIRE" alt="stars"></a>
- ENPIRE: Agentic Robot Policy Self-Improvement in the Real World
  <a href="https://arxiv.org/abs/2606.19980"><img src="https://img.shields.io/badge/arxiv-2606.19980-silver" alt="Paper"></a>
- HARBOR: A Harness Framework for Agentic Robot Reinforcement Learning
  <a href="https://arxiv.org/abs/2606.08610"><img src="https://img.shields.io/badge/arxiv-2606.08610-silver" alt="Paper"></a>
- AutoRT: Embodied Foundation Models for Large Scale Orchestration of Robotic Agents
  <a href="https://arxiv.org/abs/2401.12963"><img src="https://img.shields.io/badge/arxiv-2401.12963-silver" alt="Paper"></a>
- DrEureka: Language Model Guided Sim-To-Real Transfer
  <a href="https://arxiv.org/abs/2406.01967"><img src="https://img.shields.io/badge/arxiv-2406.01967-silver" alt="Paper"></a>
  <a href="https://github.com/eureka-research/DrEureka"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/eureka-research/DrEureka"><img src="https://img.shields.io/github/stars/eureka-research/DrEureka" alt="stars"></a>
- Eureka: Human-Level Reward Design via Coding Large Language Models
  <a href="https://arxiv.org/abs/2310.12931"><img src="https://img.shields.io/badge/arxiv-2310.12931-silver" alt="Paper"></a>
  <a href="https://github.com/eureka-research/Eureka"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/eureka-research/Eureka"><img src="https://img.shields.io/github/stars/eureka-research/Eureka" alt="stars"></a>

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
