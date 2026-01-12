# Discounted Scoring Framework (DSF)

A modular point process framework for modeling sports scoring under competing termination risks.

**Paper:** [Link forthcoming]

## Overview

The Discounted Scoring Framework integrates scoring intensity with period and game termination hazards. Unlike traditional models that treat game duration as a fixed boundary, DSF discounts expected scoring by the joint survival probability of period and game continuation. Estimation combines maximum likelihood for scoring with Cox & Breslow methods for termination.

This repository contains code for:
- Simulation studies across eleven sport configurations
- Empirical applications to MLB, NHL, and UFC data
- Parameter estimation, residual diagnostics, and calibration assessment

## Repository Structure
```
├── simulations/       # Monte Carlo simulation configurations
├── mlb/               # MLB pitch-level analysis
├── nhl/               # NHL play-by-play analysis
└── ufc/               # UFC bout-level analysis
```

## Requirements
```
Python 3.10+
numpy
scipy
pandas
numba
matplotlib
```

## Data Sources

- **MLB:** Statcast via Baseball Savant (2005–2024)
- **NHL:** NHL API (2009–2024)
- **UFC:** UFCStats.com (1994–2025)


## Citation
```bibtex
@article{cadley2026dsf,
  title={Scoring Intensity Under Competing Termination Risks: A Modular Point Process Framework},
  author={Karsten Cadley},
  journal={},
  year={2026}
}
```

## License

MIT
