---
title: We ~~are recruiting~~ have recruited a research engineer!
date: 2025-09-10
---

We propose a **one-year research engineer** contract to work at LIG and Inria Grenoble. Starting date is before the end of 2025, with some flexibility. The position is funded by the MIAI chair "Simulation-Based Inference for Climate" (SBI4C) and is renewable once (for a total of two years).

<!--more-->

---

**Important**: Applications are open until 02-November, 2025. Please apply through the [official UGA job posting](https://emploi.univ-grenoble-alpes.fr/offres/ingenieur-de-recherche-en-inference-basee-sur-des-simulations-pour-le-climat-f-h--1657489.kjsp?RH=1135797159702996)

**Context.** The research engineer position we are offering is part of the SBI4C chair of the MIAI cluster at the Grenoble Institute of Artificial Intelligence. This project aims to develop machine learning methods to better understand and model physical phenomena, particularly in climate sciences and the associated inverse problems. The objective is to extend simulation-based Bayesian inference (SBI) to large-scale climate models by designing new algorithms that take the computational cost of simulations into account and by developing efficient emulators. The reference tool for implementing SBI techniques in practice is the [`sbi`](https://sbi-dev.github.io/sbi) package, which gathers the main advances in the field. However, deploying these procedures on advanced simulations—beyond classical academic test cases—requires more robust software infrastructure, capable of leveraging supercomputing power and adopting methodologies suited for the scale of such advanced simulations. The candidate will work mainly with [Pedro Rodrigues](plcrodrigues.github.io) (LJK/Inria) and [Bruno Raffin](https://datamove.imag.fr/bruno.raffin/) (LIG/Inria).

---

**Assigned mission:** Develop a proof of concept applying SBI to large-scale numerical simulation codes in climate science.

---

**Activities:** This proof of concept will be built upon three main components:

- The [`tunax`](https://github.com/meom-group/tunax) code, which we are developing and which includes a vertical ocean physics code written in `jax` along with minimization methods to calibrate parameters.

- The [`sbi`](https://sbi-dev.github.io/sbi) software suite, to which we contribute and which, as mentioned above, encapsulates state-of-the-art SBI methods, but in a Python package not designed for large-scale deployment.

- The [`melissa`](https://gitlab.inria.fr/melissa/melissa) software , designed for training neural networks on supercomputers directly from data produced by numerical simulations.

Note that `tunax` will provide the simulator, `melissa` the orchestrator to coordinate the execution of simulations and online learning, and `sbi` the neural models and incremental parameterization strategy for selecting the next simulator instances to be executed.

The candidate will also contribute to:

- Setting up a suite of intermediate-complexity test cases (benchmark) to compare climate model calibration methods, which will eventually be made available to the community.
- Organizing the SBI hackathon planned in Grenoble in early 2026: creating the event website, structuring the proposed projects, and coordinating objectives with the main contributors to the sbi package.

---

**Required skills**: The ideal candidate will have training in numerical simulation or applied mathematics with a specialization in statistical learning, as well as knowledge of high-performance computing, at the Master’s (M2) or engineering school level. The candidate must demonstrate:

- Strong programming skills, particularly in Python; experience with cluster computing would be an asset.

- Ability to work as part of a team and to comply with established rules and procedures.

- A capacity to learn and develop skills, along with an interest in sharing knowledge (blog posts, articles, open-source contributions).

- An interest in pursuing a PhD within the SBI4C chair after the engineering position would be an additional asset for the application.