# Dynamic Adaptive Coordination

Computational materials accompanying the paper **“How Intelligence Emerges: A Minimal Theory of Dynamic Adaptive Coordination”.**

## Overview

This work introduces a **minimal dynamical systems model** describing how coordination can emerge among interacting adaptive agents through a feedback-mediated environment.

The framework shows that:

* Agents adapt their actions based on **local incentive signals**
* The environment aggregates and feeds back the consequences of these actions
* A **coordinated collective state emerges dynamically** through the interaction of persistence, coupling, and dissipation

Unlike many multi-agent approaches that rely on explicit optimization or centralized coordination, the model demonstrates that **intelligent collective behavior can arise as a property of the system dynamics itself**.

# Current Contents

This repository currently includes:

* `notebooks/minimal_linear_system.ipynb` – A minimal implementation of the coordination dynamics described in the paper, illustrating the basic mechanism through a simple linear feedback system.

* `notebooks/coordination_dynamics_verification.ipynb` – A computational notebook providing structural verification of the theoretical model, including stability analysis, structural experiments, and robustness simulations.

* `requirements.txt` – Python dependencies required to run the notebooks.

The notebooks reproduce key properties of the theoretical framework, including:

* emergent coordination dynamics
* stability conditions
* bifurcation boundaries
* structural necessity experiments
* robustness to stochastic perturbations

## Repository Structure

```
dynamic-adaptive-coordination/
│
├── README.md
├── requirements.txt
│
└── notebooks/
    ├── minimal_linear_system.ipynb
    └── coordination_dynamics_verification.ipynb
```

## Installation

### 1. Clone the repository

`git clone https://github.com/stevefatz95/dynamic-adaptive-coordination.git
cd dynamic-adaptive-coordination`

### 2. Install dependencies

`pip install -r requirements.txt`

### 3. Run the notebooks

`jupyter notebook notebooks/`

## Reproducibility

The notebooks provide **transparent computational verification** of the analytical results presented in the paper.

The implementations focus on:

* minimal linear coordination dynamics
* stability verification via Jacobian eigenvalues
* parameter regime exploration
* stochastic robustness analysis

The objective is **structural validation of the theoretical model**, not performance optimization.

## Citing This Work

If you find this work or the code implementation useful for your research or your work, please cite the corresponding paper using the following BibTeX entry (or the format specified by your target venue):

```bibtex
@article{grassi2026coordination,
  title={How Intelligence Emerges: A Minimal Theory of Dynamic Adaptive Coordination},
  author={Grassi, Stefano},
  year={2026}
}
```

## Paper

The full manuscript describing the theoretical framework can be found here:

(Add link once uploaded — e.g. arXiv / SSRN)

## License

This project is released under the MIT License.

