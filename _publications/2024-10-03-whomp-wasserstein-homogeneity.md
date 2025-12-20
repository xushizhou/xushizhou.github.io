---
title: "WHOMP: Improving Upon Randomized Controlled Trials via Wasserstein Homogeneity"
collection: publications
category: manuscripts
permalink: /publication/2024-10-03-whomp-wasserstein-homogeneity/
excerpt: "We introduce WHOMP, a Wasserstein-homogeneity optimality principle for subgroup splitting in comparative experiments (clinical trials, social experiments, and A/B tests). The method yields interpretable criteria, efficient estimators, and strong empirical gains over random partitioning, covariate-adaptive randomization, rerandomization, and anti-clustering baselines."
date: 2024-10-03
venue: "Under review (Journal of the American Statistical Association)"
paperurl: "https://arxiv.org/pdf/2409.18504"
codeurl: ""
slidesurl: ""
citation: 'Shizhou Xu, Thomas Strohmer. (2024). “WHOMP: Improving Upon Randomized Controlled Trials via Wasserstein Homogeneity.” <i>Under review at Journal of the American Statistical Association</i>.'
---

### Summary
Comparative experiments often require *splitting a population into subgroups* (e.g., stratification, cohort construction, or controlled partitioning) while minimizing accidental bias and maximizing statistical efficiency.  
This paper proposes **WHOMP**, a principled criterion built on **Wasserstein homogeneity**, and provides **efficient algorithms** to compute near-optimal subgroup splits at scale.

### Key contributions
- **Optimality criterion:** A Wasserstein-based homogeneity objective that directly targets subgroup balance in a distributional sense.
- **Algorithms:** Practical estimators and solvers designed to be used in real experimental pipelines.
- **Theory + analysis:** Analytical comparisons clarifying when and why WHOMP improves upon classical baselines.
- **Empirical validation:** Numerical experiments demonstrating consistent gains across multiple realistic settings.

### Resources
- Paper (PDF): https://arxiv.org/pdf/2409.18504
- Code: *(add link when public)*
- Slides: *(add link if available)*

### Suggested BibTeX
```bibtex
@misc{xu2024whomp,
  title        = {WHOMP: Improving Upon Randomized Controlled Trials via Wasserstein Homogeneity},
  author       = {Xu, Shizhou and Strohmer, Thomas},
  year         = {2024},
  note         = {Under review at Journal of the American Statistical Association},
  howpublished = {arXiv preprint},
}
