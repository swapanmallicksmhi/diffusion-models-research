# 🌌 Diffusion Models — Theory, Literature & Data Assimilation

[![Documentation](https://img.shields.io/badge/Documentation-Zensical-6750A4)](https://zensical.org/) ![Literature](https://img.shields.io/badge/Focus-DDPM%20%7C%20Score--SDE%20%7C%20DA-157a8c) ![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen)

A curated, research-focused knowledge base on diffusion generative models, with an emphasis on **DDPM**, **score-based diffusion**, and **data assimilation for weather and climate**.

> 🧭 **Explore:** [Foundations](docs/foundations/index.md) · [DDPM](docs/ddpm/index.md) · [Score-based diffusion](docs/score-based/index.md) · [Diffusion Data Assimilation](docs/data-assimilation/index.md) · [Reading roadmap](docs/reading-lists/index.md)

## Research tracks

| Track | Main topics | Literature |
|---|---|---|
| Foundations | Stochastic processes, diffusion, Bayesian inference | [Explore](docs/foundations/index.md) |
| DDPM | Forward/reverse processes, ELBO, noise prediction, DDIM | [Explore](docs/ddpm/index.md) |
| Score-based | Score matching, Langevin, VP/VE SDE, probability flow ODE | [Explore](docs/score-based/index.md) |
| Data assimilation | Posterior sampling, observation constraints, weather DA | [Explore](docs/data-assimilation/index.md) |

## Quick start

Requires Python 3.11+ and Git.

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
zensical serve
```

Open <http://127.0.0.1:8000>. To build: `zensical build`.

## Publish on GitHub Pages

1. Create a public GitHub repository named `diffusion-models-research`.
2. Push this repository to branch `main`.
3. In **Settings → Pages → Build and deployment**, select **GitHub Actions**.
4. The included `.github/workflows/docs.yml` builds and publishes your site on pushes to `main`.
5. Your URL will typically be `https://YOUR_USERNAME.github.io/diffusion-models-research/`.

No GitHub repository has been created or published by this archive itself.

## Add literature

Copy `templates/paper-note.md` to the relevant `docs/` track, add a short critical summary, add a citation to `references/references.bib`, and update the track's index. Prefer authoritative DOI/arXiv links; do not commit copyrighted PDFs without redistribution permission.

## Organization

```text
docs/                 # Website pages and curated literature
  foundations/
  ddpm/
  score-based/
  data-assimilation/
  applications/
  reading-lists/
references/           # BibTeX references
templates/            # Structured paper review template
.github/workflows/    # Automatic GitHub Pages publishing
zensical.toml         # Website configuration
```

## Scope and quality

Each entry should distinguish **published findings** from our **interpretation**, name the experimental setting, and explicitly note limitations. The starting bibliography is selective, not exhaustive, and should be reviewed regularly.

## License

MIT for original repository code and notes (see `LICENSE`); third-party articles remain under their respective licenses.
