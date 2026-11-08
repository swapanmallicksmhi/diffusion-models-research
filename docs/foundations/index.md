# Foundations

## Mathematical foundations

Study probability distributions, Gaussian corruption, Markov chains, score functions and stochastic differential equations before comparing model families.

A common forward perturbation in DDPM is:

$$q(x_t\mid x_0)=\mathcal{N}(\sqrt{\bar\alpha_t}x_0,(1-\bar\alpha_t)I).$$

A central object in score-based modeling is the score:

$$s(x,t)=\nabla_x\log p_t(x).$$

## Foundational reading

- **Ho, Jain & Abbeel (2020)** — [Denoising Diffusion Probabilistic Models](https://arxiv.org/abs/2006.11239)
- **Song et al. (2021)** — [Score-Based Generative Modeling through Stochastic Differential Equations](https://arxiv.org/abs/2011.13456)

## Key question

How do discrete-time noise-prediction objectives correspond to learning the score of progressively perturbed data distributions?
