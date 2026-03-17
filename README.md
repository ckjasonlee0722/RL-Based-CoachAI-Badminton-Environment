# My Contribution to CoachAI+: Baseline RL Development

This repository is a project showcase of my contribution to the broader **CoachAI+ Badminton Environment** project developed at **NYCU ADSL**.

Rather than re-releasing the full CoachAI+ system, this repository focuses on the part of the project that my teammates and I worked on: **baseline reinforcement learning development and environment-level experimentation for badminton rally simulation**.

## Project Context

CoachAI+ is a larger badminton AI project that includes:

- interactive badminton simulation environments
- learned player models
- tactical and shot evaluation modules
- visualization and web-based interfaces

This repository highlights a specific subproject built on top of that broader system.

## My Contribution

My teammates and I worked on baseline RL development for the badminton environment, including:

- implementing and experimenting with **PDQN**, **Hybrid PPO**, and **Hybrid SAC**
- integrating these agents into the **CoachAI+ badminton environment**
- using **RallyNet** as a learned opponent model
- studying **reward design**, **constraint-aware interaction**, and environment behavior during training

## Environment Setup

The baseline agents interact with a badminton rally simulation environment that models turn-based decision-making.

Key environment characteristics include:

- **turn-based rally simulation**
- **10 discrete shot types**
- **4 continuous action parameters**
- **serve and scoring logic**
- **out-of-bound and miss-hit checking**
- **constraint-aware action validation**

## Methods

### Baseline Agents
This subproject includes experiments with:

- **PDQN**
- **Hybrid PPO**
- **Hybrid SAC**

### Opponent Model
The environment uses **RallyNet** as a learned opponent for interaction and evaluation.

### Reward Design
The baseline environment includes a simple reward design based on rally outcomes and invalid actions, including:

- positive reward for winning the rally
- penalties for invalid or constrained actions
- penalties for losing due to out-of-bound or miss-hit situations

## Notes

This repository is intended as a **contribution showcase**, not a full release of the original CoachAI+ project. Many other parts of the broader system were developed outside my team’s scope.

The code and experiments highlighted here are centered on the **baseline training branch**, where we explored RL-based decision-making under the CoachAI+ badminton environment.

## Related Project

For the original CoachAI+ project and broader research context, please refer to the upstream CoachAI repositories and related publications.
