# Population Dynamics Simulator

![Python](https://img.shields.io/badge/python-3.7+-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

Interactive Python application for visualizing mathematical population growth models.

## Overview

A desktop GUI tool to explore and compare different population dynamics models used in ecology and mathematical biology:

- **Malthus Model** - Exponential growth
- **Verhulst Logistic (Discrete)** - Chaotic dynamics
- **Verhulst Logistic (Continuous)** - Growth with carrying capacity
- **Hutchinson Model** - Delayed logistic growth

## Quick Start

### Install dependencies:
```bash
pip install numpy matplotlib ddeint
```

### Run the app:
```bash
python src/main.py
```

## Usage

1. Select a model from the dropdown
2. Adjust parameters (population, growth rate, etc.)
3. Set simulation time
4. Visualize the results

## Project Structure

```
src/
├── main.py                  # Entry point
├── models/
│   └── population_models.py # Model implementations
└── views/
    └── main_window.py       # GUI (Tkinter)
```

## Models

| Model | Equation | Key Feature |
|-------|----------|-------------|
| Malthus | P(t) = P₀e^(rt) | Unlimited exponential growth |
| Discrete Logistic | Pₙ₊₁ = rPₙ(1-Pₙ) | Can show chaos |
| Continuous Logistic | P(t) = K/(1+Ae^(-rt)) | S-curve to capacity |
| Hutchinson | dP/dt = rP(t)(1-P(t-τ)/K) | Time-lag effects |

## Use Cases

- Learning population ecology
- Studying dynamical systems
- Exploring chaos theory
- Teaching mathematical modeling

## License

MIT License - see [LICENSE](LICENSE)
