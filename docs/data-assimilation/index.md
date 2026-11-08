# Diffusion Models for Data Assimilation

The central problem is to infer an atmospheric state $x$ from imperfect observations $y$, using a model prior and an observation likelihood.

$$p(x\mid y)\propto p(y\mid x)p(x).$$

Generative approaches seek plausible posterior samples rather than only one optimal analysis state.

## Research directions

- Observation-guided reverse diffusion
- Score-based trajectory data assimilation
- Conditional DDPM-based analysis generation
- Sparse and irregular weather-station observations
- Satellite radiances with nonlinear observation operators
- Posterior spread, calibration, reliability and uncertainty
- Comparisons with 3D-Var, 4D-Var, EnKF and hybrid EnVar

## Primary literature

| Paper | Year | Central contribution | Link |
|---|---:|---|---|
| Rozet & Louppe — Score-based Data Assimilation | 2024 | Score-based inference of state trajectories with observation model at inference | [arXiv](https://arxiv.org/abs/2306.10574) |
| Huang et al. — DiffDA: a Diffusion model for weather-scale Data Assimilation | 2024 | Global atmospheric DA with sparse simulated ERA5 observations | [PMLR](https://proceedings.mlr.press/v235/huang24h.html) |
| Generative Data Assimilation of Sparse Weather Station Observations at Kilometer Scales | 2025 | Score-based DA for kilometer-scale atmospheric analysis | [DOI](https://doi.org/10.1029/2024MS004505) |

## Questions for each paper

1. What serves as the prior, and how is it trained?
2. Are observations present during training, sampling, or both?
3. How is the observation error covariance represented?
4. Are the observation operators linear or nonlinear?
5. What validation demonstrates calibrated uncertainty rather than only low RMSE?
6. How does the approach scale to high-resolution NWP?

## Planned subtopics

- **Satellite DA:** radiance assimilation, RTTOV/emulators, cloudy conditions
- **Regional DA:** local domains, boundary conditions and fine-scale observations
- **Ensemble DA:** posterior sampling, spread–skill, CRPS and reliability

> Note: This library reports literature findings; it does not assert that current generative DA methods are operational replacements for established NWP DA systems.
