# Jiho Kang

Mechanical & Automotive Engineering student at Seoul National University of Science and Technology

I am interested in building reliable systems that connect data, learning, and physical interaction. My current interests include **Data Engineering**, **Robotics**, **Physical AI**, and **AI/ML Systems**.

## About Me

- **Major:** Mechanical & Automotive Engineering
- **University:** Seoul National University of Science and Technology
- **Focus areas:** Robot learning and policy improvement, simulation-to-controller interfaces, and practical ML workflows
- **Tools and technologies:** Python, C, Linux, Git, Docker, MATLAB, and Simulink

## Tech Stack

| Area | Technologies and tools |
| --- | --- |
| Programming & systems | Python, C, Linux, Git, Docker |
| Modeling & control | MATLAB, Simulink |
| Robotics & simulation | BEHAVIOR-1K, OmniGibson, RoboCasa365 |
| Learning & experimentation | VLA, JAX, Flax, Weights & Biases (W&B) |

## Selected Projects

### KIST — RHO-based Robot Policy Improvement

Explored an iterative workflow for improving robot policies from simulation rollouts. The workflow used robot, object, fixture, and joint states together with execution traces to locate failures and analyze likely causes. A coding agent iteratively revised policy code and motion strategies, progressing from atomic tasks toward long-horizon tasks.

Evaluation considered success rate, convergence, rollout and API cost, and generalization across initial states. The oracle results below are task-specific simulation results; they do not represent real-robot performance.

| Task | VLA 30EP | Oracle 30EP | Oracle 100EP |
| --- | ---: | ---: | ---: |
| TurnOnMicrowave | 18/30 | 30/30 | 100/100 |
| OpenDishwasher | 19/30 | 30/30 | 100/100 |
| CloseCabinet | 21/30 | 30/30 | 97/100 |

Real-robot application remains future work.

### BEHAVIOR-1K Capstone — XR-1 × R1Pro Interface

Built and validated an interface path between BEHAVIOR observations and an XR-1 policy with an R1Pro controller:

- Implemented a BEHAVIOR observation-to-XR-1 input adapter.
- Loaded an XR-1 checkpoint and verified GPU forward inference.
- Implemented an ActionBridge from XR-1's 60D action to R1Pro's 21D action.
- Converted end-effector coordinates from the local frame to the controller frame.
- Passed actual XR-1 outputs through to `OmniGibson env.step()`.

Full-body closed-loop task success has not yet been achieved.

### BEHAVIOR-1K VLA Policy Training

- Implemented and trained a VLA model, with model-size and workflow choices shaped by limited GPU resources.
- Set up training, checkpointing, and W&B logging workflows.
- Built an A100–RTX5070 rollout pipeline.
- Analyzed out-of-distribution freezing, repetitive behavior, and action-scale issues.

### Kaggle — Pig Posture Recognition

Trained a ConvNeXt-based classifier and worked on data splitting, augmentation, and inference optimization.

- **Public F1 progression:** 0.915 → 0.925 → 0.930 → 0.944 → 0.948
- **Individual:** 26/123
- **Team:** 16/123

### Active Roll Control

Used MATLAB/Simulink to develop and evaluate an observer and PD controller.

- **Maximum roll angle:** 3.3862° → 0.9795° (**−71.07%**)
- **Roll gradient:** 6.7738°/g → 0.6474°/g (**−90.44%**)

## Problem Solving Approach

**Observe → Analyze → Identify Cause → Modify → Validate**

I use this loop to turn system behavior into testable changes, then check those changes against measurable outcomes.

## Portfolio

[View my portfolio (PDF)](portfolio/Jiho_Kang_Portfolio.pdf)

## Contact

- **GitHub:** [YOUR_GITHUB_ID](https://github.com/YOUR_GITHUB_ID)
- **Email:** [YOUR_EMAIL](mailto:YOUR_EMAIL)


