---
title: "Research"
permalink: /research/
author_profile: yes
output:
  html_document:
    df_print: paged
---

Bayesian modeling plays a central role in many scientific disciplines and branches of machine learning, where it is of interest to quantify uncertainty. A persistent bottleneck in Bayesian analysis is the computation of the posterior distribution. This problem is exacerbated by the increasing complexity of models and the growing size of data. To address this challenge, my research program centers on developing algorithms for Bayesian inference, which can take advantage of modern computation.

A selection of research papers is available on my [home page](https://charlesm93.github.io/).
Here, I provided a more exhaustive list which includes conference posters and other technical reports.
I ordered these into four broad themes: 

* Markov chain Monte Carlo
* Variational inference
* Bayesian workflow and scientific applications
* Automatic differentiation


# Markov chain Monte Carlo

MCMC is the workhorse of Bayesian inference.
In recent years, it has become possible to efficiently parallelize MCMC by running hundreds, even thousands, of Markov chains on hardware accelerators such as GPUs. My work investigates shifts in the practice and analysis of MCMC as we transition from CPU- to GPU-based hardware.

Papers:

* (2024) <span style="color:maroon">Nested $\widehat R$: Assessing the convergence of Markov chain Monte Carlo when running many short chains.</span> C. Margossian, M. Hoffman, P. Sountsov, L. Riou-Durand, A. Vehtari and A. Gelman. _Bayesian Analysis_ [[preprint](https://arxiv.org/abs/2110.13017), [code](https://github.com/charlesm93/nested-rhat)]
* (2024) <span style="color:maroon">Listening to the Noise: Blind Denoising with Gibbs Diffusion.</span> D. Heurtel-Depeiges, C. Margossian, R. Ohana and B. Regaldo-Saint Blancard. _PMLR: International Conference on Machine Learning_ [[preprint](https://arxiv.org/pdf/2402.19455.pdf)]
* (2024) <span style="color:maroon">For how many iterations should we run Markov chain Monte Carlo?</span> C. Margossian and A. Gelman. _Handbook of Markov chain Monte Carlo_, (upcoming) 2nd Edition. [[preprint](https://arxiv.org/abs/2311.02726)]
* (2022) <span style="color:maroon">Adaptive Tuning for Metropolis Adjusted Langevin Trajectories.</span> L. Riou-Durand, P. Sountsov, J. Vogrinc, C. Margossian and S. Power. _PMLR: Artificial Intelligence and Statistics_ [[paper](https://proceedings.mlr.press/v206/riou-durand23a/riou-durand23a.pdf), [preprint](https://arxiv.org/abs/2210.12200), [code](https://github.com/tensorflow/probability/tree/main/discussion/adaptive_malt)]


Posters and technical reports:

* (2024) <span style="color:maroon">Monitoring Nonstationary Variance to Assess Convergence of MCMC.</span> E. Mokel and C. Margossian. *International Society of Bayesian Analysis (ISBA) world meeting*. Best poster award.
* (2023) <span style="color:maroon">Parallelization for Markov chains with heterogeneous runtimes.</span> S. du Ché and C. Margossian. _BayesComp_. [[poster](http://charlesm93.github.io/files/Bayescomp_ode_chains.pdf)]


# Variational Inference

VI is another workhorse of Bayesian analysis. The _modus operandi_ of VI is to find a parametric approximation of the posterior by solving an optimization problem. We can obtain fast optimization by restricting the family of approximations, for instance by using factorized and/or amortized distributions. VI is then suitable for the constrained computational budget imposed by large problems. On the other hand, a restricted approximation cannot perfectly match the posterior. A major axis of my research studies whether an imperfect approximation can still capture key features of the posterior, such as its mean, variance or entropy, even if this approximation is misleading in other ways. Concurently, I am interested in developing VI with highly expressive families of approximations, and building tractable optimization problems for such families.

Papers:

* (2024) <span style="color:maroon">Variational Inference for Uncertainty Quantification: an Analysis of Trade-Offs.</span> C. Margossian, L. Pillaud-Vivien and L. Saul. [[preprint](https://arxiv.org/abs/2403.13748), [Code](https://github.com/charlesm93/VI-ordering)]
* (2024) <span style="color:maroon">EigenVI: score-based variational inference with orthogonal function expansions.</span> D. Cai, C. Modi, C. Margossian, R. Gower, D. Blei and L. Saul. _Advances in Neural Information Processing Sysmtes_ (spotlight)
* (2024) <span style="color:maroon">Batch and match: black-box variational inference with a score-based divergence.</span> D. Cai, C. Modi, L. Pillaud-Vivien, C. Margossian, R. Gower, D. Blei and L. Saul. _PMLR: International Conference on Machine Learning_ (spotlight) [[preprint](https://arxiv.org/abs/2402.14758)]
* (2024) <span style="color:maroon">Amortized Variational Inference: when and why?</span> C. Margossian and D. Blei. _PMLR: Uncertainty in Artificial Intelligence_ [[preprint](https://arxiv.org/abs/2307.11018), [code](https://github.com/charlesm93/AVI-when-and-why), [talk](https://www.youtube.com/watch?v=vluu7BxA6js)]
* (2023) <span style="color:maroon">Variational Inference with Gaussian Score Matching.</span> C. Modi, C. Margossian, Y. Yao, R. Gower, D. Blei and L. Saul. _Advances in Neural Information Processing Systems_ [[preprint](https://arxiv.org/abs/2307.07849), [code](https://github.com/modichirag/GSM-VI)]
* (2023) <span style="color:maroon">The Shrinkage-Delinkage Trade-off: An Analysis of Factorized Gaussian Approximations for Variational Inference.</span> C. Margossian and L. Saul. _PMLR: Uncertainty in Artificial Intelligence_ (Oral) [[paper](https://proceedings.mlr.press/v216/margossian23a/margossian23a.pdf), [preprint](https://arxiv.org/abs/2302.09163), [code](https://github.com/charlesm93/variance-delinkage), [talk](https://www.youtube.com/watch?v=2q5azatd-Ko)]

# Bayesian workflow and scientific applications

Much of my work is motivated by Bayesian modeling problems in pharmacometrics, epidemiology, and (astro)physics.
A defining characteristic of these models is that they integrate a scientific (forward) model, often based on a system of differential equations, inside a statistical model.

Papers:

* (2022) <span style="color:maroon">Flexible and efficient Bayesian pharmacometrics modeling using Stan and Torsten, Part I.</span> C. Margossian, Y. Zhang and  W. Gillespie. _CPT: Pharmacometrics & Systems Pharmacology_. [[article](https://ascpt.onlinelibrary.wiley.com/doi/10.1002/psp4.12812), [preprint](https://arxiv.org/abs/2109.10184), [code](https://github.com/metrumresearchgroup/torsten_tutorial_1_supplementary), [software](https://metrumresearchgroup.github.io/Torsten/)]
* (2021) <span style="color:maroon">Bayesian Workflow for disease transmission modeling in Stan.</span> L. Grinsztajn, E. Semenova, C. Margossian and J. Riou. _Statistics in medicine_.
[[article](https://onlinelibrary.wiley.com/doi/10.1002/sim.9164), [preprint](https://arxiv.org/abs/2006.02985),
[code](https://github.com/stan-dev/example-models/tree/master/knitr/disease_transmission),
[talk](https://www.youtube.com/watch?v=unHZhfur5Sc)]
* (2021) <span style="color:maroon">Simulating Ising and Potts models at critical and cold temperatures using auxiliary Gaussian variables.</span> C. Margossian and S. Mukherjee. [[preprint](https://arxiv.org/abs/2110.10801)]
* (2020) <span style="color:maroon">Estimation of SARS-CoV-2 mortality during the early stages of an epidemic: a modelling study in Hubei, China and six regions of Europe.</span> J. Riou et al. _PLOS Medicine_. [[article](https://journals.plos.org/plosmedicine/article?id=10.1371/journal.pmed.1003189),
[preprint](https://www.medrxiv.org/content/10.1101/2020.03.04.20031104v2)]
* (2020) <span style="color:maroon">Bayesian Workflow.</span> A. Gelman et al. [[preprint](https://arxiv.org/abs/2011.01808)]
* (2014) <span style="color:maroon">Planet Hunters. VII. Discovery of a new low-mass, low-density (PH3 C) orbiting Kepler-289
with mass measurements of two additional plamets of two additional planets (PH3 B and D).</span> J. Schmitt et al. _Astrophysical Journal_. [[article](http://iopscience.iop.org/article/10.1088/0004-637X/795/2/167/meta;jsessionid=43641D4C5B1CC7595015BE11DDF1239F.c1)]

Posters and technical reports:

* (2021) <span style="color:maroon">Developping a model of SARS-CoV-2 viral dynamics under monoclonal antibody treatment.</span> A. Marc, M. Kerioui, C. Margossian, J. Bertrand, P. Maisonnasse, Y. Aldon, R. Sanders, M. Van Gils, R. Le Grand and J. Guedj. _Population Approach Group in Europe_.
* (2021) <span style="color:maroon">Solving ODEs in a Bayesian context: challenges and opportunities.</span> C. Margossian, L. Zhang, S. Weber and A. Gelman. _Population Approach Group in Europe_. [[poster](http://charlesm93.github.io/files/BayesianODE.pdf)]
* (2020) <span style="color:maroon">Bayesian model of planetary motion: exploring ideas for a modeling workflow when dealing with ordinary differential equations and multimodality.</span> C. Margossian and A. Gelman. _Stan Case Studies 7_. [[article](https://mc-stan.org/users/documentation/case-studies/planetary_motion/planetary_motion.html), [code](https://github.com/stan-dev/example-models/tree/master/knitr/planetary_motion)]
* (2018) <span style="color:maroon">Computing Steady states with Stan's nonlinear algebraic solver.</span> C. Margossian. _Stan Con Asilomar 2018_. [[article](http://charlesm93.github.io/files/2018-Margossian.pdf), [code](https://github.com/stan-dev/stancon_talks/tree/master/2018/Contributed-Talks/08_margossian), [talk](https://www.youtube.com/watch?v=JhwZIX5ryw0&feature=youtu.be)]
* (2017) <span style="color:maroon">Gaining Efficiency by combining analytical and numerical methods to solve ODEs: implementation in Stan and application to Bayesian PK/PD modeling.</span> C. Margossian and W. Gillespie. _Journal of Pharmacokinetics and Pharmacodynamics, presented at the American Conference on Pharmacometrics 8_. [[poster](http://charlesm93.github.io/files/2017b-Margossian&Gillespie-mixed_solver.pdf)]
* (2017) <span style="color:maroon">Differential equation based models in Stan.</span> C. Margossian and W. Gillespie. _Stan Con 2017_. [[article](http://mc-stan.org/events/stancon2017-notebooks/stancon2017-margossian-gillespie-ode.html), [code](https://github.com/stan-dev/stancon_talks/tree/master/2017/Contributed-Talks/05_margossian), [talk](https://www.youtube.com/watch?v=DJ0c7Bm5Djk&feature=youtu.be&t=2h53m26s)]
* (2016) <span style="color:maroon">Stan functions for pharmacometrics.</span> C. Margossian and W. Gillespie. _Journal of Pharmacokinetics and Pharmacodynamics, presented at the American Conference on Pharmacometrics 7_. [[poster](http://charlesm93.github.io/files/2016-Margossian&Gillespie-stan_for_pmx.pdf)]

# Automatic differentiation

Fitting models in high dimension, whether it be through sampling or optimization, requires gradient-based algorithms. Automatic differentiation (AD) provides a seamless and scalable manner to compute gradients (and higher-order derivatives). Reverse-mode AD has played a defining role over the last decade, enabling much of the progress in deep learning, AI, and probabilistic programming. Many popular software, including Stan, JAX, and PyTorch, are all AD libraries at heart.

I have contributed extensively to Stan's AD library in C++, in particular the propagation of derivatives through implicit functions.
These implicit functions arise in scientific forward models (e.g. ODEs, algebraic equations) and marginalization techniques (e.g. embedded Laplace approximation, hidden Markov models).

Papers:

* (2020) <span style="color:maroon">Hamiltonian Monte Carlo using an adjoint-differentiated Laplace approximation: Bayesian inference for latent Gaussian models and beyond.</span> C. Margossian, A. Vehtari, D. Simpson and R. Agrawal. _Advances in Neural Information Processing Systems_. [[article](https://proceedings.neurips.cc/paper/2020/hash/673de96b04fa3adcae1aacda704217ef-Abstract.html), [poster](http://charlesm93.github.io/files/poster_ela.pdf), [preprint](https://arxiv.org/abs/2004.12550),
[code](https://github.com/charlesm93/laplace_manuscript)]
* (2019) <span style="color:maroon">A Review of automatic differentiation and its efficient implementation.</span> C. Margossian. _Wiley interdisciplinary reviews: data mining and knowledge discovery_. [[article](https://onlinelibrary.wiley.com/doi/10.1002/widm.1305), [preprint](https://arxiv.org/abs/1811.05031)]

Technical reports:
* (2023) <span style="color:maroon">General adjoint-differentiated Laplace approximation.</span> C. Margossian. [[preprint](https://arxiv.org/abs/2306.14976)]
* (2022) <span style="color:maroon">Approximate Bayesian inference for latent Gaussian models in Stan -- two years later.</span> C. Margossian, S. Bronder, A. Vehtari, D. Simpson and R. Agrawal. [[notebook](https://htmlpreview.github.io/?https://github.com/charlesm93/StanCon2020/blob/master/notebook-2022/lgm_stan.html#inst), [code](https://github.com/charlesm93/StanCon2020)]
* (2022) <span style="color:maroon">Efficient Automatic Differentation of Implicit Functions.</span> C. Margossian and M. Betancourt [[preprint](https://arxiv.org/abs/2112.14217)]
* (2020) <span style="color:maroon">The Discrete adjoint method: efficient derivatives for functions of discrete sequences.</span> M. Betancourt, C. Margossian and V. Leos-Barajas. [[preprint](https://arxiv.org/abs/2002.00326)]


