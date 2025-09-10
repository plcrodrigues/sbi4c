---
title: About the project
date: 2025-09-10
type: pages

---

**Context and objectives**. The machine learning community has demonstrated increasing interest in
addressing open challenges across a range of scientific disciplines, such as biology,
astrophysics, and fluid dynamics. Our project, SBI4C, falls within this vibrant AI4Science landscape and
addresses a <u>fundamental challenge in experimental science: the problem of parameter inference</u>. Specifically, we aim
to determine the parameter values of a physical model that best reproduce observed
data.
![parameter inference](parameterinference.png "**Figure 1**: Given a stochastic simulator 
taking parameters $\theta$ as input and returning simulations $x \sim p(x|\theta)$, the posterior distribution $p(\theta|x_0)$ helps us determine the parameters which are the most likely to have generated observation $x_0$. Figure taken from [[Deistler et al. 2025](https://arxiv.org/abs/2508.12939)]")

**Tools**. To achieve this, we employ simulation-based inference (SBI) [[Cranmer et al. 2020](https://arxiv.org/abs/1911.01429), [Deistler et al. 2025](https://arxiv.org/abs/2508.12939)]—a suite of
methods rooted in Bayesian statistics that leverage advancements in deep generative models to
approximate posterior distributions over a simulator's full set of parameters, i.e. a probability
density function attaining larger values in regions of the parameter space that are more likely to
have generated the observed experimental data.
![sbi](sbi.png "**Figure 2**: SBI consist of four main steps: (i) draw parameters from the prior distribution $\theta_i \sim p(\theta)$, and (ii) run the simulator to generate data $x_i \sim p(x|\theta_i)$. (iii) Train over dataset $(\theta_i, x_i)$ a conditional generative model $q_\phi$ that takes $x$ as input and predicts a distribution over parameters $\theta$. (iv) 
Use $q_\phi(\theta|x_0)$ as an approximation to the posterior $p(\theta|x_0)$. Figure taken from [[Deistler et al. 2025](https://arxiv.org/abs/2508.12939)]")

**Challenges**. Despite recent successes of the SBI framework across various applied domains, its applicability
is currently constrained to relatively small-scale models. The primary methodological goal of
SBI4C is to extend the capabilities of SBI to accommodate simulators that rely on solving
large systems of partial differential equations (PDEs) to generate observations. A
quintessential example of such a simulator is a climate model, which encapsulates complex
interactions in the ocean and atmosphere to study climate physics. 
![sbi](climatesimulations.png "**Figure 3**: Blabla. Figure taken from [[Deistler et al. 2025](https://arxiv.org/abs/2508.12939)]")

**Climate models**. In this project, we will focus on such models, both as a target application and as a source of inspiration for identifying new research directions. Notably, the problem of parameter tuning has a well-established presence
in climate science literature and has garnered significant attention in recent years. However, to
date, no initiative has fully leveraged the flexibility and power of modern simulation-based
inference techniques for this purpose.

**Directions**. The SBI4C project is structured around three main axes of research:
- Sada
- SDA
- SFSAFA

**Impact**. By advancing the robustness and reproducibility of parameter inference methods in climate
science, the SBI4C project aims to make substantial contributions to the practices of
climatologists while enhancing the reliability of model-based projections for policymakers.
Moreover, the novel SBI methods we develop will be readily applicable to other domains
involving large-scale simulators, such as cosmology, computational neuroscience, and
civil engineering.