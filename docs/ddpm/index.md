# Denoising Diffusion Probabilistic Models (DDPM)

DDPM defines a finite sequence of corruption steps, then trains a neural network to reverse them.

## Topics

1. Forward Gaussian process and variance schedules
2. Reverse Markov transitions
3. Variational bounds and simplified noise-prediction objectives
4. Sampling algorithms and computational cost
5. DDIM and accelerated sampling

## Papers

| Paper | Year | Relevance | Link |
|---|---:|---|---|
| Ho, Jain & Abbeel — Denoising Diffusion Probabilistic Models | 2020 | Original DDPM formulation | [arXiv](https://arxiv.org/abs/2006.11239) |
| Song, Meng & Ermon — Denoising Diffusion Implicit Models | 2021 | Faster implicit sampling | [arXiv](https://arxiv.org/abs/2010.02502) |
| Nichol & Dhariwal — Improved Denoising Diffusion Probabilistic Models | 2021 | Improved likelihood and sampling | [arXiv](https://arxiv.org/abs/2102.09672) |

## Implementations

- [Original DDPM implementation](https://github.com/hojonathanho/diffusion)
- [Improved Diffusion](https://github.com/openai/improved-diffusion)

## Suggested notes

Describe training objective, noise schedule, U-Net architecture, inference steps, datasets, evaluation metrics and known limitations for each paper.
