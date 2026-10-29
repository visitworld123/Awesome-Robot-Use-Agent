
News: We release a benchmark to evaluate the ability of MLLM on the robot use, please see: [RobotWorld](https://robotworldai.github.io/)😙
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
- FORCA: A Force-Aware Coding Agent for Contact-Rich Robot Manipulation — *Writes Python robot programs from language and visual input, uses wrist force/torque feedback during execution, then revises the program from recorded force and visual outcomes; evaluated on five real-robot tasks without demonstrations or task-specific training.*
  <a href="https://arxiv.org/abs/2610.31841"><img src="https://img.shields.io/badge/arxiv-2610.31841-silver" alt="Paper"></a>
  <a href="https://tanoom.github.io/forca/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- Self-Building Labs — *Given a scientific goal, an AI system configures a laboratory setup by building missing layouts, digital twins, robot skills, and workflows; demonstrated across robot setups and a real quantum-dot synthesis experiment.*
  <a href="https://arxiv.org/abs/2610.23826"><img src="https://img.shields.io/badge/arxiv-2610.23826-silver" alt="Paper"></a>
  <a href="https://self-building-labs.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- CLARO: Clutter Aware Robot Orchestrator for Open-Vocabulary Grasping using VLM Agents — *A VLM agent orchestrates detection, segmentation, grasping, and pushing skills with action memory to retrieve language-specified objects in clutter; reports simulated results and 88.8% success on its real-arm evaluation.*
  <a href="https://arxiv.org/abs/2610.24016"><img src="https://img.shields.io/badge/arxiv-2610.24016-silver" alt="Paper"></a>
- Embodied Task Agents Can Perform Fine Manipulation through Tactile In-Context Learning (Tactile-ETA) — *Adds aligned visual–tactile demonstrations to a general-purpose robot agent’s context without updating its parameters; reports gains on four simulated tasks and a small set of physical manipulation tasks.*
  <a href="https://arxiv.org/abs/2610.27613"><img src="https://img.shields.io/badge/arxiv-2610.27613-silver" alt="Paper"></a>
  <a href="https://no-518.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- HexaShell: A Thin Harness for Exploring the Limits of VLM Agents as Robot Coding Agents — *A coding agent controls a dual-arm robot through a thin CLI, inspects failures, and writes reusable perception tools; v2 reports 46.9% success on the official hidden-seed benchmark (53.2% progress), while tight insertion remains difficult.*
  <a href="https://arxiv.org/abs/2610.23479"><img src="https://img.shields.io/badge/arxiv-2610.23479-silver" alt="Paper"></a>
  <a href="https://github.com/HexaFuture/HexaShell"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/HexaFuture/HexaShell"><img src="https://img.shields.io/github/stars/HexaFuture/HexaShell" alt="stars"></a>
- RoboHarness: A Simple Harness Outperforms VLA and World Action Models — *Gives a coding agent a visual-geometric control panel for invoking embodied tasks; v2 reports BEHAVIOR Challenge results and says implementation is open source, but the arXiv record does not link the repository.*
  <a href="https://arxiv.org/abs/2610.14018"><img src="https://img.shields.io/badge/arxiv-2610.14018-silver" alt="Paper"></a>
- Can a Frontier VLM Serve as a Robot Policy for Memory-Dependent Manipulation? — *A frozen frontier VLM controls memory-dependent manipulation through TCP waypoints and gripper commands while retaining visual history; evaluated in simulation with disclosed adaptive development on the test split.*
  <a href="https://arxiv.org/abs/2610.17350"><img src="https://img.shields.io/badge/arxiv-2610.17350-silver" alt="Paper"></a>
  <a href="https://embodied-astra.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/jackbjed/embodied-astra-robomme"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/jackbjed/embodied-astra-robomme"><img src="https://img.shields.io/github/stars/jackbjed/embodied-astra-robomme" alt="stars"></a>
- JoyInside-VLM-Agent: Product-Conditioned Multimodal Policy Learning for Embodied Agents — *Post-trains a multimodal ReAct agent to select tools under product-specific robot capabilities and constraints; evaluates tool decisions and includes selected physical quadruped interaction traces rather than broad robot success-rate testing.*
  <a href="https://arxiv.org/abs/2610.12957"><img src="https://img.shields.io/badge/arxiv-2610.12957-silver" alt="Paper"></a>
- TacZero: Training-Free Peg Insertion Using a General-Purpose Vision-Language Model with Tactile Feedback — *A pretrained general-purpose VLM interprets visual and tactile feedback to issue end-effector targets for physical peg insertion without additional task training; evaluated after scripted grasp preparation with human-judged outcomes.*
  <a href="https://arxiv.org/abs/2610.07621"><img src="https://img.shields.io/badge/arxiv-2610.07621-silver" alt="Paper"></a>
- RobotUse: Allocating Computation, Context, and Decisions — *Allocates task intent to a main agent, visual target and pose decisions to subagents, and geometry and control to a robot backend; a persistent playbook supports adaptation from execution experience, with simulation and physical-robot evaluation.*
  <a href="https://arxiv.org/abs/2610.04929"><img src="https://img.shields.io/badge/arxiv-2610.04929-silver" alt="Paper"></a>
  <a href="https://robotuse-team.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/robotuse-team/RobotUse"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/robotuse-team/RobotUse"><img src="https://img.shields.io/github/stars/robotuse-team/RobotUse" alt="stars"></a>
- SuperNav: An Agentic Navigation System for Any Task in Any Scene — *A pretrained multimodal agent uses navigation skills, tools, progress tracking, and a visual-point interface to delegate motion to geometric or learned executors; includes simulated evaluations and quadruped deployment.*
  <a href="https://arxiv.org/abs/2610.12126"><img src="https://img.shields.io/badge/arxiv-2610.12126-silver" alt="Paper"></a>
  <a href="https://zju3dv.github.io/SuperNav/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/zju3dv/SuperNav"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/zju3dv/SuperNav"><img src="https://img.shields.io/github/stars/zju3dv/SuperNav" alt="stars"></a>
- SpatialHarness: Test-Time Spatial Scaffolding for Fine Robotic Manipulation — *Adds synchronized virtual views and structured spatial observations to a frozen multimodal robot policy at test time; evaluated on four physical manipulation tasks with 15 trials per method and task.*
  <a href="https://arxiv.org/abs/2610.12457"><img src="https://img.shields.io/badge/arxiv-2610.12457-silver" alt="Paper"></a>
- OpenRUA: Robot-Use Agents Are Zero-Shot Visuomotor Policies — *Off-the-shelf coding agents write perception and control programs through native ROS 2 terminal interfaces, with no task-specific policy training; evaluated in simulation with time paused during agent deliberation.*
  <a href="https://arxiv.org/abs/2610.02459"><img src="https://img.shields.io/badge/arxiv-2610.02459-silver" alt="Paper"></a>
  <a href="https://github.com/terminalworld/OpenRUA"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/terminalworld/OpenRUA"><img src="https://img.shields.io/github/stars/terminalworld/OpenRUA" alt="stars"></a>
- RoboICL: Embodied In-Context Learning with GPT-6 Astra — *A frozen general-purpose VLM issues Cartesian action chunks through a validated robot interface, using demonstrations, execution receipts, and observation history for closed-loop correction; simulation and real-robot evaluation.*
  <a href="https://arxiv.org/abs/2609.34261"><img src="https://img.shields.io/badge/arxiv-2609.34261-silver" alt="Paper"></a>
  <a href="https://github.com/Mosi-AI/RoboICL"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/Mosi-AI/RoboICL"><img src="https://img.shields.io/github/stars/Mosi-AI/RoboICL" alt="stars"></a>
- ASENA: Self-evolving Agents for Embodied Navigation — *A general-purpose coding agent navigates through sensor and execution tools while accumulating persistent notes and programs; evaluates repeated-task improvement in simulation and supervised humanoid demonstrations.*
  <a href="https://arxiv.org/abs/2609.39207"><img src="https://img.shields.io/badge/arxiv-2609.39207-silver" alt="Paper"></a>
  <a href="https://asena-bot.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- MotorMind: Scaffolding General Vision Language Models for Zero-Shot Robot Manipulation — *A frozen general-purpose VLM controls robot manipulation through mid-level actions, asynchronous monitoring, outcome verification, and background memory updates; evaluated in simulation and on an xArm6.*
  <a href="https://arxiv.org/abs/2609.38078"><img src="https://img.shields.io/badge/arxiv-2609.38078-silver" alt="Paper"></a>
  <a href="https://motor-mind.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- Robot Manipulation with GPT-6-Astra: Body Knowledge, Experience Reuse, Emergent Skills, and Sim2Real Transfer — *Body descriptions and recorded experience support reusable control code and sim-to-real transfer; physical evaluation comprises 12 trials using operator-confirmed button contact.*
  <a href="https://arxiv.org/abs/2609.31770"><img src="https://img.shields.io/badge/arxiv-2609.31770-silver" alt="Paper"></a>
  <a href="https://github.com/hesd10/astra-robot-sim2real"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/hesd10/astra-robot-sim2real"><img src="https://img.shields.io/github/stars/hesd10/astra-robot-sim2real" alt="stars"></a>
- **Know Your Body: A Harness for Direct and Self-Improving Robot Control with VLMs** — KnowBody; body-grounded robot control and iterative improvement through execution feedback, evaluated on a small real-robot task suite.
  <a href="https://arxiv.org/abs/2609.28530"><img src="https://img.shields.io/badge/arxiv-2609.28530-silver" alt="Paper"></a>
  <a href="https://loule0-0.github.io/KnowBody/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- Generalizing Manipulation Skills with a Local Coding Agent — *A local open-weight VLM writes and executes perception and control code for real-world UR3e manipulation, with documented skills and in-session reuse.*
  <a href="https://arxiv.org/abs/2609.26499"><img src="https://img.shields.io/badge/arxiv-2609.26499-silver" alt="Paper"></a>
  <a href="https://rtalwar2.github.io/agentic-coding-for-robot-manipulation/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
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
- Guava: Distilling Frontier VLMs into a Compact Agent through a Robotic Manipulation Harness
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

- ThinkLocoManip: A Whole-Body Control Agentic Harness for Legged Loco-Manipulation — *Interleaves reasoning and action while composing perception, navigation, manipulation, and locomotion tools for long-horizon legged tasks.*
  <a href="https://arxiv.org/abs/2610.34370"><img src="https://img.shields.io/badge/arxiv-2610.34370-silver" alt="Paper"></a>
- Pretraining Knows What, Simulation Teaches How: Compositional Generalization in a Sim-Trained Robot Agent — *ZAP adapts a pretrained 27B VLM to robot tool use through simulation SFT and GRPO; reports real-world transfer without real-robot training data.*
  <a href="https://arxiv.org/abs/2610.35817"><img src="https://img.shields.io/badge/arxiv-2610.35817-silver" alt="Paper"></a>
- Agentic World Action Models — *AW-0 couples code-based reusable skill programs with future-video and action prediction, joining agentic planning and physical dynamics in one model.*
  <a href="https://arxiv.org/abs/2610.30136"><img src="https://img.shields.io/badge/arxiv-2610.30136-silver" alt="Paper"></a>
  <a href="https://agentic-wam.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- OmniBrain-0: A Unified Agentic Model for Embodied Intelligence — *A compact learned agent coordinates manipulation and navigation, with a rubric-guided recursive data flywheel and real-world evaluations.*
  <a href="https://arxiv.org/abs/2610.36013"><img src="https://img.shields.io/badge/arxiv-2610.36013-silver" alt="Paper"></a>
  <a href="https://public-bots.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>

### Reasoning-Acting and Dual-System Architectures

Architectures that organize reasoning and robot execution through intermediate plans, coupled reasoning and action modules, or adaptive think/act scheduling. Includes learned-policy building blocks and agent-level systems. For author-described System 1 (e.g., Jev-like system) /System 2 models (VLM-like models), fixed-rate and asynchronous coupling are distinguished from adaptive reasoning. Related task-time memory and recovery methods remain under [Planning, Skill Orchestration and Memory](#planning-skill-orchestration-and-memory).
- Make π0.5 Learn to Call Astra for Reliable Robot Manipulation — *Learns a CALL head on frozen policy features to request a general-purpose model for closed-loop recovery and then hand control back to the robot policy; evaluated on LIBERO with additional consultation cost.*
  <a href="https://arxiv.org/abs/2610.14117"><img src="https://img.shields.io/badge/arxiv-2610.14117-silver" alt="Paper"></a>
  <a href="https://kykgeek.github.io/Pi05_CALL_Astra/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- Bridging Frontier Reasoning and Robot Execution: From Autonomous Demonstration Generation to Dense Language Supervision — *Connects frontier-model guidance to a trained local policy through autonomous demonstration collection, corrective examples, and dense language supervision; evaluated in simulation and on physical manipulation tasks.*
  <a href="https://arxiv.org/abs/2610.03615"><img src="https://img.shields.io/badge/arxiv-2610.03615-silver" alt="Paper"></a>
- Code Owns the Simulation, Jev Owns the Evaluation — *Studies Jev as an evaluator of outcomes supplied by code, combining lookahead and executable skills; includes simulated Stacker control and instruction variants, with action-abstraction differences limiting causal attribution.*
  <a href="https://arxiv.org/abs/2610.01834"><img src="https://img.shields.io/badge/arxiv-2610.01834-silver" alt="Paper"></a>
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
- Spatial Memory by Agents, for Agents — *A coding agent iteratively designs spatial-memory construction and retrieval code using a fixed query agent, then freezes it before held-out evaluation across five memory tasks; reports gains over a broad ReMEmbR baseline, while noting grounding and evidence-use failures.*
  <a href="https://arxiv.org/abs/2610.22736"><img src="https://img.shields.io/badge/arxiv-2610.22736-silver" alt="Paper"></a>
  <a href="https://ba-fa-3344.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- Externalise the Memory: A Pre-Registered Study of Where an Embodied Agent’s Experience Should Live — *A pre-registered reach-task study finds retrieval memory attached to fixed policy weights helps more than distilling memory-augmented behavior into weights; the registered weight-distillation claim was underpowered and inconclusive.*
  <a href="https://arxiv.org/abs/2610.30478"><img src="https://img.shields.io/badge/arxiv-2610.30478-silver" alt="Paper"></a>
- FastHarness: Experience-Driven Review Scheduling for Vision-Language-Action Policies — *Adaptively schedules reviewer calls around a frozen VLA policy using experience and execution feedback; reports efficiency and task performance on simulated manipulation, so this is harness adaptation rather than policy training.*
  <a href="https://arxiv.org/abs/2610.31427"><img src="https://img.shields.io/badge/arxiv-2610.31427-silver" alt="Paper"></a>
  <a href="https://fastharness.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/FastHarness/fast-harness"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
- An Agentic Framework for Proactive Robots with Procedural Assistance Memory — *Maintains a finite-state procedural assistance memory that a VLM revises between days to personalize when and how a robot helps, while a separately trained VLA executes the selected tasks.*
  <a href="https://arxiv.org/abs/2610.21211"><img src="https://img.shields.io/badge/arxiv-2610.21211-silver" alt="Paper"></a>
  <a href="https://davian-robotics.github.io/PAM/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- ProactiveVLA: Augmenting Embodied Memory through Proactive Environment Exploration — *Uses a reasoning agent and frozen VLA to explore self-proposed goals, verify interactions, and consolidate reusable environment knowledge before evaluation; studies adaptation in simulated manipulation tasks.*
  <a href="https://arxiv.org/abs/2610.06999"><img src="https://img.shields.io/badge/arxiv-2610.06999-silver" alt="Paper"></a>
- RoboHarn-Evo: Evolving Hierarchical Physical Knowledge for Self-Improving Robotic Manipulation — *A dual-loop manipulation harness evolves persistent task and action knowledge from physical feedback while keeping the base model fixed, supporting retrieval, correction, and reuse across episodes.*
  <a href="https://arxiv.org/abs/2609.37583"><img src="https://img.shields.io/badge/arxiv-2609.37583-silver" alt="Paper"></a>
- Recursive Harness Distillation across Agents for Robot Manipulation — *A strong agent distills and refines intervention experience into a reusable playbook for lighter agents operating frozen robot policies; evaluated in simulation and real-world manipulation.*
  <a href="https://arxiv.org/abs/2609.33378"><img src="https://img.shields.io/badge/arxiv-2609.33378-silver" alt="Paper"></a>

- NavHarness: Towards Lifelong Embodied Navigation — *A training-free navigation harness that carries maps, task records, recovery handovers, and consolidated knowledge across reasoning sessions; evaluated in simulated navigation environments.*
  <a href="https://arxiv.org/abs/2609.34276"><img src="https://img.shields.io/badge/arxiv-2609.34276-silver" alt="Paper"></a>
  <a href="https://github.com/billzhao1030/NavHarness"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/billzhao1030/NavHarness"><img src="https://img.shields.io/github/stars/billzhao1030/NavHarness" alt="stars"></a>
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

- ReSight: Task-Driven Self-Improving Memory for Embodied Agents — *Separates execution-time memory queries from coding-agent exploration, distilling discoveries into reusable memory builders, tools, and skills.*
  <a href="https://arxiv.org/abs/2610.33487"><img src="https://img.shields.io/badge/arxiv-2610.33487-silver" alt="Paper"></a>

#### Skill and Program Evolution
- Compile Once, Run Cheap: Frozen, Portable Skills for Embodied Agents, and What Recursive Self-Improvement Adds — *A strong model authors and repairs skills offline in simulation; frozen executable skills are reused without a frontier model at every run. Skill-RSI reports seven skills across four of seven RoboTwin tasks, but three tasks fail its strict safety gate.*
  <a href="https://arxiv.org/abs/2610.25114"><img src="https://img.shields.io/badge/arxiv-2610.25114-silver" alt="Paper"></a>
  <a href="https://github.com/Orillusion/embodied-skill-rsi"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
- SERA: From VLM Planners to Robotic Agents: Self-Evolving Harnesses for History-Dependent Manipulation — *Evolves contextual memory and execution feedback around a fixed VLA executor, then freezes the harness for held-out evaluation; reports gains on RoboMME, with evidence limited to the benchmark setting.*
  <a href="https://arxiv.org/abs/2610.29560"><img src="https://img.shields.io/badge/arxiv-2610.29560-silver" alt="Paper"></a>
- Agentic RSR: Real-to-Sim-to-Real through Scene Reconstruction and Execution-Grounded Robot Policies — *A coding agent develops executable manipulation policies through progressively less privileged simulation, then carries the task interface and accumulated experience onto the real robot; the arXiv v2 appeared during this window, while code is still described as forthcoming.*
  <a href="https://arxiv.org/abs/2610.10479"><img src="https://img.shields.io/badge/arxiv-2610.10479-silver" alt="Paper"></a>
- Agentic Robot Creation through Generation, Verification, and Revision — *Roboforge turns task specifications into executable policies and revises motions or rewards from rollout feedback; includes a fabricated agent-generated robot with physical deployment.*
  <a href="https://arxiv.org/abs/2610.17881"><img src="https://img.shields.io/badge/arxiv-2610.17881-silver" alt="Paper"></a>
  <a href="https://roboforge-project.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- EmbodiedEvo: Self-Evolving Coding Agent For Physical Intelligence — *Distills a coding agent’s robot experience into reusable executable skills and diagnostic lessons, acquired on one playground scene per task and frozen for agents acting in new scenes; evaluated on RoboDojo-Sim.*
  <a href="https://arxiv.org/abs/2610.18867"><img src="https://img.shields.io/badge/arxiv-2610.18867-silver" alt="Paper"></a>
  <a href="https://github.com/RoboProbe/RoboProbe"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/RoboProbe/RoboProbe"><img src="https://img.shields.io/github/stars/RoboProbe/RoboProbe" alt="stars"></a>
- EnactOpt: Diagnosis-Guided Harness Evolution for Embodied Agents — *Uses execution diagnoses to jointly revise textual skills and executable context-management logic around frozen models; independently evolved harnesses are evaluated on embodied and text-based task benchmarks.*
  <a href="https://arxiv.org/abs/2610.14977"><img src="https://img.shields.io/badge/arxiv-2610.14977-silver" alt="Paper"></a>
- Fly-by-Code: Embodied Coding Agents for Aerial Manipulation with Active Visual and Physical Feedback — *A coding agent refines aerial-manipulation programs using separate diagnostic programs that gather active visual and physical evidence in simulation; shared APIs support subsequent physical execution.*
  <a href="https://arxiv.org/abs/2610.12549"><img src="https://img.shields.io/badge/arxiv-2610.12549-silver" alt="Paper"></a>
  <a href="https://fly-by-code.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- EMHO: EMbodied Agent Harness Optimization via Experience Traces — *Revises planning, context construction, visual tool use, and recovery logic from execution traces while keeping the embodied model frozen; evaluates harness evolution on simulated EmbodiedBench tasks and reports held-out overfitting in later iterations.*
  <a href="https://arxiv.org/abs/2610.08432"><img src="https://img.shields.io/badge/arxiv-2610.08432-silver" alt="Paper"></a>
  <a href="https://hyunjung00.github.io/emho/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- RoboRSI: Stable, Efficient, and Reusable Robot Self-Evolution in Complex Real-World Environments — *Human-guided skill-tree refinement attributes failures, revises scoped capabilities, and validates reusable skills; includes 104 evolving real-robot development rounds and simulation benchmarks.*
  <a href="https://arxiv.org/abs/2610.12424"><img src="https://img.shields.io/badge/arxiv-2610.12424-silver" alt="Paper"></a>
  <a href="https://lab.noematrix.ai/blog/2-roborsi-research-preview/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/nssmd/RoboRSI"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/nssmd/RoboRSI"><img src="https://img.shields.io/github/stars/nssmd/RoboRSI" alt="stars"></a>
- Embodied Turing Machines: Stateful Code for Robot Recursive Self-Improvement — *Coding agents develop a shared library of stateful robot programs from execution feedback; the resulting code-only policies run without VLM or VLA calls at test time, evaluated on simulated bimanual tasks.*
  <a href="https://arxiv.org/abs/2610.12369"><img src="https://img.shields.io/badge/arxiv-2610.12369-silver" alt="Paper"></a>
- RoboBridge: A Self-Evolving Embodied Agent Framework for Sim-to-Real Transfer — *Transfers revisable procedural skills from simulation to physical tasks and validates further skill updates from execution feedback, exposing a frozen VLA as a tool with optional inference-time guidance.*
  <a href="https://arxiv.org/abs/2610.02717"><img src="https://img.shields.io/badge/arxiv-2610.02717-silver" alt="Paper"></a>
- Skill2Real: Agentic Skill Learning for Zero-Shot Sim-to-Real Robot Manipulation — *Learns hierarchical executable skills through a shared robot API using simulation diagnosis and validation gates, then transfers frozen skill memories to a physical UR5e without target-task policy fine-tuning.*
  <a href="https://arxiv.org/abs/2610.02788"><img src="https://img.shields.io/badge/arxiv-2610.02788-silver" alt="Paper"></a>
- InterEvolve: Test-Time Evolution of Reward Programs for Humanoid Loco-Manipulation — *An LLM evolves staged reward programs using simulation feedback and a verified skill library, while numerical search tunes constants for a fixed pretrained humanoid controller; includes physical G1 deployment.*
  <a href="https://arxiv.org/abs/2610.02196"><img src="https://img.shields.io/badge/arxiv-2610.02196-silver" alt="Paper"></a>
  <a href="https://sirui-xu.github.io/InterEvolve"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- Reconstruct, Practice, Go Real: Guided Self-Improvement for Embodied Agents — *Improves a persistent skill library and system prompt through simulation practice, privileged failure diagnosis, and cross-task validation, then freezes the calibrated system for physical deployment.*
  <a href="https://arxiv.org/abs/2610.02204"><img src="https://img.shields.io/badge/arxiv-2610.02204-silver" alt="Paper"></a>
  <a href="https://rpg-robot.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- RoboRSI: Stable, Efficient, and Reusable Robot Self-Evolution in Complex Real-World Environments — *Research blog and open-source harness; multiple agents refine a task–skill tree from execution feedback, consolidate workflows into code, and gate skill changes with regression checks.*
  <a href="https://lab.noematrix.ai/blog/2-roborsi-research-preview/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/nssmd/RoboRSI"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/nssmd/RoboRSI"><img src="https://img.shields.io/github/stars/nssmd/RoboRSI" alt="stars"></a>
- SimEX: Simulation-Integrated Robotics AutoResearch — *A coding agent develops reusable robot toolboxes in simulation and uses limited real-world trials to repair both tools and simulators; demonstrated on three bimanual task families.*
  <a href="https://arxiv.org/abs/2609.38982"><img src="https://img.shields.io/badge/arxiv-2609.38982-silver" alt="Paper"></a>
  <a href="https://robo-simex.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- Explore, Execute, Evolve: A Skill Acquisition and Reuse Loop for Embodied Agents — *RoboSkill; an exploration–execution–evolution loop accumulates reusable textual and executable skills from robot experience, with visual and tactile feedback and cross-agent skill reuse.*
  <a href="https://arxiv.org/abs/2609.37810"><img src="https://img.shields.io/badge/arxiv-2609.37810-silver" alt="Paper"></a>
  <a href="https://github.com/SII-dannyXSC/RoboSkill"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/SII-dannyXSC/RoboSkill"><img src="https://img.shields.io/github/stars/SII-dannyXSC/RoboSkill" alt="stars"></a>
- Self-Evolving Coding Agents: From Digital Programs to Physical-World Intelligence — *HexaAnything; executable world state and control workflows support tool-based robot execution, tool refinement, and trace-based model training; includes simulation and physical-robot studies.*
  <a href="https://arxiv.org/abs/2609.35432"><img src="https://img.shields.io/badge/arxiv-2609.35432-silver" alt="Paper"></a>

- RoboFoundry: System-as-Policy Evolution for Self-Learning Embodied Agents — *Evolves context management, persistent memory, and hierarchical skills through validated execution-driven system edits while keeping the foundation model frozen; includes physical robot evaluation.*
  <a href="https://arxiv.org/abs/2609.32862"><img src="https://img.shields.io/badge/arxiv-2609.32862-silver" alt="Paper"></a>
  <a href="https://jingsongliang.com/robofoundry/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- HarnessPAI: An Evolving Harness for Physical AI — Coding agents refine executable robot harnesses between rollouts using execution feedback, while keeping the underlying action backends frozen.
  <a href="https://arxiv.org/abs/2609.29166"><img src="https://img.shields.io/badge/arxiv-2609.29166-silver" alt="Paper"></a>

- RACaP: Agentic Reasoning, Acting, and Coding as Policies for Evolvable Robot Learning — Combines reasoning, acting, and code evolution to build reusable robot APIs and harness memory; evaluated in simulation.
  <a href="https://arxiv.org/abs/2609.29394"><img src="https://img.shields.io/badge/arxiv-2609.29394-silver" alt="Paper"></a>

- AdaHVLA: Adaptive Harnesses for Long-Horizon Vision-Language-Action Execution — Refines code-based coordination between reasoning agents and frozen VLAs through rollout evidence and persistent revision memory; simulation benchmarks and a real-world quadruped deployment case.
  <a href="https://arxiv.org/abs/2609.29204"><img src="https://img.shields.io/badge/arxiv-2609.29204-silver" alt="Paper"></a>
  <a href="https://github.com/Haaareally/AdaHVLA-Adaptive_Harness_VLA"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/Haaareally/AdaHVLA-Adaptive_Harness_VLA"><img src="https://img.shields.io/github/stars/Haaareally/AdaHVLA-Adaptive_Harness_VLA" alt="stars"></a>
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

- MOTIO: Agentic Skill Engineering for Reality-Grounded Humanoid Loco-Manipulation — *Turns videos, 3D assets, motion references, and reusable interfaces into executable humanoid skills refined through simulation, physical feedback, and human approval.*
  <a href="https://arxiv.org/abs/2610.33446"><img src="https://img.shields.io/badge/arxiv-2610.33446-silver" alt="Paper"></a>
  <a href="https://iiiiqiiii.github.io/motio/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>

#### Autonomous Data Collection and Policy Improvement
- Where is Physical RSI capability from? An Observational Scaling Law of LLM-as-policy — *Introduces PhysRSI-eval across 18 manipulation tasks and analyzes first-attempt performance, efficiency, success, budget, and improvement from failure; workspace interventions suggest persistent interaction history and reusable experience can support later and cross-task gains.*
  <a href="https://arxiv.org/abs/2610.26848"><img src="https://img.shields.io/badge/arxiv-2610.26848-silver" alt="Paper"></a>
- Scaling Online Exploration for Robot Agents — *RAX uses a frozen general-purpose coding agent to learn from online robot exploration and compile verified skills into executable programs; reports multi-embodiment simulation and physical-robot tasks, with an open harness and skill library.*
  <a href="https://arxiv.org/abs/2610.22496"><img src="https://img.shields.io/badge/arxiv-2610.22496-silver" alt="Paper"></a>
  <a href="https://robot-agent-exploration.com/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/robot-agent-exploration/rax"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/robot-agent-exploration/rax"><img src="https://img.shields.io/github/stars/robot-agent-exploration/rax" alt="stars"></a>
- D-World: An Explicit World-Language-Action Model with Recursive Self-Improvement under Dual Control — *Separate perception and planning agents write and revise an executable digital twin from measured robot feedback; dual-arm towel and toaster tasks illustrate local, measurement-checked revisions while the LLM remains frozen.*
  <a href="https://arxiv.org/abs/2610.17114"><img src="https://img.shields.io/badge/arxiv-2610.17114-silver" alt="Paper"></a>
- AdaRSI: On-Demand Recursive Self-Improvement for Embodied Agents — *A coding agent first revises its robot harness, then diagnoses persistent failures through saved-state retries and selectively fine-tunes missing executor skills using self-collected demonstrations; simulation evaluation.*
  <a href="https://arxiv.org/abs/2610.20474"><img src="https://img.shields.io/badge/arxiv-2610.20474-silver" alt="Paper"></a>
- EndoRSI: Physical-Evidence-Driven Recursive Improvement of Endoscopic Robot Policies — *Uses a coding-agent research loop to revise endoscopic robot policies from physical experiments, failure evidence, and new supervision; evaluation includes benchtop and ex vivo studies under human-authorized execution.*
  <a href="https://arxiv.org/abs/2610.13376"><img src="https://img.shields.io/badge/arxiv-2610.13376-silver" alt="Paper"></a>
- EmbodiedSmith: Scaling Embodied Data through Recursive Self-Improvement Flywheel in Simulation — *Uses agents to compose skill graphs and iteratively refine simulated scenes, placements, and execution plans for robot data generation, then trains downstream policies on accepted trajectories; improvements are task-dependent.*
  <a href="https://arxiv.org/abs/2610.07969"><img src="https://img.shields.io/badge/arxiv-2610.07969-silver" alt="Paper"></a>
- EmbodiRSI: Recursive Self-Improvement for Data-Efficient Robot Adaptation — *Coordinates agent-assisted correction and adaptive data collection in task-specific simulations to improve robot policies, followed by limited human-in-the-loop physical refinement and policy-only deployment.*
  <a href="https://arxiv.org/abs/2609.38905"><img src="https://img.shields.io/badge/arxiv-2609.38905-silver" alt="Paper"></a>
- Co-Evolving Robot Orchestrators and Policies through Deployment — *Co-evolves a VLM orchestrator and robot policy using curated deployment experience, skill-level candidate verification, and rollback; evaluates frozen policy and memory on held-out simulated and physical tasks.*
  <a href="https://arxiv.org/abs/2610.09228"><img src="https://img.shields.io/badge/arxiv-2610.09228-silver" alt="Paper"></a>
- Find Something You Can't Do: Agentic Real-World Reinforcement Learning for Self-Improving VLA Models — *A vision-language agent selects feasible practice tasks and evaluates outcomes in a persistent workspace, driving residual reinforcement learning over a frozen VLA with reduced manual resets.*
  <a href="https://arxiv.org/abs/2609.32069"><img src="https://img.shields.io/badge/arxiv-2609.32069-silver" alt="Paper"></a>
- MobiAgent: Dual-Loop Recursive Policy Self-Improvement for Long-Horizon Mobile Manipulation — *A VLM planner and visual critic compose reusable skill policies, while an offline outer loop segments, verifies, and recycles deployment trajectories to fine-tune the skill library.*
  <a href="https://arxiv.org/abs/2610.03476"><img src="https://img.shields.io/badge/arxiv-2610.03476-silver" alt="Paper"></a>
- SkillWeaver: Agentic Exploration over Neural Interaction Skills for Scalable Robot Data Generation — *A VLM agent composes reusable closed-loop neural interaction skills through verifier-guided exploration, reflection, and memory to generate simulated robot demonstrations for downstream policy learning.*
  <a href="https://arxiv.org/abs/2609.36171"><img src="https://img.shields.io/badge/arxiv-2609.36171-silver" alt="Paper"></a>
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
- AgenticRoboRL: Training Robot Planners through Harnesses with Multi-Turn Reinforcement Learning — *Trains a planner through robot harnesses while freezing execution; v2 reports LIBERO-PRO success improving from 18.1% to 71.0% for a 9B model, with code/checkpoints still forthcoming.*
  <a href="https://arxiv.org/abs/2610.28589"><img src="https://img.shields.io/badge/arxiv-2610.28589-silver" alt="Paper"></a>
- Scale and Selection: What Makes Automatic Harness Evolution Work for Visual-Interface Robot Agents — *Studies rollout scale and matched champion–challenger selection for agent-driven evolution of visual robot harnesses, measuring generalization to held-out simulated tasks.*
  <a href="https://arxiv.org/abs/2609.39304"><img src="https://img.shields.io/badge/arxiv-2609.39304-silver" alt="Paper"></a>
- DynaHarness: A Dynamic Physical Harness for Self-Evolving Robot Agents — *A semantic planner and deterministic execution governor share contracts for refusal, substitution, and recovery, with evidence-based failure attribution and regression-gated capability updates around a frozen policy.*
  <a href="https://arxiv.org/abs/2609.40306"><img src="https://img.shields.io/badge/arxiv-2609.40306-silver" alt="Paper"></a>
  <a href="https://denghaoyuan123.github.io/Dynaharness_page/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
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

- VISTA: Active Exploration for Self-Improvement in Embodied Agents — *A meta-agent actively tests harness revisions in the environment and tracks version lineage while model parameters remain fixed.*
  <a href="https://arxiv.org/abs/2610.35051"><img src="https://img.shields.io/badge/arxiv-2610.35051-silver" alt="Paper"></a>
  <a href="https://agenticei.github.io/VISTA-page/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/AgenticEI/VISTA"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
- RoboDoctor: Training-Free Recursive Self-Improvement for Robot Policies — *Uses execution feedback to revise the harness, intervention policy, and physical operating methods while retaining linked experience across episodes.*
  <a href="https://arxiv.org/abs/2610.35604"><img src="https://img.shields.io/badge/arxiv-2610.35604-silver" alt="Paper"></a>

### Embodied Agent Operating Systems and Runtimes
- CARE: Know When to Escalate: Critic-Guided Adaptive Execution for Cloud-Local Embodied Agents — *A lightweight critic escalates unreliable local execution to a stronger cloud agent and shares handoff memory; reports improvements across embodied benchmarks, with latency and model-cost trade-offs to consider.*
  <a href="https://arxiv.org/abs/2610.30587"><img src="https://img.shields.io/badge/arxiv-2610.30587-silver" alt="Paper"></a>

Persistent embodied-agent systems that organize robot capabilities, state, resources, execution checks, and feedback across tasks or robots.
- InstAgent: A Recursively Self-Improving Agent Operating System for Heterogeneous Robot Collaboration — *Organizes collaboration as behavior trees with capability assignment, dependency and handoff checks; retains feedback-driven program revisions and shared spatiotemporal memory, evaluated on 20 real-world multi-robot tasks.*
  <a href="https://arxiv.org/abs/2610.23098"><img src="https://img.shields.io/badge/arxiv-2610.23098-silver" alt="Paper"></a>
- BT-Agent: Deploying Onboard Robot Agents with Behavior Trees and Multi-Fidelity Evaluation — *Deploys an onboard language-model agent that selects predefined behavior-tree skills with structured execution feedback and local interruption checks; evaluated through text, simulation, and supervised physical-robot trials.*
  <a href="https://arxiv.org/abs/2610.13862"><img src="https://img.shields.io/badge/arxiv-2610.13862-silver" alt="Paper"></a>
- From Social Reasoning to Embodied Interaction: An Agentic Framework for Social Robots — *Connects multimodal social reasoning and long-term memory to Sophia’s native gestures, speech, and facial actuators through streaming orchestration; evaluated with participant ratings and latency measurements.*
  <a href="https://arxiv.org/abs/2610.05964"><img src="https://img.shields.io/badge/arxiv-2610.05964-silver" alt="Paper"></a>
  <a href="https://robosocial.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- NavGPT-3: Harnessing Context in a Hierarchical Navigation Runtime — *Connects language-model planning, a trained navigation VLA, and monitoring through a hierarchical runtime with separate contexts and motion permissions; evaluated in navigation benchmarks and physical interruption studies.*
  <a href="https://arxiv.org/abs/2610.10787"><img src="https://img.shields.io/badge/arxiv-2610.10787-silver" alt="Paper"></a>
  <a href="https://metacognitionai.github.io/NavGPT3/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/metacognitionai/NavGPT-3"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/metacognitionai/NavGPT-3"><img src="https://img.shields.io/github/stars/metacognitionai/NavGPT-3" alt="stars"></a>
  <a href="https://huggingface.co/Metacognition-AI/NavGPT3-8B" title="Model"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
- RegenHarness: A Robot Agent Harness with Evidence-Gated Recursive Self-Improvement — *Evidence-gated skill execution, versioned task state, bounded recovery, and a protocol for regression-checked harness configuration updates; demonstrated through quadruped inspection cases.*
  <a href="https://arxiv.org/abs/2609.27612"><img src="https://img.shields.io/badge/arxiv-2609.27612-silver" alt="Paper"></a>
- NIMO Controller: a self-driving laboratory orchestrator based on the Model Context Protocol — *MCP-based tool discovery and experimental workflow orchestration for AI agents and human users in self-driving laboratories.*
  <a href="https://arxiv.org/abs/2605.15227"><img src="https://img.shields.io/badge/arxiv-2605.15227-silver" alt="Paper"></a>
  <a href="https://github.com/NIMS-DA/nimo-controller"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/NIMS-DA/nimo-controller"><img src="https://img.shields.io/github/stars/NIMS-DA/nimo-controller" alt="stars"></a>
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
- Natural-Language to Nav2: Operational Policies for Costmap-Based Navigation — *A local LLM maps operator instructions to explicit, validated JSON policies that Nav2 applies through costmap plugins; evaluated in Gazebo and on TurtleBot3, with policy interpretation errors and validator safeguards documented.*
  <a href="https://arxiv.org/abs/2610.32633"><img src="https://img.shields.io/badge/arxiv-2610.32633-silver" alt="Paper"></a>
  <a href="https://a56239637-dot.github.io/Natural-Language-to-Nav2-Project-Page/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/a56239637-dot/Natural-Language-to-Nav2-Operational-Policies-for-Costmap-Based-Navigation"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
- Multi-Tool Selection for Robotic Systems: Comparing Semantic Retrieval and LLM — *Compares retrieval and LLM routing for selecting executable robot capabilities from natural-language requests; evaluation uses 164 annotated prompts, so it tests tool selection rather than closed-loop robot task success.*
  <a href="https://arxiv.org/abs/2610.31013"><img src="https://img.shields.io/badge/arxiv-2610.31013-silver" alt="Paper"></a>
- MoCaP: Mobile Code-as-Policies for Zero-Shot Mobile Manipulation from Passive Human Videos — *Extracts spatial memory and approach priors from passive human video, then uses a code-as-policy agent and robot-specific navigation and manipulation tools for closed-loop mobile manipulation on physical hardware.*
  <a href="https://arxiv.org/abs/2610.20998"><img src="https://img.shields.io/badge/arxiv-2610.20998-silver" alt="Paper"></a>
  <a href="https://mocap-7.github.io/MoCAP-page/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/MoCAP-7/MoCAP"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/MoCAP-7/MoCAP"><img src="https://img.shields.io/github/stars/MoCAP-7/MoCAP" alt="stars"></a>
- VLMs are Native Action Models: Unleashing the Manipulation Capabilities of VLMs with Explicit Action-Space Grounding — *Grounds VLM-generated textual pose actions with an explicit tool-center-point frame and visual action-space cues, studying both zero-shot control and task-specific post-training in simulated and physical manipulation.*
  <a href="https://arxiv.org/abs/2610.12832"><img src="https://img.shields.io/badge/arxiv-2610.12832-silver" alt="Paper"></a>
- PhysCaP: Grounding Code-as-Policy Agent with Physics-Informed Exploration — *Augments code-as-policy agents with proprioception-based mass and stiffness measurement tools, using a Planner and Prioritizer to acquire task-relevant physical evidence; evaluated on physical tabletop tasks and in simulation.*
  <a href="https://arxiv.org/abs/2608.21031"><img src="https://img.shields.io/badge/arxiv-2608.21031-silver" alt="Paper"></a>
  <a href="https://physcap.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- Robotic Long-Horizon Manipulation with Progressive In-Context Code Generation and Episodic Feedback — *Generates executable robot plans from progressively organized in-context examples and uses episodic visual feedback for replanning; evaluated in simulation with four physical tabletop demonstrations.*
  <a href="https://arxiv.org/abs/2503.21969"><img src="https://img.shields.io/badge/arxiv-2503.21969-silver" alt="Paper"></a>
- Fewer Tokens, Better Action: GPT-6 Astra Robot Agents with 14% Higher Success Rate but 65% Fewer Tokens — *An interactive Python interface composes robot primitives and VLA policies with conditional checks, local retries, and selective feedback; evaluated against tool calling on 700 paired simulated task instances.*
  <a href="https://arxiv.org/abs/2610.01939"><img src="https://img.shields.io/badge/arxiv-2610.01939-silver" alt="Paper"></a>
  <a href="https://github.com/DAGroup-PKU/PyRUA-Lean"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/DAGroup-PKU/PyRUA-Lean"><img src="https://img.shields.io/github/stars/DAGroup-PKU/PyRUA-Lean" alt="stars"></a>
- InCoRo: In-Context Learning for Robotics Control with Feedback Loops — *An off-the-shelf LLM updates robot commands from scene-state feedback and in-context examples; demonstrated on physical SCARA and DELTA robots in static and dynamic environments.*
  <a href="https://arxiv.org/abs/2402.05188"><img src="https://img.shields.io/badge/arxiv-2402.05188-silver" alt="Paper"></a>
- Make Code as Policy Great Again: Frontier Agents Write, Call, and Evolve Robot Tools — *URAI; programming agents develop reusable robot tools with execution feedback and human guidance, while execution agents call validated tools for simulated and real bimanual tasks.*
  <a href="https://arxiv.org/abs/2609.39018"><img src="https://img.shields.io/badge/arxiv-2609.39018-silver" alt="Paper"></a>
- KPI: A Promptable Kernel for Physical Interaction on Humanoids — *A vision-language agent specifies reference trajectories and interaction contracts for a contact-control kernel above an unchanged whole-body tracker; demonstrated on instruction-driven humanoid interaction tasks.*
  <a href="https://arxiv.org/abs/2609.36151"><img src="https://img.shields.io/badge/arxiv-2609.36151-silver" alt="Paper"></a>
  <a href="https://kpi-robot.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>

- Encore: Few-Shot Agentic Discovery of Manipulation Strategies — *A coding agent reads structured demonstration evidence, develops policy programs through a fixed perception-and-action API, and freezes them for held-out evaluation; includes two bimanual real-robot tasks.*
  <a href="https://arxiv.org/abs/2609.37359"><img src="https://img.shields.io/badge/arxiv-2609.37359-silver" alt="Paper"></a>
  <a href="https://github.com/YIFANK/encore"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/YIFANK/encore"><img src="https://img.shields.io/github/stars/YIFANK/encore" alt="stars"></a>
- CognitiveReality: Robot-Agnostic Semantic Gaussian Mapping with an LLM Agent for Immersive Collaborative VR Teleoperation — *An LLM routes language and spatial references to typed tools and robot missions over a shared semantic map, with operator confirmation and physical quadruped evaluation.*
  <a href="https://arxiv.org/abs/2609.31418"><img src="https://img.shields.io/badge/arxiv-2609.31418-silver" alt="Paper"></a>

- **RAPID: Robot Agentic Programming from Demonstrations** — Converts visual demonstrations into robot programs through task specifications, reusable primitives, and interactive verification.
  <a href="https://arxiv.org/abs/2609.30249"><img src="https://img.shields.io/badge/arxiv-2609.30249-silver" alt="Paper"></a>

- **Coding Agents for Generalized Task and Motion Planning Problems** — Coding agents synthesize reusable planning programs for simulated environments; held-out evaluation executes fixed programs without test-time LLM calls.
  <a href="https://arxiv.org/abs/2609.30233"><img src="https://img.shields.io/badge/arxiv-2609.30233-silver" alt="Paper"></a>
  <a href="https://agenticgentamp.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/tomsilver/robocode"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/tomsilver/robocode"><img src="https://img.shields.io/github/stars/tomsilver/robocode" alt="stars"></a>
- ManiSkillFormer: Demonstration-Free Compositional Manipulation via Geometric Contracts and Agentic Skill Graph
  <a href="https://arxiv.org/abs/2609.16331"><img src="https://img.shields.io/badge/arxiv-2609.16331-silver" alt="Paper"></a>
  <a href="https://patricia1019.github.io/ManiSkillFormer/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
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
- Plan First, Act Later: Streaming Reasoning for Executable Memory in Robot Control (PAL) — *Streams visual evidence into semantic-event memory and an executable subtask list for a VLM planner and low-level VLA; reports 56.05% on RoboMME and 60.83% across four real-world manipulation tasks.*
  <a href="https://arxiv.org/abs/2610.29329"><img src="https://img.shields.io/badge/arxiv-2610.29329-silver" alt="Paper"></a>
  <a href="https://qinghangliu.github.io/pal-webpage/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/QinghangLiu/PAL_official"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>

Task decomposition, reusable skill orchestration, and task-time memory. Includes learned hierarchical planners and action models where applicable.
- AVALON: Zero-Shot Indoor Navigation with Human-Seeded Topological Memory — *Uses a human-seeded topological map and editable task memory to guide local navigation, verify semantic arrivals, and update physical-state records from robot evidence; evaluated on a quadruped in one office.*
  <a href="https://arxiv.org/abs/2610.21586"><img src="https://img.shields.io/badge/arxiv-2610.21586-silver" alt="Paper"></a>
- ChunkAct: Action Chunking for Agentic Robotics — *Compiles task knowledge into executable action chunks with typed failure exits, reducing planner calls while retaining feedback-driven replanning; evaluated on simulated manipulation benchmarks.*
  <a href="https://arxiv.org/abs/2610.18874"><img src="https://img.shields.io/badge/arxiv-2610.18874-silver" alt="Paper"></a>
- Gamma: Grounded Multi-Agent Memory with Mechanical Audit for Memory-Intensive Manipulation — *Combines grounded text memory, separate writer and reasoner agents, and mechanical verification of memory claims to guide a fixed subgoal-conditioned manipulation policy; evaluated in simulation.*
  <a href="https://arxiv.org/abs/2610.12793"><img src="https://img.shields.io/badge/arxiv-2610.12793-silver" alt="Paper"></a>
  <a href="https://github.com/1999Lyd/GAMMA"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/1999Lyd/GAMMA"><img src="https://img.shields.io/github/stars/1999Lyd/GAMMA" alt="stars"></a>
- REMM: Revisable Embodied Memory for Manipulation — *Maintains revisable task state backed by an append-only evidence log, withdraws dependent conclusions, and schedules verified recovery skills around a frozen robot policy; physical trials include operator assistance.*
  <a href="https://arxiv.org/abs/2610.12710"><img src="https://img.shields.io/badge/arxiv-2610.12710-silver" alt="Paper"></a>
  <a href="https://revanthsenthil.github.io/remm/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- RoboAware: Learning to Coordinate Embodied Skills from Counterfactual Outcomes — *Learns a state-conditioned coordinator from matched counterfactual simulator branches to route between modular skills and frozen end-to-end policies while a frozen coding agent generates local executable programs.*
  <a href="https://arxiv.org/abs/2610.11480"><img src="https://img.shields.io/badge/arxiv-2610.11480-silver" alt="Paper"></a>
- Proactive Robot Assistance via Event-Driven Reasoning over State Changes — *Triggers VLM reasoning from stable before-and-after scene states to infer assistance needs and select indexed robot primitives; physical tabletop evaluation counts clarification as an appropriate response alongside autonomous assistance.*
  <a href="https://arxiv.org/abs/2610.08344"><img src="https://img.shields.io/badge/arxiv-2610.08344-silver" alt="Paper"></a>
- OntoPlan: An Ontology-Grounded Scene Representation and Agentic Framework for Scalable Robot Task Planning — *Connects ontology-grounded scene retrieval and goal formalization to a symbolic planner through an agentic workflow; evaluates symbolic task planning in fully specified worlds rather than perception-to-action robot execution.*
  <a href="https://arxiv.org/abs/2610.07649"><img src="https://img.shields.io/badge/arxiv-2610.07649-silver" alt="Paper"></a>
  <a href="https://github.com/namhyeongwoo/OntoPlan"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/namhyeongwoo/OntoPlan"><img src="https://img.shields.io/github/stars/namhyeongwoo/OntoPlan" alt="stars"></a>
- Recursive Video In-Context Learning for Agentic Robot — *Exposes a demonstration as a hierarchy of keyframes, phases, moments, and clips that an agent retrieves through read-only tools while orchestrating a frozen VLA; evaluated on LIBERO in simulation.*
  <a href="https://arxiv.org/abs/2610.06843"><img src="https://img.shields.io/badge/arxiv-2610.06843-silver" alt="Paper"></a>
  <a href="https://bwr-hhh.github.io/rvicl/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/BWR-hhh/rvicl"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/BWR-hhh/rvicl"><img src="https://img.shields.io/github/stars/BWR-hhh/rvicl" alt="stars"></a>
- MarvisNav: Making Memory Visible on Route Choices for Zero-Shot Object Navigation — *Projects topological exploration states onto egocentric route choices for VLM-based object navigation, coupling visible memory with sparse high-level decisions; includes simulation evaluation and Go2 deployment demonstrations.*
  <a href="https://arxiv.org/abs/2610.06510"><img src="https://img.shields.io/badge/arxiv-2610.06510-silver" alt="Paper"></a>
  <a href="https://wangjincheng1998.github.io/MarvisNav/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- Beyond the Remembered World: Predictive 4D Belief for Persistent Navigation in Evolving Worlds — *A frozen VLM invokes temporal-memory, prediction, inspection, and navigation tools to search for targets whose locations change; evaluated in simulation and matched physical-robot trials, with gains strongest under learnable routines.*
  <a href="https://arxiv.org/abs/2609.39166"><img src="https://img.shields.io/badge/arxiv-2609.39166-silver" alt="Paper"></a>
  <a href="https://zju4embodiedai.github.io/EvolvingNav/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/ZJU4EmbodiedAI/EvolvingNav"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/ZJU4EmbodiedAI/EvolvingNav"><img src="https://img.shields.io/github/stars/ZJU4EmbodiedAI/EvolvingNav" alt="stars"></a>
- AgenticNav: Zero-Shot Vision-and-Language Navigation as a Tool-Calling Harness — *Exposes pixel-target actions, on-demand depth queries, and selective visual memory recall as tools for a VLM navigation agent; evaluated in VLN-CE and on two physical robot platforms.*
  <a href="https://arxiv.org/abs/2606.10577"><img src="https://img.shields.io/badge/arxiv-2606.10577-silver" alt="Paper"></a>
- NavHarness: Adaptive Goals for Agentic Vision-Language Navigation — *Four agents coordinate goal generation, verification, memory, and visuomotor execution, compressing navigation history at verified goal boundaries; evaluated on 24 real-robot route trials.*
  <a href="https://arxiv.org/abs/2609.39915"><img src="https://img.shields.io/badge/arxiv-2609.39915-silver" alt="Paper"></a>
  <a href="https://Navharness.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- RoboHarness: Memory-Driven Orchestration of Heterogeneous Robot Policies for Long-Horizon Planning — *An agentic orchestration layer exposes heterogeneous robot policies as reusable skills, using execution evidence and memory to route tasks and bridge policy handoffs without joint retraining; simulation and real-robot evaluation.*
  <a href="https://arxiv.org/abs/2607.18060"><img src="https://img.shields.io/badge/arxiv-2607.18060-silver" alt="Paper"></a>
  <a href="https://www.robo-harness.com/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- Simple Agentic Memory for Generalist Robot Policies — *SimpleARM; a training-free external memory layer maintains task-relevant typed state, retrieves history-dependent information, and re-grounds recalled entities for frozen robot policies; evaluated on RoboMME.*
  <a href="https://arxiv.org/abs/2609.36595"><img src="https://img.shields.io/badge/arxiv-2609.36595-silver" alt="Paper"></a>
  <a href="https://simplearm.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- NavJev: Efficient Vision-Language Navigation via Action-Centric Visual Compression and Discriminative Action-Semantic Memory — *Action-centric visual compression and discriminative action-semantic memory support typed Jev decisions for vision-language navigation, evaluated in R2R-CE and two real indoor environments.*
  <a href="https://arxiv.org/abs/2609.34969"><img src="https://img.shields.io/badge/arxiv-2609.34969-silver" alt="Paper"></a>
  <a href="https://kai-sheng-caesar.github.io/NavJev/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
Cross-cutting reasoning/action coupling and System 1/System 2 designs are listed under [Reasoning-Acting and Dual-System Architectures](#reasoning-acting-and-dual-system-architectures).
- Actively Resolving Contextual Uncertainty for Underspecified Tasks in Natural Language — *CLUE; an LLM agent resolves ambiguous goals through map queries, inspection, navigation, and manipulation skills, with closed-loop evaluation on a physical Spot robot.*
  <a href="https://arxiv.org/abs/2609.30428"><img src="https://img.shields.io/badge/arxiv-2609.30428-silver" alt="Paper"></a>
  <a href="https://zacravichandran.github.io/CLUE/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- NavProbe: Evidence-Grounded Reasoning with Active Memory Retrieval for Zero-Shot Navigation — *A hierarchical VLM navigation agent that retrieves visual and geometric evidence to revise subgoals and select parameterized navigation skills.*
  <a href="https://arxiv.org/abs/2609.27526"><img src="https://img.shields.io/badge/arxiv-2609.27526-silver" alt="Paper"></a>
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
- CarryOn: A Dual-Loop Harness for Personalized and Reliable Robot Assistance — *Augments a frozen VLA with revisable user and scene memory, geometric action shielding, and reusable recovery skills refined through reflection; evaluated in simulation and targeted physical-robot studies.*
  <a href="https://arxiv.org/abs/2610.21453"><img src="https://img.shields.io/badge/arxiv-2610.21453-silver" alt="Paper"></a>
  <a href="https://vincent2311.github.io/Projects/CarryOn/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/JIA-Lab-research/CarryOn" title="Repository available; code release pending"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/JIA-Lab-research/CarryOn"><img src="https://img.shields.io/github/stars/JIA-Lab-research/CarryOn" alt="stars"></a>
- Cracking Mobile Manipulation: From Failure Diagnosis to Agentic Robot System — *Diagnoses long-horizon mobile-manipulation failures and adds demonstration-based skills, adaptive visual memory, base positioning, and end-effector corrections around a fixed subtask VLA; simulation and physical evaluation.*
  <a href="https://arxiv.org/abs/2610.19600"><img src="https://img.shields.io/badge/arxiv-2610.19600-silver" alt="Paper"></a>
  <a href="https://github.com/PKU-VaLuE-Lab/Cracking-Mobile-Manipulation" title="Repository available; code release pending"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/PKU-VaLuE-Lab/Cracking-Mobile-Manipulation"><img src="https://img.shields.io/github/stars/PKU-VaLuE-Lab/Cracking-Mobile-Manipulation" alt="stars"></a>
- ParallelWorld: Test-Time Scaling for Agentic Embodied Reasoning — *Uses verifier-guided search over imagined outcomes of executable primitives, then executes one action and replans; evaluated on embodied understanding and simulated manipulation, with additional test-time computation.*
  <a href="https://arxiv.org/abs/2608.22971"><img src="https://img.shields.io/badge/arxiv-2608.22971-silver" alt="Paper"></a>
  <a href="https://agenticei.github.io/ParallelWorld-page/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/AgenticEI/ParallelWorld"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/AgenticEI/ParallelWorld"><img src="https://img.shields.io/github/stars/AgenticEI/ParallelWorld" alt="stars"></a>
- Recova: Agent-Guided Failure Recovery for Autonomous Robotic Manipulation — *An agent develops recovery programs in a digital twin and monitors, restores, verifies, and resumes robot tasks; real-world experience and human demonstrations improve separate task and recovery policies.*
  <a href="https://arxiv.org/abs/2610.01178"><img src="https://img.shields.io/badge/arxiv-2610.01178-silver" alt="Paper"></a>
  <a href="https://www.liuisabella.com/Recova"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
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

- RoboDuo: Attempt, Check and Atomic Recovery through Code for Vision-Language-Action Models — *A coding agent checks full-task VLA completion and delegates remaining atomic steps to a second VLA; the agent itself emits no robot actions.*
  <a href="https://arxiv.org/abs/2610.34108"><img src="https://img.shields.io/badge/arxiv-2610.34108-silver" alt="Paper"></a>
- RetroNav: Scene-Grounded Retrospection and Retry for Self-Evolving Lifelong Navigation — *Grounds retry briefs in accumulated scene evidence and prior navigation episodes; arXiv says the code will be released.*
  <a href="https://arxiv.org/abs/2610.35172"><img src="https://img.shields.io/badge/arxiv-2610.35172-silver" alt="Paper"></a>
- Which Hand Was Late? Diagnosis for Robot Failure Recovery in Bimanual Tool Use — *Studies what sensing can identify about bimanual failures and uses an escalation-based repair policy; evaluated in simulation.*
  <a href="https://arxiv.org/abs/2610.37533"><img src="https://img.shields.io/badge/arxiv-2610.37533-silver" alt="Paper"></a>
- Refuses When Asked, Complies When Acting: A Runtime Safety Check for Robot Control Loops — *Adds a pre-motion hazard check to a tool-driven robot harness; small physical study found hazardous instructions were blocked in 15/15 trials.*
  <a href="https://arxiv.org/abs/2610.27350"><img src="https://img.shields.io/badge/arxiv-2610.27350-silver" alt="Paper"></a>

#### Multi-Robot Coordination
- UAV-SwarmAgent: Scalable Multi-UAV Reconnaissance and Task Allocation via Code Generation and Vision-Language Reasoning — *A ground-station agent converts a natural-language mission into executable per-UAV routes, assigns work by route cost, and dispatches worker agents for incident verification; simulation reports 244/255 detections and a speedup capped at 1.52× for five UAVs.*
  <a href="https://arxiv.org/abs/2610.32559"><img src="https://img.shields.io/badge/arxiv-2610.32559-silver" alt="Paper"></a>
- Policy Search in Code Space for Multi-Agent Pathfinding — *Human-directed coding agents propose, implement, test, and verify policy code in simulation; v2 reports higher performance on MAPF and warehouse throughput, an offline algorithm-discovery workflow rather than inference-time robot control.*
  <a href="https://arxiv.org/abs/2610.25946"><img src="https://img.shields.io/badge/arxiv-2610.25946-silver" alt="Paper"></a>
- CoEvolve: Self-Evolving Code Policies from Skills to Strategies for Humanoid Robots — *Evolves executable coordination code over fixed motor skills using physical verification and retained experience; reports 8 completed tasks across 15 base runs with two simulated Unitree G1 robots, while contact stability remains limited.*
  <a href="https://arxiv.org/abs/2610.23288"><img src="https://img.shields.io/badge/arxiv-2610.23288-silver" alt="Paper"></a>

Task allocation, communication, and organizational structures for teams of robots or embodied agents. ORCH is evaluated in simulation; system-level runtimes are listed under [Embodied Agent Operating Systems and Runtimes](#embodied-agent-operating-systems-and-runtimes).
- Persistent LLM Orchestration of Heterogeneous Robot Teams via Partial Delegation to Multi-Agent Protocols — *Maintains a compact semantic world state and delegates routine coordination to multi-agent protocols while selectively re-engaging an LLM for changing rescue tasks; evaluated in abstract heterogeneous-team simulations.*
  <a href="https://arxiv.org/abs/2610.15224"><img src="https://img.shields.io/badge/arxiv-2610.15224-silver" alt="Paper"></a>
- Verifier-Mediated Multi-LLM Coordination for Multi-Robot Path Planning — *Coordinates robot-specific language-model plans through geometric conflict checks and structured replanning feedback; studied in CARLA scenarios with a physical quadrotor demonstration.*
  <a href="https://arxiv.org/abs/2610.12761"><img src="https://img.shields.io/badge/arxiv-2610.12761-silver" alt="Paper"></a>
- Managing Context and Communication in Distributed Agentic UAV Swarms — *Combines local language-model agents, structured note memory, and deterministic interest-aware gossip for distributed UAV coordination; evaluated with ten UAVs in simulated search and rescue.*
  <a href="https://arxiv.org/abs/2610.01569"><img src="https://img.shields.io/badge/arxiv-2610.01569-silver" alt="Paper"></a>
- DuoMind: Enabling Distributed Multi-Robot Coordination with Semantic Communication — *Distributed VLM orchestrators exchange semantic messages and guide fine-tuned VLA controllers through language, evaluated on two-agent RoboPoly and RoboTwin manipulation tasks in simulation.*
  <a href="https://arxiv.org/abs/2610.02161"><img src="https://img.shields.io/badge/arxiv-2610.02161-silver" alt="Paper"></a>
  <a href="https://hanchuzhou.github.io/duomind_project_page/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://huggingface.co/datasets/ucd-dare/robopoly_demo" title="Dataset"><img src="https://img.shields.io/badge/huggingface-yellow" alt="huggingface"></a>
- Systematic Multi-Agent Vision-and-Language Navigation: Formulation, Benchmark, and Method — *MAVLN and TRISS; constrained multi-agent navigation with an LLM subtask scheduler, shared topological memory, and conflict-aware execution, evaluated in simulated scenes.*
  <a href="https://arxiv.org/abs/2609.35965"><img src="https://img.shields.io/badge/arxiv-2609.35965-silver" alt="Paper"></a>
  <a href="https://xyz9911.github.io/mavln/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
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
- WorldMirror: Agentic Real-to-Sim Generation of Interactive Worlds from In-the-Wild Robot Demonstrations — *A coding agent orchestrates scene and 3D-generation tools to build an executable world program, then uses verification feedback to refine interactive digital twins and replay recorded robot trajectories; evaluated on DROID demonstrations.*
  <a href="https://arxiv.org/abs/2610.31834"><img src="https://img.shields.io/badge/arxiv-2610.31834-silver" alt="Paper"></a>
- JARVIS: From Visual Manuals to Autonomous Robotic Assembly — *A benchmark for interpreting visual assembly manuals and executing long-horizon procedures; JARVIS-agentic composes robot primitives into executable programs with feedback-based verification and recovery, without task-specific trajectories or parameter updates.*
  <a href="https://arxiv.org/abs/2610.27618"><img src="https://img.shields.io/badge/arxiv-2610.27618-silver" alt="Paper"></a>
- Alpha: Systematic Fault Injection and Robustness Evaluation for LLM-Driven Embodied Manipulation — *Injects perception, actuation, kinematic, and planner-output faults to distinguish physical failures from planner/interface errors; a 150-episode simulation study found the measured LLM gap came from output corruption, not the matched physical/kinematic faults.*
  <a href="https://arxiv.org/abs/2610.30197"><img src="https://img.shields.io/badge/arxiv-2610.30197-silver" alt="Paper"></a>
  <a href="https://github.com/jonajoy142/alpha-embodied-robustness"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
- Embodied Playground: A Long-Horizon Agentic Robotics Benchmark for Physical, Strategic, and Spatial Reasoning — *Tests the full loop of observation, tool use, control-code generation, and independent success/validity checks across 410 task environments; its EP-100 subset covers five suites and 16 task types.*
  <a href="https://arxiv.org/abs/2610.27039"><img src="https://img.shields.io/badge/arxiv-2610.27039-silver" alt="Paper"></a>
  <a href="https://winniechen2002.github.io/Agent-bench-website/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/Winniechen2002/Embodied-Playground"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
- TARSphere: A Robot-Oriented Full-Stack Framework for Long-Horizon Embodied Agents in Evolving Physical and Social Environments — *A full-stack benchmark for embodied agents across evolving physical and social environments, with 360 episodes in 30 indoor scenes; evaluates long-horizon interaction, adaptation, and human coordination while exposing safety and robustness limits.*
  <a href="https://arxiv.org/abs/2610.30043"><img src="https://img.shields.io/badge/arxiv-2610.30043-silver" alt="Paper"></a>
  <a href="https://xuyicheng-zju.github.io/TARSphere/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/xuyicheng-zju/TARSphere"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
- HandsOn: A Large-Scale Simulation Benchmark for Generalizable Dexterous Manipulation — *A cross-embodiment manipulation benchmark that includes prompted GPT-6 with move_eef tool control as a zero-shot baseline (5.2% Core-50 and 1.9% Transfer-16 over 660 trials); most of the paper studies trained policies, and qualitative robot rollouts do not establish broad real-world generalization.*
  <a href="https://arxiv.org/abs/2610.26765"><img src="https://img.shields.io/badge/arxiv-2610.26765-silver" alt="Paper"></a>
- RoboBugBench: Benchmarking Automated Repair of Real Robot Software Under an Audited Behavioral Oracle — *Tests coding agents on 33 execution-validated ROS 2 defects; simulation behavior rather than unit tests grades repairs, and the authors identify important false-acceptance limits in the shipped oracle.*
  <a href="https://arxiv.org/abs/2610.16369"><img src="https://img.shields.io/badge/arxiv-2610.16369-silver" alt="Paper"></a>
- System1-Arena: Which Decisions Can Be Left to System 1? — *Evaluates typed-decision models including Jev on static questions and mixed-domain closed loops, with simulated robotics interfaces and a latency-aware protocol; separates local decision accuracy from end-to-end success.*
  <a href="https://arxiv.org/abs/2610.21244"><img src="https://img.shields.io/badge/arxiv-2610.21244-silver" alt="Paper"></a>
  <a href="https://tianyucodings.github.io/S1-Arena"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/TianyuCodings/S1-Arena"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/TianyuCodings/S1-Arena"><img src="https://img.shields.io/github/stars/TianyuCodings/S1-Arena" alt="stars"></a>
- SEAR: Self-Evolving Agentic Robotics — *A framework and benchmark for code-as-policy, live agent control, and agent-driven policy research, with controls for interaction budgets, repeated attempts, and reusable experience across simulated and physical tasks.*
  <a href="https://arxiv.org/abs/2610.18792"><img src="https://img.shields.io/badge/arxiv-2610.18792-silver" alt="Paper"></a>
  <a href="https://sear.bot/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/Self-Evolving-Agentic-Robotics/SEAR" title="Repository available; code release pending"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/Self-Evolving-Agentic-Robotics/SEAR"><img src="https://img.shields.io/github/stars/Self-Evolving-Agentic-Robotics/SEAR" alt="stars"></a>
- Towards a Systematic Study of Embodied System 2 over Full Task Execution Cycles — *Studies embodied System 2 across full task cycles using evidence memory, progress verification, and dynamic agendas, with simulation and offline next-action evaluation on recorded robot demonstrations.*
  <a href="https://arxiv.org/abs/2610.17657"><img src="https://img.shields.io/badge/arxiv-2610.17657-silver" alt="Paper"></a>
  <a href="https://vfishc.github.io/scoper/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- Embodied Skill Bench: Benchmarking How Well Agents with Embodied Skills Perform on Physical Tasks — *Benchmarks reusable embodied skills and adaptive delegation in simulated manipulation, including a separate Jev waypoint skill that exposes a success–latency trade-off when paired with a frontier VLM.*
  <a href="https://arxiv.org/abs/2610.16238"><img src="https://img.shields.io/badge/arxiv-2610.16238-silver" alt="Paper"></a>
  <a href="https://github.com/HanZhi306/EmbodiedSkill-Bench"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/HanZhi306/EmbodiedSkill-Bench"><img src="https://img.shields.io/github/stars/HanZhi306/EmbodiedSkill-Bench" alt="stars"></a>
- MAGMA-Bench: Evaluating Long-Horizon Embodied Agents under Dynamic Tasks and Execution Failures — *Benchmarks long-horizon skill-calling agents under changing goals, asynchronous multi-robot execution, and controlled failures using structured task-level simulation; abstracts away raw perception and low-level motor control.*
  <a href="https://arxiv.org/abs/2610.13534"><img src="https://img.shields.io/badge/arxiv-2610.13534-silver" alt="Paper"></a>
  <a href="https://magma-rob.github.io/magma-bench"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/MAGMA-rob/magma-bench"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/MAGMA-rob/magma-bench"><img src="https://img.shields.io/github/stars/MAGMA-rob/magma-bench" alt="stars"></a>
- RESCUE: Is This Alarm Worth Acting On? Counterfactual Evaluation of VLA Runtime Monitors — *Evaluates robot runtime alarms by restoring simulator and policy state and comparing counterfactual interventions, measuring whether acting on an alarm improves outcomes rather than detection accuracy alone.*
  <a href="https://arxiv.org/abs/2610.13516"><img src="https://img.shields.io/badge/arxiv-2610.13516-silver" alt="Paper"></a>
- EmbodiedCLBench: Evaluating Continual Learning for Self-Evolving Embodied Agents — *Evaluates whether coding-agent harnesses transfer interaction histories or distilled skill summaries from basic to composed tasks on offline embodied state-transition graphs; does not evaluate live physical control or continual weight updates.*
  <a href="https://arxiv.org/abs/2610.13021"><img src="https://img.shields.io/badge/arxiv-2610.13021-silver" alt="Paper"></a>
  <a href="https://pku-value-lab.github.io/EmbodiedCLBench-homepage/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/PKU-VaLuE-Lab/EmbodiedCLBench"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/PKU-VaLuE-Lab/EmbodiedCLBench"><img src="https://img.shields.io/github/stars/PKU-VaLuE-Lab/EmbodiedCLBench" alt="stars"></a>
- What Should Embodied Agents Remember? Benchmarking and Evaluating Memory Modality for Embodied Agents — *Benchmarks memory representations and their inference costs for embodied agents using fixed observation histories followed by memory-dependent requests; includes limited physical delivery demonstrations.*
  <a href="https://arxiv.org/abs/2610.12561"><img src="https://img.shields.io/badge/arxiv-2610.12561-silver" alt="Paper"></a>
- BiGym 2.0: Benchmarking Learned and Agent-Developed Policies for Humanoid Household Manipulation — *Benchmarks learned policies and cold-start coding-agent programs on simulated G1 household manipulation under a shared whole-body controller, with 20 tasks and native VR demonstrations; the principal comparison covers nine tasks.*
  <a href="https://arxiv.org/abs/2610.07594"><img src="https://img.shields.io/badge/arxiv-2610.07594-silver" alt="Paper"></a>
- SharedKV-BT: Node-Local Typed Decisions for Behavior-Tree Agents — *Combines node-local typed candidate scoring with behavior-tree stage gating and external postcondition checks; studies simulated robot manipulation and navigation alongside fixed computer-use tasks, without physical-robot validation.*
  <a href="https://arxiv.org/abs/2610.07327"><img src="https://img.shields.io/badge/arxiv-2610.07327-silver" alt="Paper"></a>
- RobotWorld: Benchmarking Multimodal Agents for Robot Use Across Diverse Tasks and Embodiments — *Benchmarks multimodal agents through robot interfaces across 84 simulated tasks and diverse embodiments, with explicit interaction budgets and executable success checks; reports outcomes and execution-trace limitations.*
  <a href="https://arxiv.org/abs/2610.10409"><img src="https://img.shields.io/badge/arxiv-2610.10409-silver" alt="Paper"></a>
  <a href="https://robotworldai.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/robotworldai/robotworld"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/robotworldai/robotworld"><img src="https://img.shields.io/github/stars/robotworldai/robotworld" alt="stars"></a>

Jev+Robot

- robo-jev: A 10 Hz Typed-Decision Layer for Physical Robots — *A typed decision layer with deterministic execution; its R13 simulation audit passed a registered comparison after delegating gripper, path, and force choices to rules, while semantic and stop failures remain.*
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
- robojev: Natural-Language Control of a WidowX AI Arm with Jev Typed Judgments — *A real-hardware prototype using typed Jev decisions to sequence reusable manipulation primitives; reported demonstrations are heavily fitted to one paper cup and one table.*
  <a href="https://github.com/alee792/robojev"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/alee792/robojev"><img src="https://img.shields.io/github/stars/alee792/robojev" alt="stars"></a>

Robot integration, deployment, latency, runtime reliability, and evaluation of model-plus-interface systems. Includes benchmarks for memory, safety, and recovery, as well as surveys of robot policy verification.
  - RoboQuest: Generalist Physical Agents that Search, Inspect and Test — *Evaluates information-seeking mobile-manipulation agents on ten simulated search, inspection, and interactive-testing tasks, separating missing evidence and premature commitment from execution failures.*
  <a href="https://arxiv.org/abs/2610.10388"><img src="https://img.shields.io/badge/arxiv-2610.10388-silver" alt="Paper"></a>
  <a href="https://declare-lab.github.io/RoboQuest/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/declare-lab/RoboQuest"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/declare-lab/RoboQuest"><img src="https://img.shields.io/github/stars/declare-lab/RoboQuest" alt="stars"></a>
- Are Frontier VLM Agents Ready to Be Robot Generalists? An Empirical Study with the Embodied Agent Arena — *Evaluates seven VLM agents across 1,000 cases spanning geometry, spatial reasoning, affordance, planning, and manipulation, separating local competence from complete task success under source-specific interfaces.*
  <a href="https://arxiv.org/abs/2610.00854"><img src="https://img.shields.io/badge/arxiv-2610.00854-silver" alt="Paper"></a>
  <a href="https://embodied-agent-arena.github.io/embodied-agent-arena/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/embodied-agent-arena/embodied-agent-arena"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/embodied-agent-arena/embodied-agent-arena"><img src="https://img.shields.io/github/stars/embodied-agent-arena/embodied-agent-arena" alt="stars"></a>
- DrivingBench: Can Vision-Language Models Drive a Toyota Corolla? — *A physical-vehicle benchmark exposing three MCP tools to vision-language models, evaluated at parking-lot speeds with a supervising safety driver and bounded retry attempts.*
  <a href="https://arxiv.org/abs/2609.38948"><img src="https://img.shields.io/badge/arxiv-2609.38948-silver" alt="Paper"></a>
  <a href="https://drivingbench.com"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/aditya-ramabadran/drivingbench_harness_v1"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/aditya-ramabadran/drivingbench_harness_v1"><img src="https://img.shields.io/github/stars/aditya-ramabadran/drivingbench_harness_v1" alt="stars"></a>
- LIBERO-Agent: Evaluating General-Purpose Agents for Direct Embodied Manipulation — *An agent-native manipulation benchmark with evaluator-owned state and success checks; the public source release provides the 30-task primary suite, while the broader catalog is reserved for a later release.*
  <a href="https://arxiv.org/abs/2609.39507"><img src="https://img.shields.io/badge/arxiv-2609.39507-silver" alt="Paper"></a>
  <a href="https://github.com/dzj441/Libero-Agent"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/dzj441/Libero-Agent"><img src="https://img.shields.io/github/stars/dzj441/Libero-Agent" alt="stars"></a>
- RLE-Bench: A Qualifying Exam for Coding Agents as Robot Learning Engineers — *Evaluates coding agents across interactive robot control, policy development, perception and estimation, and mechanical design under explicit resource budgets and independent artifact evaluation.*
  <a href="https://arxiv.org/abs/2609.34210"><img src="https://img.shields.io/badge/arxiv-2609.34210-silver" alt="Paper"></a>
  <a href="https://rle-bench.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/RLE-Bench/RLE-Bench"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/RLE-Bench/RLE-Bench"><img src="https://img.shields.io/github/stars/RLE-Bench/RLE-Bench" alt="stars"></a>
- EmbodiedSWE: Coding Agents for Long Horizon Dexterous Robotics — *A simulation benchmark for coding agents and a pipeline that diversifies verified solutions into demonstrations for robot policy learning.*
  <a href="https://arxiv.org/abs/2609.27308"><img src="https://img.shields.io/badge/arxiv-2609.27308-silver" alt="Paper"></a>
  <a href="https://embodiedswe.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/EmbodiedSWE/EmbodiedSWE"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/EmbodiedSWE/EmbodiedSWE"><img src="https://img.shields.io/github/stars/EmbodiedSWE/EmbodiedSWE" alt="stars"></a>
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

- RobotAgentBench: Towards Open-world Robot Autonomy — *Evaluates task discovery, contextual reasoning, manipulation, and recovery across 50 household layouts; the benchmark evaluation is simulation-based.*
  <a href="https://arxiv.org/abs/2610.34649"><img src="https://img.shields.io/badge/arxiv-2610.34649-silver" alt="Paper"></a>
  <a href="https://aetherlabsai.github.io/RobotAgentBench/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/AetherLabsAI/RobotAgentBench"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
- EmbodiedLab: Benchmarking Embodied Agents That Act to Know — *A physics-based simulated laboratory benchmark for agents that choose experiments and operate apparatus to discover unknown outcomes.*
  <a href="https://arxiv.org/abs/2610.35385"><img src="https://img.shields.io/badge/arxiv-2610.35385-silver" alt="Paper"></a>
  <a href="https://hexafuture.ai/benchmarks/embodiedlab/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/HexaFuture/EmbodiedLab"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
- SceneAgent: An Agentic Pipeline from 3D and 4D Captures to Simulation Environments — *Uses simulator inspection and repair to turn static and dynamic captures into interactive, policy-learning scenes; real-robot transfer is preliminary.*
  <a href="https://arxiv.org/abs/2610.34745"><img src="https://img.shields.io/badge/arxiv-2610.34745-silver" alt="Paper"></a>
- SceneRig: An Agentic System for Simulation-Ready 3D Scene Reconstruction from Single Images — *Uses simulator edit-and-validate loops to produce physically stable scenes from single images; a CoRL 2026 Agentic Robotics Workshop paper.*
  <a href="https://arxiv.org/abs/2610.28585"><img src="https://img.shields.io/badge/arxiv-2610.28585-silver" alt="Paper"></a>
  <a href="https://red-fairy.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>

### Perspectives and Reports
- Can AI Agents Help Robotic Engineers? Lessons from Two Focus Days in Industry — *A small industrial case study finds no general productivity gain from AI coding agents in vendor-specific robot programming beyond repetitive-code tasks, and highlights the learning curve and need for domain adaptation.*
  <a href="https://arxiv.org/abs/2610.32636"><img src="https://img.shields.io/badge/arxiv-2610.32636-silver" alt="Paper"></a>

These are essays, research blogs, and evaluations; they are listed separately from papers.
- The Bitter Lesson Comes to Robotics — *Compares nine frontier multimodal models on six physical manipulation tasks; v2 reports rapid July–October 2026 capability growth while concluding that the systems still miss practical action-budget requirements.*
  <a href="https://arxiv.org/abs/2610.25287"><img src="https://img.shields.io/badge/arxiv-2610.25287-silver" alt="Paper"></a>
- Has GPT-6-Astra Achieved Embodied Intelligence? — *A v2 report evaluates GPT-6-Astra across 12 benchmarks and eight robot configurations, examining in-context demonstrations, System 2/System 1 harnesses, real-world limits, and benchmark design.*
  <a href="https://arxiv.org/abs/2610.22471"><img src="https://img.shields.io/badge/arxiv-2610.22471-silver" alt="Paper"></a>
- Toward Recursive Self-Improvement in Physical AI — *A survey separates behavioral gains from genuine improvement of the learning procedure and improver, and proposes controlled two-round tests; it concludes that existing physical studies have not isolated gains attributable to recursion.*
  <a href="https://arxiv.org/abs/2610.29677"><img src="https://img.shields.io/badge/arxiv-2610.29677-silver" alt="Paper"></a>
  <a href="https://physical2rsi.github.io/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
  <a href="https://github.com/Physical2RSI/Awesome-Physical2RSI"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
- Multimodal Embodied Agents: A Unified Capability-centric Perspective from Computer-Use to Robot-Use — *Organizes embodied agents around Perceive, Anticipate, Plan, Act, and Verify (PAPAV), comparing computer-use and robot-use systems and auditing benchmark coverage; a useful taxonomy rather than a new method.*
  <a href="https://arxiv.org/abs/2610.30108"><img src="https://img.shields.io/badge/arxiv-2610.30108-silver" alt="Paper"></a>
  <a href="https://showlab.github.io/Awesome-Multimodal-Embodied-Agent/"><img src="https://img.shields.io/badge/-project-blue" alt="Project"></a>
- Towards Agentic Robots: Model, Data, Environment, and Harness — *A survey organizing agentic robotics across model, data, environment, and harness functions, covering how agents develop robot capabilities and orchestrate their use.*
  <a href="https://arxiv.org/abs/2610.20442"><img src="https://img.shields.io/badge/arxiv-2610.20442-silver" alt="Paper"></a>
  <a href="https://github.com/chonghanqin/Awesome-Agentic-Robots"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/chonghanqin/Awesome-Agentic-Robots"><img src="https://img.shields.io/github/stars/chonghanqin/Awesome-Agentic-Robots" alt="stars"></a>
- Who Improves the Robot? Toward Physical Recursive Self-Improvement — *A survey and perspective distinguishing improvements to robot capabilities from improvements to the improvement process itself, with an emphasis on agent harnesses, verification, and evidence for physical recursive self-improvement.*
  <a href="https://arxiv.org/abs/2610.18842"><img src="https://img.shields.io/badge/arxiv-2610.18842-silver" alt="Paper"></a>
  <a href="https://github.com/SAIL-Research-Lab/Physical-RSI"><img src="https://img.shields.io/badge/-github-teal?logo=github" alt="github"></a>
  <a href="https://github.com/SAIL-Research-Lab/Physical-RSI"><img src="https://img.shields.io/github/stars/SAIL-Research-Lab/Physical-RSI" alt="stars"></a>
- When Faster Decisions Do Not Make Better Agents: An Empirical Study of Jev in Agent Workflows — *An empirical study of Jev-based action selection in text-only ALFWorld and AndroidWorld, separating cheaper decisions from task success, recovery, and cost per successful outcome; no physical-robot experiments.*
  <a href="https://arxiv.org/abs/2610.13092"><img src="https://img.shields.io/badge/arxiv-2610.13092-silver" alt="Paper"></a>
- Silicon Language: A Robot-Native Knowledge Exchange Framework for Heterogeneous Robots — *Proposes robot-native knowledge packets for cross-embodiment exchange, with an operator-assisted laboratory proof of concept; autonomous fleet exchange and general skill transfer remain unvalidated.*
  <a href="https://arxiv.org/abs/2610.07650"><img src="https://img.shields.io/badge/arxiv-2610.07650-silver" alt="Paper"></a>
- What Stops Recursive Self-Improvement in Robotics? Lessons from 123 Rounds of Agentic Skill Discovery — *Technical report; a simulation case study of agent-driven skill discovery, exposing perception, evaluation, and memory bottlenecks despite 123 improvement rounds without success on the primary target task.*
  <a href="https://arxiv.org/abs/2609.31760"><img src="https://img.shields.io/badge/arxiv-2609.31760-silver" alt="Paper"></a>
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
- Profiling a Frontier Agent with EBench: From Direct Control to Harness with Policy — *Compares a frontier agent issuing direct waypoints with a tool harness that invokes post-trained policies, including long-horizon and contact-rich failure modes.*
  <a href="https://arxiv.org/abs/2610.35832"><img src="https://img.shields.io/badge/arxiv-2610.35832-silver" alt="Paper"></a>

