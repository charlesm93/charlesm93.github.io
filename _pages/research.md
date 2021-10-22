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


### Writing

I try to post formal articles on [research gate](https://www.researchgate.net/profile/Charles_Margossian).
Here, I'll also lay out other projects and resources.

Preprint and publications:
*(2021) Simulating Ising and Potts models at critical and cold temperatures using auxiliary Gaussian variables. Charles C. Margossian and Sumit Mukherjee. [[preprint](https://arxiv.org/abs/2110.10801)]\
Keywords: _Statistical physics, Random graphs, Spin glass, Gibbs sampling, Tempering._
* (2021) Efficient and flexible Bayesian pharmacometrics modeling using Stan and Torsten, Part I. Charles C. Margossian, Yi Zhang and William R. Gillespie. [[preprint](https://arxiv.org/abs/2109.10184)]\
Keywords: _Pharmacometrics, Bayesian workflow, hierarchical model, Stan, Torsten._
* (2021) Developping a model of SARS-CoV-2 viral dynamics under monoclonal antibody treatment. Aurélien Marc, Marion Kerioui, Charles Margossian, Julie Bertrand, Pauline Maisonnasse, Yoan Aldon, Rogier W Sanders, Marit Van Gils, Roger Le Grand, Jérémie Guedj. _Population Approach Group in Europe_.\
Keywords: _Pharmacometrics, Covid-19, Bayesian workflow, hierarchical model, Stan._
* (2021) Solving ODEs in a Bayesian context: challenges and opportunities. Charles C. Margossian, Lu Zhang, Sebastian Weber and Andrew Gelman. _Population Approach Group in Europe_. [[poster](http://charlesm93.github.io/files/BayesianODE.pdf)]\
Keywords: _Pharmacometrics, ODE-based models, Hamiltonian Monte Carlo, Pathfinder, Stan._
* (2020) Bayesian Workflow. Andrew Gelman et al. [[preprint](https://arxiv.org/abs/2011.01808)]
* (2020) Hamiltonian Monte Carlo using an adjoint-differentiated Laplace approximation: Bayesian inference for latent Gaussian models and beyond. Charles C. Margossian, Aki Vehtari, Daniel Simpson and Raj Agrawal. _NeurIPS 2020_. [[article](https://proceedings.neurips.cc/paper/2020/hash/673de96b04fa3adcae1aacda704217ef-Abstract.html), [poster](http://charlesm93.github.io/files/poster_ela.pdf), [preprint](https://arxiv.org/abs/2004.12550),
 [code](https://github.com/charlesm93/laplace_manuscript)]\
 Keywords: _Hierarchical models, Hamiltonian Monte Carlo, Embedded Laplace approximation, Automatic Differentiation, Gaussian processes, Sparsity inducing priors, Stan._
* (2020) Approximate Bayesian inference for latent Gaussian models in Stan. Charles C. Margossian, Aki Vehtari, Daniel Simpson and Raj Agrawal. _presented at Stan Con 2020_. [[notebook](http://charlesm93.github.io/files/lgm_stan.pdf),
[code](https://github.com/charlesm93/StanCon2020), [talk](https://www.youtube.com/watch?v=hbYsakCQiew&list=PLCrWEzJgSUqzI3goQEAKkDsHg72inmqbe&index=16&t)]\
Keywords: _Hierarchical models, Hamiltonian Monte Carlo, Embedded Laplace approximation, Automatic Differentiation, Gaussian processes, Sparsity inducing priors, Stan._
* (2020) Bayesian Workflow for disease transmission modeling in Stan. Leo Grinsztajn, Elizaveta Semenova, Charles C. Margossian and Julien Riou. _Statistics in medicine_.
[[article](https://onlinelibrary.wiley.com/doi/10.1002/sim.9164), [preprint](https://arxiv.org/abs/2006.02985),
[html file](https://mc-stan.org/users/documentation/case-studies/boarding_school_case_study.html),
[code](https://github.com/stan-dev/example-models/tree/master/knitr/disease_transmission),
[talk](https://www.youtube.com/watch?v=unHZhfur5Sc)]\
Keywords: _Epidimeology, Covid-19, Bayesian workflow, ODE-based models, Stan._
* (2020) Estimation of SARS-CoV-2 mortality during the early stages of an epidemic: a modelling study in Hubei, China and six regions of Europe. Julien Riou et al. _PLOS Medicine_. [[article](https://journals.plos.org/plosmedicine/article?id=10.1371/journal.pmed.1003189),
[preprint](https://www.medrxiv.org/content/10.1101/2020.03.04.20031104v2)]\
Keywords: _Epidimeology, Covid-19, Bayesian modeling, Stan._
* (2020) The Discrete adjoint method: efficient derivatives for functions of discrete sequences. Michael Betancourt, Charles C. Margossian and Vianey Leos-Barajas. [[preprint](https://arxiv.org/abs/2002.00326)]\
Keywords: _Automatic differentiation, Difference equations, Hidden Markov models._
* (2019) A Review of automatic differentiation and its efficient implementation. Charles C. Margossian. _Wiley interdisciplinary reviews: data mining and knowledge discovery_. [[article](https://onlinelibrary.wiley.com/doi/10.1002/widm.1305), [preprint](https://arxiv.org/abs/1811.05031)]\
Keyword: _Automatic differentiation_
* (2018) Computing Steady states with Stan's nonlinear algebraic solver. Charles C. Margossian. _Stan Con Asilomar 2018_. [[article](http://charlesm93.github.io/files/2018-Margossian.pdf), [code](https://github.com/stan-dev/stancon_talks/tree/master/2018/Contributed-Talks/08_margossian), [talk](https://www.youtube.com/watch?v=JhwZIX5ryw0&feature=youtu.be)]\
Keywords: _Pharmacometrics, Bayesian inference, Stan._
* (2017) Gaining Efficiency by combining analytical and numerical methods to solve ODEs: implementation in Stan and application to Bayesian PK/PD modeling. Charles C. Margossian and Bill Gillespie. _Journal of Pharmacokinetics and Pharmacodynamics, presented at the American Conference on Pharmacometrics 8_. [[poster](http://charlesm93.github.io/files/2017b-Margossian&Gillespie-mixed_solver.pdf)]\
Keywords: _Pharmacometrics, Bayesian inference, Stan, Torsten._
* (2017) Differential equation based models in Stan. Charles C. Margossian and Bill Gillespie. _Stan Con 2017_. [[article](http://mc-stan.org/events/stancon2017-notebooks/stancon2017-margossian-gillespie-ode.html), [code](https://github.com/stan-dev/stancon_talks/tree/master/2017/Contributed-Talks/05_margossian), [talk](https://www.youtube.com/watch?v=DJ0c7Bm5Djk&feature=youtu.be&t=2h53m26s)]\
Keywords: _Pharmacometrics, Bayesian inference, Stan._
* (2016) Stan functions for pharmacometrics. Charles C. Margossian and Bill Gillespie. _Journal of Pharmacokinetics and Pharmacodynamics, presented at the American Conference on Pharmacometrics 7_. [[poster](http://charlesm93.github.io/files/2016-Margossian&Gillespie-stan_for_pmx.pdf)]\
Keywords: _Pharmacometrics, Bayesian inference, Stan, Torsten._
* (2014) Planet Hunters. VII. Discovery of a new low-mass, low-density (PH3 C) orbiting Kepler-289
with mass measurements of two additional plamets of two additional planets (PH3 B and D). Joseph Schmitt et al. _Astrophysical Journal_. [[article](http://iopscience.iop.org/article/10.1088/0004-637X/795/2/167/meta;jsessionid=43641D4C5B1CC7595015BE11DDF1239F.c1)]\
Keywords: _Astronomy, Exoplanets, KEPLER._

Technical reports:

* (2020) Bayesian model of planetary motion: exploring ideas for a modeling workflow when dealing with ordinary differential equations and multimodality. Charles C. Margossian and Andrew Gelman. _Stan Case Studies 7_. [[article](https://mc-stan.org/users/documentation/case-studies/planetary_motion/planetary_motion.html), [code](https://github.com/stan-dev/example-models/tree/master/knitr/planetary_motion)]
* The Stan Book. Stan development team. [[manual](https://mc-stan.org/docs/2_18/stan-users-guide/index.html)]
* Torsten User Manual.  Bill Gillespie, Yi Zhang, Charles C. Margossian, and Metrum Research Group. [[manual](https://metrumresearchgroup.github.io/Torsten/)]
* (2018) Technical appendix for Torsten. Charles C. Margossian. _in progress_. [[technical report](https://github.com/charlesm93/presentations-and-writing/blob/master/TorstenAppendix/Torsten_appendix.pdf)]
* Contributing New Functions to Stan. Stan development team. [[wiki page](https://github.com/stan-dev/stan/wiki/Contributing-New-Functions-to-Stan)]


### Softwares

* Stan: a probabilistic programing language. Stan development team. [[Home page](https://mc-stan.org/)]
* Torsten: a pharmacometrics library for Stan. Bill Gillespie, Yi Zhang, Charles C. Margossian, and Metrum Research Group. [[GitHub](https://github.com/metrumresearchgroup/Torsten)]
* mrgsolve: pharmacometrics and quantitative systems pharmacology simulation in R. Kyle Baron and contributors. [[Home page](https://mrgsolve.github.io/)]


### Others

With [Sumit Mukherjee](http://stat.columbia.edu/~sumitm/), I'm working on simulation methods for spin glass models, of which the Ising model is a special case.

In 2018, I worked on an econometrics model with
[Shosh Vasserman](https://scholar.harvard.edu/vasserman/home).
The data generating process of the model involved the solution to a constrained optimization problem, resulting in a discontinuous posterior. Finding an appropriate sampler remains an open problem.
See this discussion on [non-smooth posterior and KKT](https://discourse.mc-stan.org/t/non-smooth-posterior-and-kkt-problem/6281).

In 2018, I did a class project in population genetics with [Elliott Gordon Rodriguez](http://stat.columbia.edu/department-directory/name/elliot-gordon/), working with Guy Sella and his [lab](https://sellalab.biology.columbia.edu/) in the Department of Biological Sciences.

As an undergraduate at Yale, I worked with the [exoplanet group](http://exoplanets.astro.yale.edu/), in the Department of Astronomy.
