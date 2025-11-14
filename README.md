# Probabilistic Generative Models

**Imperial College London – Department of Mathematics**  
**MSc in Applied Mathematics**  
**Dates: Spring Term 2025 / 2026**  
**Format: 10 weeks, 3 hours per week (roughly 2h lecture + 1h demonstration)**  
**Staff: Felipe Tobar (Lecturer), Camilo Carvajal Reyes, Skye Purchase**

---

## Introduction

This module provides a modern introduction to *probabilistic generative modelling*, from foundational conceptual principles including graphical models, variational inference and Bayesian nonparametric models, to recent developments such as Transformers, diffusion models and flow matching. The module aims to give students a unified understanding of generative modelling as the *transportation of probability distributions*. The course blends mathematical content, algorithm development, and hands-on demonstrations.

---

# Weekly Plan

## **Week 1 — Foundations of Generative Modelling & Nonparametric Models**

### Content
- Latent variable models, sampling vs likelihood  
- Explicit models: mixtures, factor analysers  
- Bayesian inference, KL divergence, ELBO intuition  
- Bayesian nonparametrics:  
  - Gaussian Processes (as generative priors)  
  - Dirichlet Processes (CRP, stick-breaking)  
- Motivation for geometric/OT viewpoints

### Literature
- MacKay — *Information Theory, Inference, and Learning Algorithms*  
- Bishop — *Pattern Recognition and Machine Learning*  
- Rasmussen & Williams — *Gaussian Processes for Machine Learning* (online)  
- Blei — *Dirichlet Process Mixtures*: https://arxiv.org/abs/1601.00670  

---

## **Week 2 — An Introduction to Optimal Transport**

### Content
- The transportation problem
- Monge and Kantorovich
- Computation of OT: Exact and Sinkhorn
- Metric properties, Wasserstein distances and couplings  
- Dynamic OT (Benamou–Brenier)  
- Geodesics & probability paths  
- OT as a lens for generative models:  
  - Flows as transport maps  
  - Diffusion as stochastic transport  

### Literature
- Peyré & Cuturi — *Computational Optimal Transport*: https://optimaltransport.github.io/  
- Villani — *Topics in Optimal Transportation*  
- Santambrogio — *Optimal Transport for Applied Mathematicians*  
- Cuturi — *Sinkhorn Distances*: https://arxiv.org/abs/1306.0895  

---

## **Week 3 — Graphical Models, EM, Classical Inference**

### Content
- Directed & undirected graphical models  
- EM algorithm (derivation)  
- Exact inference & message passing  
- Approximate inference: mean-field, Gibbs, BP  
- Bridge to modern VI

### Literature
- Koller & Friedman — *Probabilistic Graphical Models*  
- Bishop — PRML  
- Dempster et al. — *EM Algorithm*  

---

## **Week 4 — Variational Inference: From Classical to Amortised VI**

### Content
- ELBO derivation  
- Variational families & structured VI  
- Coordinate-ascent & stochastic VI  
- Amortised inference and neural variational methods

### Literature
- Blei et al. — *Variational Inference: A Review*: https://arxiv.org/abs/1601.00670
- Jordan et al. — *Variational Methods for Graphical Models*  
- Hoffman et al. — *Stochastic Variational Inference*: https://arxiv.org/abs/1206.7051  

---

## **Week 5 — Deep Latent Variable Models: VAEs & GANs**

### Content
- Deep latent generative models  
- Encoder–decoder architecture  
- Reparameterisation trick  
- β-VAE, disentanglement  
- GANs: adversarial training, divergences, stability  
- VAEs vs GANs from geometric & OT perspectives

### Literature
- Kingma & Welling — *Auto-Encoding Variational Bayes*: https://arxiv.org/abs/1312.6114  
- Goodfellow et al. — *Generative Adversarial Nets*: https://arxiv.org/abs/1406.2661  
- Arjovsky et al. — *Wasserstein GAN*: https://arxiv.org/abs/1701.07875  
- Higgins et al. — *β-VAE*: https://openreview.net/forum?id=Sy2fzU9gl  

---

## **Week 6 — Autoregressive Models & Transformers**

### Content
- Early Autoregressive models  
- Sequential generative modelling  
- Attention: inner products in the feature space
- Transformers as large-scale likelihood models  
- Sampling strategies (top-k, top-p, temperature)  
- Comparison with latent models and flow models

### Literature
- Vaswani et al. — *Attention is All You Need*: https://arxiv.org/abs/1706.03762  
- Radford et al. — *Language Models are Unsupervised Multitask Learners*  

---

## **Week 7 — Normalizing Flows**

### Content
- Change-of-variables formula  
- Designing invertible networks  
- Warped GPs  
- Flows as transport maps  
- Strengths, limitations, and geometry

### Literature
- Rezende & Mohamed — *Normalizing Flows*: https://arxiv.org/abs/1505.05770  
- Papamakarios et al. — *Normalizing Flows Tutorial*: https://arxiv.org/abs/1912.02762  
- Dinh et al. — *RealNVP*: https://arxiv.org/abs/1605.08803  
- Rios & Tobar - *Compositionally warped GPs*

---

## **Week 8 — Flow Matching & Continuous Generative Flows**

### Content
- Continuous-time generative models  
- Neural ODEs & continuity equations  
- Flow matching: vector-field supervision  
- No Jacobians or invertibility constraints  
- Deterministic vs stochastic generative flows  
- Connection to OT and diffusion

### Literature
- Lipman et al. — *Flow Matching for Generative Modelling*: https://arxiv.org/abs/2210.02747  
- Chen et al. — *Neural ODEs*: https://arxiv.org/abs/1806.07366  
- Albergo & Vanden-Eijnden — *Stochastic Dynamics & Flows*  

---

## **Week 9 — Score-Based Models & Diffusion: Theory**

### Content
- Score matching  
- Denoising score matching  
- Score-based generative modelling as reverse SDEs  
- Discrete–continuous diffusion connections  
- Links to energy-based models and flows

### Literature
- Hyvärinen — *Score Matching*: https://jmlr.org/papers/v6/hyvarinen05a.html  
- Song & Ermon — *Score-Based Generative Modelling via SDEs*: https://arxiv.org/abs/2011.13456  
- Vincent — *Denoising Score Matching*  

---

## **Week 10 — Practical Diffusion Models: DDPM, DDIM, Guidance, OT Unification**

### Content
- DDPM training objective  
- Noise schedules, ancestral sampling  
- DDIM: deterministic sampling  
- Classifier-free guidance  
- Efficiency & likelihood estimation  
- Unifying flows, flow matching, and diffusion via OT

### Literature
- Ho et al. — *DDPM*: https://arxiv.org/abs/2006.11239  
- Song et al. — *DDIM*: https://arxiv.org/abs/2010.02502  
- Dhariwal & Nichol — *Diffusion Models Beat GANs*: https://arxiv.org/abs/2105.05233  
- Albergo et al. — *Stochastic Interpolants*: https://arxiv.org/abs/2303.08797  

---





