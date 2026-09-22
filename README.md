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
- [Reasoning-Acting and Dual-System Architectures](#reasoning-acting-and-dual-system-architectures)
- [Self-Evolving Robot Agents](#self-evolving-robot-agents)
- [Embodied Agent Operating Systems and Runtimes](#embodied-agent-operating-systems-and-runtimes)
- [Programming and Spatial Action Interfaces](#programming-and-spatial-action-interfaces)
- [Planning, Skill Orchestration and Memory](#planning-skill-orchestration-and-memory)
  - [Task Planning, Skill Orchestration and Memory](#task-planning-skill-orchestration-and-memory)
  - [Safe Planning, Verification and Failure Recovery](#safe-planning-verification-and-failure-recovery)
  - [Multi-Robot Coordination](#multi-robot-coordination)
- [Language-Native Actions and Cross-Embodiment Transfer](#language-native-actions-and-cross-embodiment-transfer)
- [Infrastructure and Benchmarks](#infrastructure-and-benchmarks)
- [Perspectives and Reports](#perspectives-and-reports)

### General-Purpose Robot-Use Agents

General-purpose models operating robots through reusable harnesses, tools, and visual interfaces.
- AR-WAM: A Visual-Conditioned Agent-Ready World Action Model for Robotic Manipulation — *Agent-ready manipulation through visual grounding, operation tokens, and `detect` / `execute` / `query` interfaces.*
  <a href="https://arxiv.org/abs/2609.23578"><img src="https://img.shields.io/badge/arxiv-2609.23578-silver" alt="Paper"></a>

- Structured World-State Reasoning for Agentic Robotic Search — *WORLDS maintains a persistent world-state graph and lets agents request, verify, and revise observations before selecting a target.*
  <a href="https://arxiv.org/abs/2609.23841"><img src="https://img.shields.io/badge/arxiv-2609.23841-silver" alt="Paper"></a>
- Transferring the Intelligence of VLMs to Robotic Control — *RoboDawn*
  <a href="https://robodawn.top/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- RoboFind: Multi-Agent Personalized Object Search for People Who Are Blind or Have Low Vision 
  <a href="https://arxiv.org/abs/2609.20330"><img src="https://img.shields.io/badge/arxiv-2609.20330-silver" alt="Paper"></a>

- Navi-Agent: Unlocalized Monocular Navigation Agent — *Previously reported; coordinate-free spatial memory for closed-loop navigation, progress verification and recovery.*
  <a href="https://arxiv.org/abs/2609.20388"><img src="https://img.shields.io/badge/arxiv-2609.20388-silver" alt="Paper"></a>

- In-Context Robot Learning with VLM Agents — *GPT-Policy; in-context adaptation without parameter updates.*
  <a href="https://arxiv.org/abs/2609.19138"><img src="https://img.shields.io/badge/arxiv-2609.19138-silver" alt="Paper"></a>
  <a href="https://cheng-haha.github.io/GPT-Policy/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/cheng-haha/GPT-Policy"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/cheng-haha/GPT-Policy"><img src="https://img.shields.io/github/stars/cheng-haha/GPT-Policy" alt="stars"></a>
- WetRobo: A Reproducible Robot Kit for Coding Agents in Biological Laboratories — *Laboratory robotics.*
  <a href="https://arxiv.org/abs/2609.18435"><img src="https://img.shields.io/badge/arxiv-2609.18435-silver" alt="Paper"></a>
  <a href="https://github.com/tsudalab/WetRobo"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/tsudalab/WetRobo"><img src="https://img.shields.io/github/stars/tsudalab/WetRobo" alt="stars"></a>
- HarnessVLN: Unifying Training-Free Embodied Navigation through an Agent Harness — *Navigation.*
  <a href="https://arxiv.org/abs/2609.15195"><img src="https://img.shields.io/badge/arxiv-2609.15195-silver" alt="Paper"></a>
  <a href="https://agibot-harnessvln.netlify.app/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- EMERGE-Policy: A Robot Mind Emerges Beyond a Single Policy
  <a href="https://arxiv.org/abs/2608.29896"><img src="https://img.shields.io/badge/arxiv-2608.29896-silver" alt="Paper"></a>
  <a href="https://emerge-policy.github.io/EMERGE-Policy/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/EMERGE-Policy/EMERGE-Policy"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/EMERGE-Policy/EMERGE-Policy"><img src="https://img.shields.io/github/stars/EMERGE-Policy/EMERGE-Policy" alt="stars"></a>
- Agent as Policy for Robotic Manipulation
  <a href="https://arxiv.org/abs/2609.12541"><img src="https://img.shields.io/badge/arxiv-2609.12541-silver" alt="Paper"></a>
  <a href="https://agent-as-policy-2026.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://huggingface.co/datasets/Agent-as-Policy/agent-as-policy"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
- Show-Harness: Just a VLM Agent Can Play Robots
  <a href="https://arxiv.org/abs/2609.10522"><img src="https://img.shields.io/badge/arxiv-2609.10522-silver" alt="Paper"></a>
  <a href="https://showlab.github.io/Show-Harness"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/showlab/Show-Harness"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/showlab/Show-Harness"><img src="https://img.shields.io/github/stars/showlab/Show-Harness" alt="stars"></a>
  <a href="https://huggingface.co/showlab/Show-Harness-VLMs"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
  <a href="https://huggingface.co/datasets/showlab/Show-Harness-Data" title="Dataset"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
- VIA: Visual Interface Agent for Robot Control
  <a href="https://arxiv.org/abs/2607.11119"><img src="https://img.shields.io/badge/arxiv-2607.11119-silver" alt="Paper"></a>
  <a href="https://via.hengyuanhu.com/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/hengyuan-hu/via"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/hengyuan-hu/via"><img src="https://img.shields.io/github/stars/hengyuan-hu/via" alt="stars"></a>
- CaP-X: A Framework for Benchmarking and Improving Coding Agents for Robot Manipulation
  <a href="https://arxiv.org/abs/2603.22435"><img src="https://img.shields.io/badge/arxiv-2603.22435-silver" alt="Paper"></a>
  <a href="https://capgym.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/capgym/cap-x"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/capgym/cap-x"><img src="https://img.shields.io/github/stars/capgym/cap-x" alt="stars"></a>
- Guava: An Effective and Universal Harness for Embodied Manipulation
  <a href="https://arxiv.org/abs/2606.18363"><img src="https://img.shields.io/badge/arxiv-2606.18363-silver" alt="Paper"></a>
  <a href="https://guava-harness.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- ETA: A New Agentic Paradigm for Embodied Tasks
  <a href="https://arxiv.org/abs/2608.03924"><img src="https://img.shields.io/badge/arxiv-2608.03924-silver" alt="Paper"></a>
  <a href="https://openmoss.ai/OpenETA/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/OpenMOSS/OpenETA"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/OpenMOSS/OpenETA"><img src="https://img.shields.io/github/stars/OpenMOSS/OpenETA" alt="stars"></a>
- Maestro: Orchestrating Robotics Modules with Vision-Language Models for Zero-Shot Generalist Robots
  <a href="https://arxiv.org/abs/2511.00917"><img src="https://img.shields.io/badge/arxiv-2511.00917-silver" alt="Paper"></a>
  <a href="https://maestro-robot.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>

### Reasoning-Acting and Dual-System Architectures

Architectures that organize reasoning and robot execution through intermediate plans, coupled reasoning and action modules, or adaptive think/act scheduling. Includes learned-policy building blocks and agent-level systems. For author-described System 1 (e.g., Jev-like system) /System 2 models (VLM-like models), fixed-rate and asynchronous coupling are distinguished from adaptive reasoning. Related task-time memory and recovery methods remain under [Planning, Skill Orchestration and Memory](#planning-skill-orchestration-and-memory).

- DSWAM: A Dual-System World Action Foundation Model for Fine-Grained Robot Manipulation — *System 1 WAM execution with an optional System 2 subtask planner; video co-training without future-video generation at inference.*
  <a href="https://arxiv.org/abs/2607.04927"><img src="https://img.shields.io/badge/arxiv-2607.04927-silver" alt="Paper"></a>
  <a href="https://ds-wam.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- Fast-ThinkAct: Efficient Vision-Language-Action Reasoning via Verbalizable Latent Planning — *Preference-guided distillation compresses reasoning into verbalizable latents for action policies; evaluated in simulation and embodied reasoning benchmarks.*
  <a href="https://arxiv.org/abs/2601.09708"><img src="https://img.shields.io/badge/arxiv-2601.09708-silver" alt="Paper"></a>
  <a href="https://jasper0314-huang.github.io/fast-thinkact/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- ThinkAct: Vision-Language-Action Reasoning via Reinforced Visual Latent Planning — *Action-aligned reinforcement learning connects a vision-language reasoner to a diffusion policy through visual plan latents; simulation evaluation.*
  <a href="https://arxiv.org/abs/2507.16815"><img src="https://img.shields.io/badge/arxiv-2507.16815-silver" alt="Paper"></a>
  <a href="https://jasper0314-huang.github.io/thinkact-vla/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- Fast-in-Slow: A Dual-System Foundation Model Unifying Fast Manipulation within Slow Reasoning — *Partially shared System 1/System 2 parameters with asynchronous observations and action generation; simulation and real-robot evaluation.*
  <a href="https://arxiv.org/abs/2506.01953"><img src="https://img.shields.io/badge/arxiv-2506.01953-silver" alt="Paper"></a>
  <a href="https://fast-in-slow.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/CHEN-H01/Fast-in-Slow"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/CHEN-H01/Fast-in-Slow"><img src="https://img.shields.io/github/stars/CHEN-H01/Fast-in-Slow" alt="stars"></a>
- Agentic Robot: A Brain-Inspired Framework for Vision-Language-Action Models in Embodied Agents — *Planner–executor–verifier coordination with subgoal verification and recovery; evaluated on LIBERO.*
  <a href="https://arxiv.org/abs/2505.23450"><img src="https://img.shields.io/badge/arxiv-2505.23450-silver" alt="Paper"></a>
  <a href="https://agentic-robot.github.io"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/Agentic-Robot/agentic-robot"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/Agentic-Robot/agentic-robot"><img src="https://img.shields.io/github/stars/Agentic-Robot/agentic-robot" alt="stars"></a>
- OneTwoVLA: A Unified Vision-Language-Action Model with Adaptive Reasoning — *A unified VLA predicts reasoning or action mode tokens to think at critical moments and otherwise execute action chunks.*
  <a href="https://arxiv.org/abs/2505.11917"><img src="https://img.shields.io/badge/arxiv-2505.11917-silver" alt="Paper"></a>
  <a href="https://one-two-vla.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/Fanqi-Lin/OneTwoVLA"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/Fanqi-Lin/OneTwoVLA"><img src="https://img.shields.io/github/stars/Fanqi-Lin/OneTwoVLA" alt="stars"></a>
- GR00T N1: An Open Foundation Model for Generalist Humanoid Robots — *An Eagle-2 vision-language System 2 conditions a flow-matching System 1 action module, jointly trained across heterogeneous data.*
  <a href="https://arxiv.org/abs/2503.14734"><img src="https://img.shields.io/badge/arxiv-2503.14734-silver" alt="Paper"></a>
  <a href="https://github.com/NVIDIA/Isaac-GR00T/tree/n1-release"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/NVIDIA/Isaac-GR00T"><img src="https://img.shields.io/github/stars/NVIDIA/Isaac-GR00T" alt="stars"></a>
- Hi Robot: Open-Ended Instruction Following with Hierarchical Vision-Language-Action Models — *A high-level VLM guides a low-level VLA through language; planning refreshes periodically and on user feedback.*
  <a href="https://arxiv.org/abs/2502.19417"><img src="https://img.shields.io/badge/arxiv-2502.19417-silver" alt="Paper"></a>
  <a href="https://www.pi.website/research/hirobot"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- Robotic Control via Embodied Chain-of-Thought Reasoning — *ECoT; a VLA reasons about plans, sub-tasks, motion and visually grounded state before predicting robot actions.*
  <a href="https://arxiv.org/abs/2407.08693"><img src="https://img.shields.io/badge/arxiv-2407.08693-silver" alt="Paper"></a>
  <a href="https://embodied-cot.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/MichalZawalski/embodied-CoT"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/MichalZawalski/embodied-CoT"><img src="https://img.shields.io/github/stars/MichalZawalski/embodied-CoT" alt="stars"></a>

### Self-Evolving Robot Agents

Systems that turn experience into reusable knowledge, skill programs, improved policies, or validated capability upgrades. Includes human-guided methods and learned-policy precursors where noted.

#### Memory and Knowledge Evolution
- MessyMem: Learning-from-Doing Memory for Mobile Manipulation
  <a href="https://arxiv.org/abs/2609.15976"><img src="https://img.shields.io/badge/arxiv-2609.15976-silver" alt="Paper"></a>
  <a href="https://messymem.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- Robo-Cortex: A Self-Evolving Embodied Agent via Dual-Grain Cognitive Memory and Autonomous Knowledge Induction
  <a href="https://arxiv.org/abs/2605.18729"><img src="https://img.shields.io/badge/arxiv-2605.18729-silver" alt="Paper"></a>
  <a href="https://robocortex66.github.io/robo-cortex/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- Distilling and Retrieving Generalizable Knowledge for Robot Manipulation via Language Corrections
  <a href="https://arxiv.org/abs/2311.10678"><img src="https://img.shields.io/badge/arxiv-2311.10678-silver" alt="Paper"></a>
  <a href="https://sites.google.com/stanford.edu/droc"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/Stanford-ILIAD/droc"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/Stanford-ILIAD/droc"><img src="https://img.shields.io/github/stars/Stanford-ILIAD/droc" alt="stars"></a>

#### Skill and Program Evolution
- Learning and Transferring Closed-Loop Robot Software — *Coding-agent optimization and reuse of closed-loop robot programs in simulation.*
  <a href="https://arxiv.org/abs/2609.19906"><img src="https://img.shields.io/badge/arxiv-2609.19906-silver" alt="Paper"></a>
- Self-Evolving Embodied Agents via Skill-Harness Evolution — *SHAPER; frozen-model skill and harness optimization.*
  <a href="https://arxiv.org/abs/2608.11350"><img src="https://img.shields.io/badge/arxiv-2608.11350-silver" alt="Paper"></a>
- ASPIRE: Agentic /Skills Discovery for Robotics
  <a href="https://arxiv.org/abs/2607.00272"><img src="https://img.shields.io/badge/arxiv-2607.00272-silver" alt="Paper"></a>
  <a href="https://research.nvidia.com/labs/gear/aspire/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/NVlabs/ASPIRE"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/NVlabs/ASPIRE"><img src="https://img.shields.io/github/stars/NVlabs/ASPIRE" alt="stars"></a>
- Lifelong Robot Library Learning: Bootstrapping Composable and Generalizable Skills for Embodied Control with Language Models
  <a href="https://arxiv.org/abs/2406.18746"><img src="https://img.shields.io/badge/arxiv-2406.18746-silver" alt="Paper"></a>
  <a href="https://gtziafas.github.io/LRLL_project"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- Eureka: Human-Level Reward Design via Coding Large Language Models
  <a href="https://arxiv.org/abs/2310.12931"><img src="https://img.shields.io/badge/arxiv-2310.12931-silver" alt="Paper"></a>
  <a href="https://eureka-research.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/eureka-research/Eureka"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/eureka-research/Eureka"><img src="https://img.shields.io/github/stars/eureka-research/Eureka" alt="stars"></a>
- DrEureka: Language Model Guided Sim-To-Real Transfer
  <a href="https://arxiv.org/abs/2406.01967"><img src="https://img.shields.io/badge/arxiv-2406.01967-silver" alt="Paper"></a>
  <a href="https://eureka-research.github.io/dr-eureka/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/eureka-research/DrEureka"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/eureka-research/DrEureka"><img src="https://img.shields.io/github/stars/eureka-research/DrEureka" alt="stars"></a>

#### Autonomous Data Collection and Policy Improvement
- KnowDemo: Knowledge-Guided Robot Demonstration Generation from Human Videos — *VLM-based task-knowledge extraction for generating diverse, validated robot demonstrations.*
  <a href="https://arxiv.org/abs/2609.21229"><img src="https://img.shields.io/badge/arxiv-2609.21229-silver" alt="Paper"></a>
  <a href="https://zhiyuan-gao.github.io/knowdemo/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- MAGMA-GEN: Validated Recovery Supervision from Ambiguous Failures via Counterfactual Re-Execution — *Simulation-validated recovery data for fine-tuning tool-using robot language policies.*
  <a href="https://arxiv.org/abs/2609.20056"><img src="https://img.shields.io/badge/arxiv-2609.20056-silver" alt="Paper"></a>
  <a href="https://github.com/MAGMA-rob/magma-gen"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/MAGMA-rob/magma-gen"><img src="https://img.shields.io/github/stars/MAGMA-rob/magma-gen" alt="stars"></a>
- RoboClaw: An Agentic Framework for Scalable Long-Horizon Robotic Tasks
  <a href="https://arxiv.org/abs/2603.11558"><img src="https://img.shields.io/badge/arxiv-2603.11558-silver" alt="Paper"></a>
  <a href="https://roboclaw-agibot.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/RoboClaw-Robotics/RoboClaw"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/RoboClaw-Robotics/RoboClaw"><img src="https://img.shields.io/github/stars/RoboClaw-Robotics/RoboClaw" alt="stars"></a>
- Zero2Skill: Bootstrapping Robot Skills through Autonomous Data Collection, Training, and Deployment
  <a href="https://arxiv.org/abs/2607.14047"><img src="https://img.shields.io/badge/arxiv-2607.14047-silver" alt="Paper"></a>
  <a href="https://open-gigaai.github.io/Zero2Skill"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/open-gigaai/Zero2Skill"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/open-gigaai/Zero2Skill"><img src="https://img.shields.io/github/stars/open-gigaai/Zero2Skill" alt="stars"></a>
- ENPIRE: Agentic Robot Policy Self-Improvement in the Real World — *Coding-agent-driven real-world policy and algorithm improvement.*
  <a href="https://arxiv.org/abs/2606.19980"><img src="https://img.shields.io/badge/arxiv-2606.19980-silver" alt="Paper"></a>
  <a href="https://research.nvidia.com/labs/gear/enpire/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/NVlabs/ENPIRE"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/NVlabs/ENPIRE"><img src="https://img.shields.io/github/stars/NVlabs/ENPIRE" alt="stars"></a>
- HARBOR: A Harness Framework for Agentic Robot Reinforcement Learning
  <a href="https://arxiv.org/abs/2606.08610"><img src="https://img.shields.io/badge/arxiv-2606.08610-silver" alt="Paper"></a>
  <a href="https://supersglzc.github.io/harbor-rl/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/supersglzc/harbor-rl"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/supersglzc/harbor-rl"><img src="https://img.shields.io/github/stars/supersglzc/harbor-rl" alt="stars"></a>
- AutoRT: Embodied Foundation Models for Large Scale Orchestration of Robotic Agents
  <a href="https://arxiv.org/abs/2401.12963"><img src="https://img.shields.io/badge/arxiv-2401.12963-silver" alt="Paper"></a>
  <a href="https://auto-rt.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- Autonomous Improvement of Instruction Following Skills via Foundation Models
  <a href="https://arxiv.org/abs/2407.20635"><img src="https://img.shields.io/badge/arxiv-2407.20635-silver" alt="Paper"></a>
  <a href="https://auto-improvement.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/rail-berkeley/soar"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/rail-berkeley/soar"><img src="https://img.shields.io/github/stars/rail-berkeley/soar" alt="stars"></a>
- RoboCat: A Self-Improving Generalist Agent for Robotic Manipulation
  <a href="https://arxiv.org/abs/2306.11706"><img src="https://img.shields.io/badge/arxiv-2306.11706-silver" alt="Paper"></a>
  <a href="https://deepmind.google/blog/robocat-a-self-improving-robotic-agent/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- RISE: Self-Improving Robot Policy with Compositional World Model
  <a href="https://arxiv.org/abs/2602.11075"><img src="https://img.shields.io/badge/arxiv-2602.11075-silver" alt="Paper"></a>
  <a href="https://opendrivelab.com/RISE/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/OpenDriveLab/RISE"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/OpenDriveLab/RISE"><img src="https://img.shields.io/github/stars/OpenDriveLab/RISE" alt="stars"></a>
- AllDayNav: Lifelong Navigation via Real-World Reinforcement Learning
  <a href="https://arxiv.org/abs/2606.10927"><img src="https://img.shields.io/badge/arxiv-2606.10927-silver" alt="Paper"></a>
  <a href="https://bagh2178.github.io/AllDayNav/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>

#### Capability Upgrades and Regression Control

- Learning Without Losing Identity: Capability Evolution for Embodied Agents
  <a href="https://arxiv.org/abs/2604.07799"><img src="https://img.shields.io/badge/arxiv-2604.07799-silver" alt="Paper"></a>
  <a href="https://s20sc.github.io/aeros-project/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/s20sc/capability-evolution"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/s20sc/capability-evolution"><img src="https://img.shields.io/github/stars/s20sc/capability-evolution" alt="stars"></a>
- Governed Capability Evolution: Lifecycle-Time Compatibility Checking and Rollback for AI-Component-Based Systems, with Embodied Agents as Case Study
  <a href="https://arxiv.org/abs/2604.08059"><img src="https://img.shields.io/badge/arxiv-2604.08059-silver" alt="Paper"></a>
  <a href="https://s20sc.github.io/aeros-project/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/s20sc/governed-capability-evolution"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/s20sc/governed-capability-evolution"><img src="https://img.shields.io/github/stars/s20sc/governed-capability-evolution" alt="stars"></a>

Related system-level memory and learning mechanisms: [PhyAgentOS, ABot-Claw, and WCM](#embodied-agent-operating-systems-and-runtimes). Execution-time recovery methods are listed under [Safe Planning, Verification and Failure Recovery](#safe-planning-verification-and-failure-recovery).

### Embodied Agent Operating Systems and Runtimes

Persistent embodied-agent systems that organize robot capabilities, state, resources, execution checks, and feedback across tasks or robots.
- Retriever: Composing the Perception-Reasoning-Action Loop for Long-Horizon Manipulation — *Asynchronous runtime and deterministic replay.*
  <a href="https://arxiv.org/abs/2607.17213"><img src="https://img.shields.io/badge/arxiv-2607.17213-silver" alt="Paper"></a>
  <a href="https://retriever.systems"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/openretriever/retriever"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/openretriever/retriever"><img src="https://img.shields.io/github/stars/openretriever/retriever" alt="stars"></a>
- Harness Robotic OS: A Unified Embodied-Agent Runtime for Closed-Loop Quadruped Inspection
  <a href="https://arxiv.org/abs/2609.11225"><img src="https://img.shields.io/badge/arxiv-2609.11225-silver" alt="Paper"></a>
- PhyAgentOS: A Self-Evolving Operating System for Embodied Agents with Decoupled Cognitive Planning and Physical Execution
  <a href="https://arxiv.org/abs/2607.16636"><img src="https://img.shields.io/badge/arxiv-2607.16636-silver" alt="Paper"></a>
  <a href="https://phy-agent-os.x-era.com/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/PhyAgentOS/PhyAgentOS-core"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/PhyAgentOS/PhyAgentOS-core"><img src="https://img.shields.io/github/stars/PhyAgentOS/PhyAgentOS-core" alt="stars"></a>
- RoboOS: A Hierarchical Embodied Framework for Cross-Embodiment and Multi-Agent Collaboration
  <a href="https://arxiv.org/abs/2505.03673"><img src="https://img.shields.io/badge/arxiv-2505.03673-silver" alt="Paper"></a>
  <a href="https://flagopen.github.io/RoboOS/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
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
  <a href="https://s20sc.github.io/aeros-project/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/s20sc/aeros"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/s20sc/aeros"><img src="https://img.shields.io/github/stars/s20sc/aeros" alt="stars"></a>
- HoloAgent-0: A Unified Embodied Agent Framework with 3D Spatial Memory
  <a href="https://arxiv.org/abs/2606.23565"><img src="https://img.shields.io/badge/arxiv-2606.23565-silver" alt="Paper"></a>
  <a href="https://horizonrobotics.github.io/robot_lab/holoagent/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/HorizonRobotics/HoloAgent"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/HorizonRobotics/HoloAgent"><img src="https://img.shields.io/github/stars/HorizonRobotics/HoloAgent" alt="stars"></a>
- EmbodiedSkills: A Unified Framework for Orchestrating, Training, and Deploying VLA Agents
  <a href="https://arxiv.org/abs/2609.01281"><img src="https://img.shields.io/badge/arxiv-2609.01281-silver" alt="Paper"></a>
  <a href="https://github.com/DCDmllm/EmbodiedSkills"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/DCDmllm/EmbodiedSkills"><img src="https://img.shields.io/github/stars/DCDmllm/EmbodiedSkills" alt="stars"></a>
- WCM: World-Cognition Model for Generalizable Human-Robot Interaction
  <a href="https://arxiv.org/abs/2607.22999"><img src="https://img.shields.io/badge/arxiv-2607.22999-silver" alt="Paper"></a>
- EMOS: Embodiment-aware Heterogeneous Multi-robot Operating System with LLM Agents
  <a href="https://arxiv.org/abs/2410.22662"><img src="https://img.shields.io/badge/arxiv-2410.22662-silver" alt="Paper"></a>
  <a href="https://emos-project.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/SgtVincent/EMOS"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/SgtVincent/EMOS"><img src="https://img.shields.io/github/stars/SgtVincent/EMOS" alt="stars"></a>

### Programming and Spatial Action Interfaces

Code, visual prompts, geometric constraints, and other interfaces that connect model reasoning to robot execution.
- ManiSkillFormer: Demonstration-Free Compositional Manipulation via Task-Conditioned Geometric Contracts
  <a href="https://arxiv.org/abs/2609.16331"><img src="https://img.shields.io/badge/arxiv-2609.16331-silver" alt="Paper"></a>
- AntiGrounding: Executable Robot Trajectories as Visual Prompts for VLM-Guided Manipulation — *VLM selection of executable trajectories through a visual interface and an initialized digital twin.*
  <a href="https://arxiv.org/abs/2506.12374"><img src="https://img.shields.io/badge/arxiv-2506.12374-silver" alt="Paper"></a>
- Auto-HSI: Personalized human control of a robot swarm on demand by using LLMs for online automatic code generation — *Human-in-the-loop interface.*
  <a href="https://arxiv.org/abs/2609.16346"><img src="https://img.shields.io/badge/arxiv-2609.16346-silver" alt="Paper"></a>
- KINO: A Keyframe Interface for VLM Planning and Whole-Body Control in Humanoid Loco-Manipulation — *Learned low-level controller.*
  <a href="https://arxiv.org/abs/2609.18869"><img src="https://img.shields.io/badge/arxiv-2609.18869-silver" alt="Paper"></a>
- AnchorVLN: Geometry-Anchored Vision-Language Grounding Reasoning for Open-Vocabulary Navigation
  <a href="https://arxiv.org/abs/2609.12285"><img src="https://img.shields.io/badge/arxiv-2609.12285-silver" alt="Paper"></a>
  <a href="https://github.com/aryanmangal769/embodied-nav-mcp"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/aryanmangal769/embodied-nav-mcp"><img src="https://img.shields.io/github/stars/aryanmangal769/embodied-nav-mcp" alt="stars"></a>
- GTA-2: A Multi-VLM Framework for Synthesizing Robot Manipulation Skills via Grounded Task Axes
  <a href="https://arxiv.org/abs/2609.09808"><img src="https://img.shields.io/badge/arxiv-2609.09808-silver" alt="Paper"></a>
  <a href="https://gta2-project.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- Evolve Vision-Language-Action Model into an Agent with On-the-fly Tool-use
  <a href="https://arxiv.org/abs/2608.14047"><img src="https://img.shields.io/badge/arxiv-2608.14047-silver" alt="Paper"></a>
- Code as Policies: Language Model Programs for Embodied Control
  <a href="https://arxiv.org/abs/2209.07753"><img src="https://img.shields.io/badge/arxiv-2209.07753-silver" alt="Paper"></a>
  <a href="https://code-as-policies.github.io"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/google-research/google-research/tree/master/code_as_policies"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://huggingface.co/spaces/jackyliang42/code-as-policies" title="Demo"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
- ProgPrompt: Generating Situated Robot Task Plans using Large Language Models
  <a href="https://arxiv.org/abs/2209.11302"><img src="https://img.shields.io/badge/arxiv-2209.11302-silver" alt="Paper"></a>
  <a href="https://progprompt.github.io"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/NVlabs/progprompt-vh"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/NVlabs/progprompt-vh"><img src="https://img.shields.io/github/stars/NVlabs/progprompt-vh" alt="stars"></a>
- ChatGPT for Robotics: Design Principles and Model Abilities
  <a href="https://arxiv.org/abs/2306.17582"><img src="https://img.shields.io/badge/arxiv-2306.17582-silver" alt="Paper"></a>
  <a href="https://www.microsoft.com/en-us/research/articles/chatgpt-for-robotics/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/microsoft/PromptCraft-Robotics"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/microsoft/PromptCraft-Robotics"><img src="https://img.shields.io/github/stars/microsoft/PromptCraft-Robotics" alt="stars"></a>
- VoxPoser: Composable 3D Value Maps for Robotic Manipulation with Language Models
  <a href="https://arxiv.org/abs/2307.05973"><img src="https://img.shields.io/badge/arxiv-2307.05973-silver" alt="Paper"></a>
  <a href="https://voxposer.github.io"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/huangwl18/VoxPoser"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/huangwl18/VoxPoser"><img src="https://img.shields.io/github/stars/huangwl18/VoxPoser" alt="stars"></a>
- ReKep: Spatio-Temporal Reasoning of Relational Keypoint Constraints for Robotic Manipulation
  <a href="https://arxiv.org/abs/2409.01652"><img src="https://img.shields.io/badge/arxiv-2409.01652-silver" alt="Paper"></a>
  <a href="https://rekep-robot.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/huangwl18/ReKep"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/huangwl18/ReKep"><img src="https://img.shields.io/github/stars/huangwl18/ReKep" alt="stars"></a>
- PIVOT: Iterative Visual Prompting Elicits Actionable Knowledge for VLMs
  <a href="https://arxiv.org/abs/2402.07872"><img src="https://img.shields.io/badge/arxiv-2402.07872-silver" alt="Paper"></a>
  <a href="https://pivot-prompt.github.io"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://huggingface.co/spaces/pivot-prompt/pivot-prompt-demo"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
- MOKA: Open-World Robotic Manipulation through Mark-Based Visual Prompting
  <a href="https://arxiv.org/abs/2403.03174"><img src="https://img.shields.io/badge/arxiv-2403.03174-silver" alt="Paper"></a>
  <a href="https://moka-manipulation.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/moka-manipulation/moka"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/moka-manipulation/moka"><img src="https://img.shields.io/github/stars/moka-manipulation/moka" alt="stars"></a>
- SoFar: Language-Grounded Orientation Bridges Spatial Reasoning and Object Manipulation
  <a href="https://arxiv.org/abs/2502.13143"><img src="https://img.shields.io/badge/arxiv-2502.13143-silver" alt="Paper"></a>
  <a href="https://qizekun.github.io/sofar/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/qizekun/SoFar"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/qizekun/SoFar"><img src="https://img.shields.io/github/stars/qizekun/SoFar" alt="stars"></a>
  <a href="https://huggingface.co/collections/qizekun/sofar" title="Collection"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
- LangNav: Language as a Perceptual Representation for Navigation
  <a href="https://arxiv.org/abs/2310.07889"><img src="https://img.shields.io/badge/arxiv-2310.07889-silver" alt="Paper"></a>
  <a href="https://github.com/pbw-Berwin/LangNav"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/pbw-Berwin/LangNav"><img src="https://img.shields.io/github/stars/pbw-Berwin/LangNav" alt="stars"></a>
  <a href="https://huggingface.co/bpan/LangNav-Sim2k-Llama2" title="Model"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
- LM-Nav: Robotic Navigation with Large Pre-Trained Models of Language, Vision, and Action
  <a href="https://arxiv.org/abs/2207.04429"><img src="https://img.shields.io/badge/arxiv-2207.04429-silver" alt="Paper"></a>
  <a href="https://sites.google.com/view/lmnav"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/blazejosinski/lm_nav"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/blazejosinski/lm_nav"><img src="https://img.shields.io/github/stars/blazejosinski/lm_nav" alt="stars"></a>
- Language to Rewards for Robotic Skill Synthesis
  <a href="https://arxiv.org/abs/2306.08647"><img src="https://img.shields.io/badge/arxiv-2306.08647-silver" alt="Paper"></a>
  <a href="https://language-to-reward.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/google-deepmind/language_to_reward_2023"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/google-deepmind/language_to_reward_2023"><img src="https://img.shields.io/github/stars/google-deepmind/language_to_reward_2023" alt="stars"></a>
- Trust the PRoC3S: Solving Long-Horizon Robotics Problems with LLMs and Constraint Satisfaction
  <a href="https://arxiv.org/abs/2406.05572"><img src="https://img.shields.io/badge/arxiv-2406.05572-silver" alt="Paper"></a>
  <a href="https://aidan-curtis.github.io/proc3s.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/Learning-and-Intelligent-Systems/proc3s"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/Learning-and-Intelligent-Systems/proc3s"><img src="https://img.shields.io/github/stars/Learning-and-Intelligent-Systems/proc3s" alt="stars"></a>

### Planning, Skill Orchestration and Memory

Agents that select and coordinate robot capabilities, track state, verify outcomes, and recover from failures.

#### Task Planning, Skill Orchestration and Memory

Task decomposition, reusable skill orchestration, and task-time memory. Includes learned hierarchical planners and action models where applicable.
Cross-cutting reasoning/action coupling and System 1/System 2 designs are listed under [Reasoning-Acting and Dual-System Architectures](#reasoning-acting-and-dual-system-architectures).

- World Action Planner: Generalizable Decision-Making with Action-Conditioned World Models — *VLM action plans are refined through action-conditioned world-model imagination, optimization and search; simulation evaluation.*
  <a href="https://arxiv.org/abs/2607.27599"><img src="https://img.shields.io/badge/arxiv-2607.27599-silver" alt="Paper"></a>
  <a href="https://worldactionplanner.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/XiangchengZhang/world-action-planner"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/XiangchengZhang/world-action-planner"><img src="https://img.shields.io/github/stars/XiangchengZhang/world-action-planner" alt="stars"></a>
- MistyPilot: Enabling Social-Robot Control through Multi-Agent LLM Skill Orchestration — *Natural-language skill orchestration, sensor-event binding, and dialogue-state management on a physical social robot.*
  <a href="https://arxiv.org/abs/2608.15549"><img src="https://img.shields.io/badge/arxiv-2608.15549-silver" alt="Paper"></a>
  <a href="https://wangxiaoshawn.github.io/MistyPilot.html"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/WangXiaoShawn/MistyPilot"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/WangXiaoShawn/MistyPilot"><img src="https://img.shields.io/github/stars/WangXiaoShawn/MistyPilot" alt="stars"></a>
- Bridging Thought and Action: Taming Long-Horizon Instability in Open-Source LLM Agents with a MetaTool-Enhanced ROS Framework
  <a href="https://arxiv.org/abs/2609.13335"><img src="https://img.shields.io/badge/arxiv-2609.13335-silver" alt="Paper"></a>
- 2AM: Grounding Agent-Side Memory as Guidance for Steerable Action Models in Long-Horizon Manipulation
  <a href="https://arxiv.org/abs/2609.11308"><img src="https://img.shields.io/badge/arxiv-2609.11308-silver" alt="Paper"></a>
- Memory as Plans: World-Action Modeling with Memory-Grounded Planning
  <a href="https://arxiv.org/abs/2609.11561"><img src="https://img.shields.io/badge/arxiv-2609.11561-silver" alt="Paper"></a>
  <a href="https://github.com/aipixel/MaP-WAM"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/aipixel/MaP-WAM"><img src="https://img.shields.io/github/stars/aipixel/MaP-WAM" alt="stars"></a>
  <a href="https://sizhezhao.github.io/projects/MaP-WAM/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- Towards Long-horizon Embodied Agents with Tool-Aligned Vision-Language-Action Models
  <a href="https://arxiv.org/abs/2605.13119"><img src="https://img.shields.io/badge/arxiv-2605.13119-silver" alt="Paper"></a>
- Do As I Can, Not As I Say: Grounding Language in Robotic Affordances
  <a href="https://arxiv.org/abs/2204.01691"><img src="https://img.shields.io/badge/arxiv-2204.01691-silver" alt="Paper"></a>
  <a href="https://say-can.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- SayCanPay: Heuristic Planning with Large Language Models using Learnable Domain Knowledge — *Offline action-sequence search; simulation evaluation.*
  <a href="https://arxiv.org/abs/2308.12682"><img src="https://img.shields.io/badge/arxiv-2308.12682-silver" alt="Paper"></a>
  <a href="https://rishihazra.github.io/SayCanPay/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/RishiHazra/saycanpay"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/RishiHazra/saycanpay"><img src="https://img.shields.io/github/stars/RishiHazra/saycanpay" alt="stars"></a>
- Inner Monologue: Embodied Reasoning through Planning with Language Models
  <a href="https://arxiv.org/abs/2207.05608"><img src="https://img.shields.io/badge/arxiv-2207.05608-silver" alt="Paper"></a>
  <a href="https://innermonologue.github.io"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- SayPlan: Grounding Large Language Models using 3D Scene Graphs for Scalable Robot Task Planning
  <a href="https://arxiv.org/abs/2307.06135"><img src="https://img.shields.io/badge/arxiv-2307.06135-silver" alt="Paper"></a>
  <a href="https://sayplan.github.io"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- RoboStream: Weaving Spatio-Temporal Reasoning with Memory in Vision-Language Models for Robotics
  <a href="https://arxiv.org/abs/2603.12939"><img src="https://img.shields.io/badge/arxiv-2603.12939-silver" alt="Paper"></a>
  <a href="https://robostream123.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/yu2hi13/RoboStream"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/yu2hi13/RoboStream"><img src="https://img.shields.io/github/stars/yu2hi13/RoboStream" alt="stars"></a>
- Towards the Harness of Embodied Agents
  <a href="https://arxiv.org/abs/2608.11246"><img src="https://img.shields.io/badge/arxiv-2608.11246-silver" alt="Paper"></a>
  <a href="https://eit-hai.github.io/thea"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/EIT-HAI/Thea"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/EIT-HAI/Thea"><img src="https://img.shields.io/github/stars/EIT-HAI/Thea" alt="stars"></a>
- Harness VLA: Steering Frozen VLAs into Reliable Manipulation Primitives via Memory-Guided Agents
  <a href="https://arxiv.org/abs/2607.08448"><img src="https://img.shields.io/badge/arxiv-2607.08448-silver" alt="Paper"></a>
  <a href="https://harnessvla.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/RLinf/RPent"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/RLinf/RPent"><img src="https://img.shields.io/github/stars/RLinf/RPent" alt="stars"></a>
- Being-0: A Humanoid Robotic Agent with Vision-Language Models and Modular Skills
  <a href="https://arxiv.org/abs/2503.12533"><img src="https://img.shields.io/badge/arxiv-2503.12533-silver" alt="Paper"></a>
  <a href="https://beingbeyond.github.io/Being-0"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/BeingBeyond/Being-0"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/BeingBeyond/Being-0"><img src="https://img.shields.io/github/stars/BeingBeyond/Being-0" alt="stars"></a>
- MOSAIC: Modular Foundation Models for Assistive and Interactive Cooking
  <a href="https://arxiv.org/abs/2402.18796"><img src="https://img.shields.io/badge/arxiv-2402.18796-silver" alt="Paper"></a>
  <a href="https://portal-cornell.github.io/MOSAIC/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>

- Creative Robot Tool Use with Large Language Models — *RoboTool; executable plans over parameterized skills.*
  <a href="https://arxiv.org/abs/2310.13065"><img src="https://img.shields.io/badge/arxiv-2310.13065-silver" alt="Paper"></a>
  <a href="https://creative-robotool.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>

#### Safe Planning, Verification and Failure Recovery

Methods that assess risks, verify execution, and trigger corrective planning or recovery. Failure-recovery benchmarks are listed under [Infrastructure and Benchmarks](#infrastructure-and-benchmarks).
- FRAMES: Failure Recovery And Monitoring of Embodied Skills for Humanoid Loco-Manipulation — *A planner, VLM monitor, recovery agent, and memory module form a failure-aware supervisory loop for humanoid skills.*
  <a href="https://arxiv.org/abs/2609.22538"><img src="https://img.shields.io/badge/arxiv-2609.22538-silver" alt="Paper"></a>
- CommitFlow: Semantic Commitment Verification and Local Correction for Long-Horizon Robot Manipulation VLA Execution — *Frozen-policy execution harness with semantic commitment monitoring, local correction and stage-level verification.*
  <a href="https://arxiv.org/abs/2609.21908"><img src="https://img.shields.io/badge/arxiv-2609.21908-silver" alt="Paper"></a>

- When Should a Failing Robot Ask? Initiating Corrective Human-Robot Dialogue from Audited Sensor Evidence — *Evidence-aware choice between autonomous action, additional sensing and human assistance after failure.*
  <a href="https://arxiv.org/abs/2609.21942"><img src="https://img.shields.io/badge/arxiv-2609.21942-silver" alt="Paper"></a>

- Coding Agents with an Obstacle-Aware Harness for Safe Robot Manipulation — *SafeHarness; obstacle-aware route verification, replanning, and contact execution, evaluated in simulation.*
  <a href="https://arxiv.org/abs/2609.20822"><img src="https://img.shields.io/badge/arxiv-2609.20822-silver" alt="Paper"></a>
- GAVEL: Graph World Models for Verified and Efficient Long-Horizon LLM Task Planning 
  <a href="https://arxiv.org/abs/2609.19315"><img src="https://img.shields.io/badge/arxiv-2609.19315-silver" alt="Paper"></a>
- Safe Task Planning with Long-Term Graph Memory for Embodied Agents
  <a href="https://arxiv.org/abs/2609.08444"><img src="https://img.shields.io/badge/arxiv-2609.08444-silver" alt="Paper"></a>
  <a href="https://sites.google.com/view/safemem"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/lty759/SafeMem"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/lty759/SafeMem"><img src="https://img.shields.io/github/stars/lty759/SafeMem" alt="stars"></a>
- VLA-Corrector: Stage-Aware Observable State Understanding for Prompt-Based Closed-Loop Recovery of Vision-Language-Action Policies
  <a href="https://arxiv.org/abs/2609.06508"><img src="https://img.shields.io/badge/arxiv-2609.06508-silver" alt="Paper"></a>
- CoPAL: Corrective Planning of Robot Actions with Large Language Models
  <a href="https://arxiv.org/abs/2310.07263"><img src="https://img.shields.io/badge/arxiv-2310.07263-silver" alt="Paper"></a>
  <a href="https://hri-eu.github.io/Loom/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/HRI-EU/Loom"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/HRI-EU/Loom"><img src="https://img.shields.io/github/stars/HRI-EU/Loom" alt="stars"></a>
- REFLECT: Summarizing Robot Experiences for Failure Explanation and Correction
  <a href="https://arxiv.org/abs/2306.15724"><img src="https://img.shields.io/badge/arxiv-2306.15724-silver" alt="Paper"></a>
  <a href="https://robot-reflect.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/real-stanford/reflect"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/real-stanford/reflect"><img src="https://img.shields.io/github/stars/real-stanford/reflect" alt="stars"></a>
- DoReMi: Grounding Language Model by Detecting and Recovering from Plan-Execution Misalignment
  <a href="https://arxiv.org/abs/2307.00329"><img src="https://img.shields.io/badge/arxiv-2307.00329-silver" alt="Paper"></a>
  <a href="https://sites.google.com/view/doremi-paper"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- AHA: A Vision-Language-Model for Detecting and Reasoning Over Failures in Robotic Manipulation
  <a href="https://arxiv.org/abs/2410.00371"><img src="https://img.shields.io/badge/arxiv-2410.00371-silver" alt="Paper"></a>
  <a href="https://aha-vlm.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/NVlabs/AHA"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/NVlabs/AHA"><img src="https://img.shields.io/github/stars/NVlabs/AHA" alt="stars"></a>

- Robots That Ask For Help: Uncertainty Alignment for Large Language Model Planners — *KnowNo; calibrated uncertainty and human clarification.*
  <a href="https://arxiv.org/abs/2307.01928"><img src="https://img.shields.io/badge/arxiv-2307.01928-silver" alt="Paper"></a>
  <a href="https://robot-help.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/google-research/google-research/tree/master/language_model_uncertainty"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>

#### Multi-Robot Coordination

Task allocation, communication, and organizational structures for teams of robots or embodied agents. ORCH is evaluated in simulation; system-level runtimes are listed under [Embodied Agent Operating Systems and Runtimes](#embodied-agent-operating-systems-and-runtimes).
- AeroWeaver: An Embodied-Agent Harness for Weaving Aerial Skills into Distributed, Adaptive Swarm Execution — *Simulation.*
  <a href="https://arxiv.org/abs/2609.18520"><img src="https://img.shields.io/badge/arxiv-2609.18520-silver" alt="Paper"></a>
  <a href="https://github.com/Admire-ljb/AeroWeaver"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/Admire-ljb/AeroWeaver"><img src="https://img.shields.io/github/stars/Admire-ljb/AeroWeaver" alt="stars"></a>
- ORCH: Organizational Principles Enable Collective Intelligence in Embodied AI
  <a href="https://arxiv.org/abs/2609.11737"><img src="https://img.shields.io/badge/arxiv-2609.11737-silver" alt="Paper"></a>
- RoCo: Dialectic Multi-Robot Collaboration with Large Language Models
  <a href="https://arxiv.org/abs/2307.04738"><img src="https://img.shields.io/badge/arxiv-2307.04738-silver" alt="Paper"></a>
  <a href="https://project-roco.github.io"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/MandiZhao/robot-collab"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/MandiZhao/robot-collab"><img src="https://img.shields.io/github/stars/MandiZhao/robot-collab" alt="stars"></a>
- SMART-LLM: Smart Multi-Agent Robot Task Planning using Large Language Models
  <a href="https://arxiv.org/abs/2309.10062"><img src="https://img.shields.io/badge/arxiv-2309.10062-silver" alt="Paper"></a>
  <a href="https://sites.google.com/view/smart-llm/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/SMARTlab-Purdue/SMART-LLM"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/SMARTlab-Purdue/SMART-LLM"><img src="https://img.shields.io/github/stars/SMARTlab-Purdue/SMART-LLM" alt="stars"></a>

### Language-Native Actions and Cross-Embodiment Transfer

Related learned-policy methods that preserve language interfaces or reduce adaptation to new embodiments; these generally involve robotics training.

- Actions as Language: Fine-Tuning VLMs into VLAs Without Catastrophic Forgetting
  <a href="https://arxiv.org/abs/2509.22195"><img src="https://img.shields.io/badge/arxiv-2509.22195-silver" alt="Paper"></a>
  <a href="https://vlm2vla.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/irom-princeton/vlm2vla"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/irom-princeton/vlm2vla"><img src="https://img.shields.io/github/stars/irom-princeton/vlm2vla" alt="stars"></a>
  <a href="https://huggingface.co/AasherH/vlm2vla" title="Model"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
- LAP: Language-Action Pre-Training Enables Zero-shot Cross-Embodiment Transfer
  <a href="https://arxiv.org/abs/2602.10556"><img src="https://img.shields.io/badge/arxiv-2602.10556-silver" alt="Paper"></a>
  <a href="https://lap-vla.github.io"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/lihzha/lap"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/lihzha/lap"><img src="https://img.shields.io/github/stars/lihzha/lap" alt="stars"></a>
  <a href="https://huggingface.co/lihzha/LAP-3B"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
  <a href="https://huggingface.co/collections/lihzha/lap" title="Collection"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
- VLA-0: Building State-of-the-Art VLAs with Zero Modification
  <a href="https://arxiv.org/abs/2510.13054"><img src="https://img.shields.io/badge/arxiv-2510.13054-silver" alt="Paper"></a>
  <a href="https://vla0.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/NVlabs/vla0"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/NVlabs/vla0"><img src="https://img.shields.io/github/stars/NVlabs/vla0" alt="stars"></a>
  <a href="https://huggingface.co/ankgoyal/vla0-libero" title="Model"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
- LLARVA: Vision-Action Instruction Tuning Enhances Robot Learning
  <a href="https://arxiv.org/abs/2406.11815"><img src="https://img.shields.io/badge/arxiv-2406.11815-silver" alt="Paper"></a>
  <a href="https://llarva24.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/Dantong88/LLARVA"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/Dantong88/LLARVA"><img src="https://img.shields.io/github/stars/Dantong88/LLARVA" alt="stars"></a>
- LLaRA: Supercharging Robot Learning Data for Vision-Language Policy
  <a href="https://arxiv.org/abs/2406.20095"><img src="https://img.shields.io/badge/arxiv-2406.20095-silver" alt="Paper"></a>
  <a href="https://github.com/LostXine/LLaRA"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/LostXine/LLaRA"><img src="https://img.shields.io/github/stars/LostXine/LLaRA" alt="stars"></a>
  <a href="https://huggingface.co/variante/llava-1.5-7b-llara-D-inBC-Aux-B-VIMA-80k" title="Model"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
- CLAP: Direct VLM-to-VLA Adaptation via Language-Action Grounding
  <a href="https://arxiv.org/abs/2607.08974"><img src="https://img.shields.io/badge/arxiv-2607.08974-silver" alt="Paper"></a>
  <a href="https://omron-sinicx.github.io/clap/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- RT-H: Action Hierarchies Using Language
  <a href="https://arxiv.org/abs/2403.01823"><img src="https://img.shields.io/badge/arxiv-2403.01823-silver" alt="Paper"></a>
  <a href="https://rt-hierarchy.github.io"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control
  <a href="https://arxiv.org/abs/2307.15818"><img src="https://img.shields.io/badge/arxiv-2307.15818-silver" alt="Paper"></a>
  <a href="https://robotics-transformer2.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- In-Context World Modeling for Robotic Control
  <a href="https://arxiv.org/abs/2606.26025"><img src="https://img.shields.io/badge/arxiv-2606.26025-silver" alt="Paper"></a>

### Infrastructure and Benchmarks
Jev+Robot
- robo-jev: A 10 Hz Typed-Decision Layer for Physical Robots — *A System-One-style decision layer that scores typed robot actions, stop conditions, gripper states, paths, speed, and force for a deterministic executor.*
  <a href="https://github.com/STEERIX-home/robo-jev"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/STEERIX-home/robo-jev"><img src="https://img.shields.io/github/stars/STEERIX-home/robo-jev" alt="stars"></a>

- EmbodiedJev: MuJoCo Robot Decision Workbench — *Browser-based MuJoCo and Franka Panda workbench supporting Jev, Claude, OpenAI-compatible APIs, and local MiniCPM models with visible observe–decide–execute–feedback loops.*
  <a href="https://github.com/FBddcz/embodied-jev"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/FBddcz/embodied-jev"><img src="https://img.shields.io/github/stars/FBddcz/embodied-jev" alt="stars"></a>

- RoboJEV: Two-Stage JEV Control of a Franka Panda in MuJoCo — *Two-stage typed decisions for task intent followed by Cartesian motion and gripper commands, evaluated with independent physical success checks.*
  <a href="https://github.com/lykycy123/RoboJEV"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/lykycy123/RoboJEV"><img src="https://img.shields.io/github/stars/lykycy123/RoboJEV" alt="stars"></a>

- Jev Robot Control — *Reproducible xArm7 MuJoCo comparison of Jev, GPT-6 Astra, and GPT-4.1 mini with archived trajectories, offline verification, and replay.*
  <a href="https://github.com/openroboto-ai/jev-robot-control"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/openroboto-ai/jev-robot-control"><img src="https://img.shields.io/github/stars/openroboto-ai/jev-robot-control" alt="stars"></a>


Robot integration, deployment, latency, runtime reliability, and evaluation of model-plus-interface systems. Includes benchmarks for memory, safety, and recovery, as well as surveys of robot policy verification.
- From Rollout to Reset: A Graph-Based Harness for Autonomous Long-Horizon Manipulation Evaluation — *HALTER; scene-graph-based evaluation, reset planning, and reset verification on a physical robot.*
  <a href="https://arxiv.org/abs/2609.19413"><img src="https://img.shields.io/badge/arxiv-2609.19413-silver" alt="Paper"></a>
- VABench: Measuring Embodied Spatial Intelligence through Visual Demonstrations, Active Perception, and Metric Control — *Simulation benchmark for general-purpose MLLMs using active camera control, Cartesian action commands, and execution feedback.*
  <a href="https://arxiv.org/abs/2609.19554"><img src="https://img.shields.io/badge/arxiv-2609.19554-silver" alt="Paper"></a>
  <a href="https://github.com/zhangzhongbo2213/VABench"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/zhangzhongbo2213/VABench"><img src="https://img.shields.io/github/stars/zhangzhongbo2213/VABench" alt="stars"></a>
- Towards Embodied Air-Ground Cooperative Object Search: Benchmark, Dataset and Agentic Method — *AGOS; simulated aerial-ground collaboration.*
  <a href="https://arxiv.org/abs/2609.08402"><img src="https://img.shields.io/badge/arxiv-2609.08402-silver" alt="Paper"></a>
- FluxVLA Engine: A One-Stop VLA Engineering Platform for Embodied Intelligence — *Engineering platform.*
  <a href="https://arxiv.org/abs/2609.17210"><img src="https://img.shields.io/badge/arxiv-2609.17210-silver" alt="Paper"></a>
  <a href="https://github.com/FluxVLA/FluxVLA"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/FluxVLA/FluxVLA"><img src="https://img.shields.io/github/stars/FluxVLA/FluxVLA" alt="stars"></a>
  <a href="https://huggingface.co/limxdynamics/FluxVLAEngine" title="Model"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
  <a href="https://huggingface.co/datasets/limxdynamics/FluxVLAData" title="Dataset"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
- No Free Checker: A Survey of Verifiers for Robot Policies — *Survey.*
  <a href="https://arxiv.org/abs/2609.09250"><img src="https://img.shields.io/badge/arxiv-2609.09250-silver" alt="Paper"></a>
  <a href="https://zjuscl.github.io/Awesome-Robot-Verifier/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/ZJUSCL/Awesome-Robot-Verifier"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/ZJUSCL/Awesome-Robot-Verifier"><img src="https://img.shields.io/github/stars/ZJUSCL/Awesome-Robot-Verifier" alt="stars"></a>
- EvoNav-Bench: Benchmarking Lifelong Navigation in Evolving Environments
  <a href="https://arxiv.org/abs/2609.08292"><img src="https://img.shields.io/badge/arxiv-2609.08292-silver" alt="Paper"></a>
- ReactHuman: A Physics-Grounded Benchmark for Human-Like Reactive Decision-Making in Embodied Multimodal LLMs
  <a href="https://arxiv.org/abs/2609.10895"><img src="https://img.shields.io/badge/arxiv-2609.10895-silver" alt="Paper"></a>
  <a href="https://huggingface.co/datasets/Alan123/reacthuman-benchmark-scaled"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
- MEMOBench: A Process Level Memory Benchmark for Robotic Manipulation
  <a href="https://arxiv.org/abs/2609.07047"><img src="https://img.shields.io/badge/arxiv-2609.07047-silver" alt="Paper"></a>
  <a href="https://github.com/Collab-Gen/MEMOBench"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/Collab-Gen/MEMOBench"><img src="https://img.shields.io/github/stars/Collab-Gen/MEMOBench" alt="stars"></a>
  <a href="https://huggingface.co/datasets/SunSeaLucky/MEMOBench" title="Dataset"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
- LIBERO-RECOVER: Beyond Task Success Towards Failure Recovery in Robotic Manipulation Models
  <a href="https://arxiv.org/abs/2609.05178"><img src="https://img.shields.io/badge/arxiv-2609.05178-silver" alt="Paper"></a>
  <a href="https://liulin815.github.io/LIBERO-Recovery/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/liulin815/LIBERO-Recovery"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/liulin815/LIBERO-Recovery"><img src="https://img.shields.io/github/stars/liulin815/LIBERO-Recovery" alt="stars"></a>
- Enabling Novel Mission Operations and Interactions with ROSA: The Robot Operating System Agent
  <a href="https://arxiv.org/abs/2410.06472"><img src="https://img.shields.io/badge/arxiv-2410.06472-silver" alt="Paper"></a>
  <a href="https://github.com/nasa-jpl/rosa"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/nasa-jpl/rosa"><img src="https://img.shields.io/github/stars/nasa-jpl/rosa" alt="stars"></a>
- RoboScript: Code Generation for Free-Form Manipulation Tasks across Real and Simulation — *ROS-based deployment and code-generation benchmark.*
  <a href="https://arxiv.org/abs/2402.14623"><img src="https://img.shields.io/badge/arxiv-2402.14623-silver" alt="Paper"></a>
- SPINE: Bridging the Cyber-Physical Gap with Agentic AI
  <a href="https://arxiv.org/abs/2607.13049"><img src="https://img.shields.io/badge/arxiv-2607.13049-silver" alt="Paper"></a>
- Harness Engineering for Physical AI: Robot Middleware Is the Harness Layer
  <a href="https://arxiv.org/abs/2606.09416"><img src="https://img.shields.io/badge/arxiv-2606.09416-silver" alt="Paper"></a>
- Reducing Latency in LLM-Based Natural Language Commands Processing for Robot Navigation
  <a href="https://arxiv.org/abs/2506.00075"><img src="https://img.shields.io/badge/arxiv-2506.00075-silver" alt="Paper"></a>
- EmbodiedBench: Comprehensive Benchmarking Multi-modal Large Language Models for Vision-Driven Embodied Agents
  <a href="https://arxiv.org/abs/2502.09560"><img src="https://img.shields.io/badge/arxiv-2502.09560-silver" alt="Paper"></a>
  <a href="https://embodiedbench.github.io"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/EmbodiedBench/EmbodiedBench"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/EmbodiedBench/EmbodiedBench"><img src="https://img.shields.io/github/stars/EmbodiedBench/EmbodiedBench" alt="stars"></a>
  <a href="https://huggingface.co/EmbodiedBench"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
- Embodied Agent Interface: Benchmarking LLMs for Embodied Decision Making
  <a href="https://arxiv.org/abs/2410.07166"><img src="https://img.shields.io/badge/arxiv-2410.07166-silver" alt="Paper"></a>
  <a href="https://embodied-agent-interface.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/embodied-agent-interface/embodied-agent-interface"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/embodied-agent-interface/embodied-agent-interface"><img src="https://img.shields.io/github/stars/embodied-agent-interface/embodied-agent-interface" alt="stars"></a>
  <a href="https://huggingface.co/datasets/Inevitablevalor/EmbodiedAgentInterface"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
- PARTNR: A Benchmark for Planning and Reasoning in Embodied Multi-agent Tasks
  <a href="https://arxiv.org/abs/2411.00081"><img src="https://img.shields.io/badge/arxiv-2411.00081-silver" alt="Paper"></a>
  <a href="https://aihabitat.org/partnr/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
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
- Introducing Auto Engineering for Robotics - General Robotics, 2026. *Blog / demo.*
  <a href="https://www.generalrobotics.company/post/introducing-auto-engineering-for-robotics"><img src="https://img.shields.io/badge/-article-blue" alt="Article"></a>
