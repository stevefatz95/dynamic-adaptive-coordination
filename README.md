# Feedback-Coupled Memory Systems: Dynamical Model for Adaptive Coordination

Computational materials accompanying the paper:

> Grassi, S. (2026). **Feedback-Coupled Memory Systems: Dynamical Model for
> Adaptive Coordination**.

## Overview

This repository introduces the computational verification of **Feedback-Coupled
Memory Systems (FCMS)**, a class of closed-loop dynamical systems in which
agents, incentives, and a persistent environment are recursively coupled.

The framework demonstrates that:

- Agents update their states based on **local incentive signals** with no
  global observation
- The environment accumulates interaction history and feeds it back as
  directional pressure
- A **coordinated collective state emerges dynamically** from the interplay
  of persistence, coupling, and dissipation

Unlike approaches that rely on explicit optimization or centralized control,
the model shows that coordination arises as a **stability property of the
system dynamics**, not as the solution to an optimization problem.

## Repository Contents

| File | Description |
| :--- | :--- |
| `notebooks/figures_fcms.ipynb` | Reproduces Figures 2–5 from the paper: disagreement dynamics, early warning signatures, nonlinear phase portrait, and scalability |
| `notebooks/coordination_dynamics_verification.ipynb` | Structural verification of the theoretical model: stability analysis, ablation studies, bifurcation analysis, robustness simulations, and macroscopic scalability |
| `figures/Figure_1.png` | Recursive FCMS architecture diagram |
| `figures/Figure_2.png` | Disagreement dynamics and Neimark–Sacker boundary |
| `figures/Figure_3.png` | Early warning signatures near bifurcation threshold |
| `figures/Figure_4.png` | Nonlinear phase portrait under tanh saturation |
| `figures/Figure_5.png` | Synchronization variance scaling with population size |
| `requirements.txt` | Python dependencies |

## Repository Structure
```
dynamic-adaptive-coordination/
│
├── README.md
├── requirements.txt
│
├── figures/
│   ├── Figure_1.png
│   ├── Figure_2.png
│   ├── Figure_3.png
│   ├── Figure_4.png
│   └── Figure_5.png
│
└── notebooks/
    ├── figures_fcms.ipynb
    └── coordination_dynamics_verification.ipynb
```

## Installation

### 1. Clone the repository
```bash
git clone https://github.com/stevefatz95/dynamic-adaptive-coordination.git
cd dynamic-adaptive-coordination
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the notebooks
```bash
jupyter notebook notebooks/
```

## Reproducibility

The notebooks provide transparent computational verification of the analytical
results presented in the paper. All code blocks are minimal implementations of
the exact equations derived in the manuscript and Appendix.

`figures_fcms.ipynb` reproduces:
- Disagreement dynamics and critical slowing down (Figure 2)
- Early warning signatures: variance and autocorrelation (Figure 3)
- Nonlinear phase portrait under tanh saturation (Figure 4)
- Synchronization variance scaling with population size N (Figure 5)

`coordination_dynamics_verification.ipynb` verifies:
- Baseline stability via Jacobian eigenvalues
- Structural necessity through ablation of coupling, persistence, and dissipation
- Exact stability boundary and Neimark–Sacker bifurcation surface
- Noise robustness and parameter heterogeneity
- Nonlinear robustness under tanh saturation
- Macroscopic scalability to N = 10^6 agents

The objective is structural validation of the theoretical model, not
performance optimization.

## Parameters

Core parameters used throughout (matching the main text):

| Parameter | Value | Meaning |
| :--- | :--- | :--- |
| `gamma` | 1.0 | Memory dissipation rate |
| `eta` | 0.1 | Agent responsiveness |
| `beta_c` | ≈ 1.581 | Critical coupling threshold |

## Citing This Work
```bibtex
@article{grassi2026fcms,
  title={Feedback-Coupled Memory Systems: Dynamical Model for Adaptive Coordination},
  author={Grassi, Stefano},
  year={2026}
}
```

## Preprint

The full manuscript is available at:
[https://arxiv.org/abs/2603.11560](https://arxiv.org/abs/2603.11560)

## License

This project is released under the MIT License.
