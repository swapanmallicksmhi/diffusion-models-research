# Score-Based Diffusion Models

This track focuses on learning the score of noise-perturbed distributions and integrating reverse-time dynamics.

## Topics

- Score matching and denoising score matching
- Annealed Langevin dynamics
- Variance-exploding (VE) SDE and variance-preserving (VP) SDE
- Reverse-time SDE and probability-flow ODE
- Predictor–corrector sampling and numerical solvers

## Key formulation

For forward dynamics $dx=f(x,t)dt+g(t)dW$, the associated reverse-time SDE uses the learned score, with the time direction reversed:

$$dx=[f(x,t)-g(t)^2\nabla_x\log p_t(x)]dt+g(t)d\bar W.$$

The meaning of $dt$ and the reverse Wiener process must be interpreted in reverse time.

## Papers and code

| Paper | Year | Link |
|---|---:|---|
| Song & Ermon — Generative Modeling by Estimating Gradients of the Data Distribution | 2019 | [arXiv](https://arxiv.org/abs/1907.05600) |
| Song et al. — Score-Based Generative Modeling through SDEs | 2021 | [arXiv](https://arxiv.org/abs/2011.13456) |

Official example: [score_sde_pytorch](https://github.com/yang-song/score_sde_pytorch).

## Comparison with DDPM

DDPM and score-based diffusion are **closely related formulations**, not necessarily mutually exclusive model classes. The SDE framework can unify several discrete- and continuous-time approaches.
