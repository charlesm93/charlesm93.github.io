---
title: "Research"
permalink: /research/
author_profile: no
output:
  html_document:
    df_print: paged
---

My interests lie in applied and computational statistics.
A lot of my work is motivated by problems in Bayesian modeling.
More precisely:

* Simulation algorithms and the computation of high-dimensional integrals.
This encompasses Markov chains Monte Carlo, Gibbs and Hamiltonian Monte Carlo sampling, and approximate methods such as embedded Laplace approximations.
* Automatic differentiation, meaning the computation of derivatives to supports gradient based algorithms.
Emphasis on the differentiation of implicit functions, such as solutions to differential equations.
* Hierarchical and latent Gaussian models, the geometry of their posteriors, and how this interacts with simulation algorithms.
* Bayesian modeling workflows with applications in pharmacometrics, epidimeology, and physics.
* Ising and Spin glass models, graph models, and more generally high-dimensional discrete spaces.


<!--- ### Bayesian workflow

To make the most of our data, we need principled workflows to build, fit, and criticize our models.
This can only be done if our computational tools allow us to express our scientific
ideas and make accurate inference.
Since we will break, debug and revise our models many times, we also need algorithms
that run efficiently.
Moreover, our tools must be expressive, accurate and fast.
I work on the development of such tools and their software implementation,
primarly in the probabilistic programing language [Stan](http://mc-stan.org/).
Stan's primary inference engine is Hamiltonian Monte Carlo (HMC) sampling.

I'm interested in the algorithmic differentiation of models with complex
likelihoods to support gradient-based methods such as HMC.
Examples of such models include DAE-based likelihoods and hidden Markov processes.
I also study hybrid methods that combine HMC with approximate methods,
such as the Laplace approximation,
and can help us tackle models with high-dimensional latent variables.


### Applications in pharmacometrics

Most models in pharmacometrics are based on systems of ordinary differential equations
(ODEs). To do inference on such models, we not only need to solve ODEs, but also to
propagate derivatives through them.
We must furthermore model the broad array of treatments patients can undergo.
To address these issues, I develop general purpose tools for ODE-based models in
Stan. With colleagues at [Metrum](https://metrumrg.com/), I co-created [Torsten](https://github.com/metrumresearchgroup/Torsten),
an extension of Stan with specialized routines for pharmacometrics.
--->


### Writing

I try to post formal articles on [research gate](https://www.researchgate.net/profile/Charles_Margossian).
Here, I'll also lay out other projects and resources.

Preprint and publications:

* (2020) Bayesian model of planetary motion: exploring ideas for a modeling workflow when dealing with ordinary differential equations and multimodality. Charles C. Margossian and Andrew Gelman. _Stan Case Studies 7_. [[article](https://mc-stan.org/users/documentation/case-studies/planetary_motion/planetary_motion.html), [code](https://github.com/stan-dev/example-models/tree/master/knitr/planetary_motion)]

* (2020) Bayesian Workflow. Andrew Gelman et al. [[preprint](https://arxiv.org/abs/2011.01808)]

* (2020) Hamiltonian Monte Carlo using an adjoint-differentiated Laplace approximation. Charles C. Margossian, Aki Vehtari, Daniel Simpson and Raj Agrawal. _NeurIPS 2020_. [[preprint](https://arxiv.org/abs/2004.12550),
 [code](https://github.com/charlesm93/laplace_manuscript)]

* (2020) Approximate Bayesian inference for latent Gaussian models in Stan. Charles C. Margossian, Aki Vehtari, Daniel Simpson and Raj Agrawal. _presented at Stan Con 2020_. [[article](http://charlesm93.github.io/files/lgm_stan.pdf),
[code](https://github.com/charlesm93/StanCon2020), [talk](https://www.youtube.com/watch?v=hbYsakCQiew&list=PLCrWEzJgSUqzI3goQEAKkDsHg72inmqbe&index=16&t)]

* (2020) Bayesian Workflow for disease transmission modeling in Stan. Leo Grinsztajn, Elizaveta Semenova, Charles C. Margossian and Julien Riou.
[[preprint](https://arxiv.org/abs/2006.02985),
[html file](https://mc-stan.org/users/documentation/case-studies/boarding_school_case_study.html),
[code](https://github.com/stan-dev/example-models/tree/master/knitr/disease_transmission),
[talk](https://www.youtube.com/watch?v=unHZhfur5Sc)]

* (2020) Estimation of SARS-CoV-2 mortality during the early stages of an epidemic: a modelling study in Hubei, China and six regions of Europe. Julien Riou et al. _PLOS Medicine_. [[article](https://journals.plos.org/plosmedicine/article?id=10.1371/journal.pmed.1003189),
[preprint](https://www.medrxiv.org/content/10.1101/2020.03.04.20031104v2)]

* (2020) The Discrete adjoint method: efficient derivatives for functions of discrete sequences. Michael Betancourt, Charles C. Margossian and Vianey Leos-Barajas. [[preprint](https://arxiv.org/abs/2002.00326)]

* (2019) A Review of automatic differentiation and its efficient implementation. Charles C. Margossian. _Wiley interdisciplinary reviews: data mining and knowledge discovery_. [[article](https://onlinelibrary.wiley.com/doi/10.1002/widm.1305), [preprint](https://arxiv.org/abs/1811.05031)]
* (2018) Computing Steady states with Stan's nonlinear algebraic solver. Charles C. Margossian. _Stan Con Asilomar 2018_. [[article](http://charlesm93.github.io/files/2018-Margossian.pdf), [code](https://github.com/stan-dev/stancon_talks/tree/master/2018/Contributed-Talks/08_margossian), [talk](https://www.youtube.com/watch?v=JhwZIX5ryw0&feature=youtu.be)]
* (2017) Gaining Efficiency by combining analytical and numerical methods to solve ODEs: implementation in Stan and application to Bayesian PK/PD modeling. Charles C. Margossian and Bill Gillespie. _Journal of Pharmacokinetics and Pharmacodynamics, presented at the American Conference on Pharmacometrics 8_. [[poster](http://charlesm93.github.io/files/2017b-Margossian&Gillespie-mixed_solver.pdf)]
* (2017) Differential equation based models in Stan. Charles C. Margossian and Bill Gillespie. _Stan Con 2017_. [[article](http://mc-stan.org/events/stancon2017-notebooks/stancon2017-margossian-gillespie-ode.html), [code](https://github.com/stan-dev/stancon_talks/tree/master/2017/Contributed-Talks/05_margossian), [talk](https://www.youtube.com/watch?v=DJ0c7Bm5Djk&feature=youtu.be&t=2h53m26s)]
* (2016) Stan functions for pharmacometrics. Charles C. Margossian and Bill Gillespie. _Journal of Pharmacokinetics and Pharmacodynamics, presented at the American Conference on Pharmacometrics 7_. [[poster](http://charlesm93.github.io/files/2016-Margossian&Gillespie-stan_for_pmx.pdf)]
* (2014) Planet Hunters. VII. Discovery of a new low-mass, low-density (PH3 C) orbiting Kepler-289
with mass measurements of two additional plamets of two additional planets (PH3 B and D). Joseph Schmitt et al. _Astrophysical Journal_. [[article](http://iopscience.iop.org/article/10.1088/0004-637X/795/2/167/meta;jsessionid=43641D4C5B1CC7595015BE11DDF1239F.c1)]

Technical reports:

* The Stan Book. Stan development team. [[manual](https://mc-stan.org/docs/2_18/stan-users-guide/index.html)]
* Torsten User Manual. Charles C. Margossian, Yi Zhang, Bill Gillespie and Metrum Research Group. [[manual](https://metrumresearchgroup.github.io/Torsten/)]
* (2018) Technical appendix for Torsten. Charles C. Margossian. _in progress_. [[technical report](https://github.com/charlesm93/presentations-and-writing/blob/master/TorstenAppendix/Torsten_appendix.pdf)]
* Contributing New Functions to Stan. Stan development team. [[wiki page](https://github.com/stan-dev/stan/wiki/Contributing-New-Functions-to-Stan)]


### Softwares

* Stan: a probabilistic programing language. Stan development team. [[Home page](https://mc-stan.org/)]
* Torsten: a pharmacometrics library for Stan. Charles C Margossian, Yi Zhang, Bill Gillespie and Metrum Research Group. [[GitHub](https://github.com/metrumresearchgroup/Torsten)]
* mrgsolve: pharmacometrics and quantitative systems pharmacology simulation in R. Kyle Baron and contributors. [[Home page](https://mrgsolve.github.io/)]


### Others

With [Sumit Mukherjee](http://stat.columbia.edu/~sumitm/), I'm working on simulation methods for spin glass models, of which the Ising model is a special case.

In 2018, I worked on an econometrics model with
[Shosh Vasserman](https://scholar.harvard.edu/vasserman/home).
The data generating process of the model involved the solution to a constrained optimization problem, resulting in a discontinuous posterior. Finding an appropriate sampler remains an open problem.
See this discussion on [non-smooth posterior and KKT](https://discourse.mc-stan.org/t/non-smooth-posterior-and-kkt-problem/6281).

In 2018, I did a class project in population genetics with [Elliott Gordon Rodriguez](http://stat.columbia.edu/department-directory/name/elliot-gordon/), working with Guy Sella and his [lab](https://sellalab.biology.columbia.edu/) in the Department of Biological Sciences.

As an undergraduate at Yale, I worked with the [exoplanet group](http://exoplanets.astro.yale.edu/), in the Department of Astronomy.
