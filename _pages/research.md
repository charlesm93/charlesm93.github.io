---
# layout: archive
title: "Research"
permalink: /research/
author_profile: no
---

My interests lie in applied and computational statistics. A few keywords: 

* **Methods**: Bayesian inference, hierarchical models, probabilistic programing, simulation algorithms,  
    automatic differentiation, differential equations
* **Applications**:  pharmacometrics, systems biology, physics, astronomy


### Bayesian modeling

To make the most of our data, we need principled workflows to build, fit, and criticize our models.
This can only be done if our computational tools allow us to express our scientific
ideas and make accurate inference.
Since we will break, debug, and improve our models many times, we also need algorithms
that run efficiently.
Moreover, our tools must be expressive, accurate, and fast.

I work on the development of such tools and their software implementation,
primarly in the probabilitic programing language [Stan](http://mc-stan.org/).
Recently, I've been working on fast Bayesian approximation algorithms,
differentiation methods, and fitting hierarchical models.


### Applications in pharmacometrics

Most models in pharmacometrics are based on systems of ordinary differential equations
(ODEs). To do inference on such models, we not only need to solve ODEs, but also to
propagate derivatives through them.
We must furthermore model the broad array of treatments patients can undergo.
To address these issues, I develop general purpose tools for ODE-based models in
Stan. With colleagues at [Metrum](https://metrumrg.com/), I co-created [Torsten](https://github.com/metrumresearchgroup/Torsten), 
an extension of Stan with specialized routines for pharmacometrics.

### Others

Certain mathematical formalisms persevere accross disciplines.
ODEs, for example, are used in pharmacometrics, astronomy, physics, epidimeology, and more.
As a result, my work sometimes leads me to collaborate with experts in fields I'm less familiar with.
Recently, I've been spending time on a rather difficult econometrics model with 
[Shosh Vasserman](https://scholar.harvard.edu/vasserman/home).

I also have a nascent interest in genetics, which I cultivate by attending journal meetings
at professor [Guy Sella's lab](https://sellalab.biology.columbia.edu/).

As an undergraduate at Yale, I worked with the [exoplanet group](http://exoplanets.astro.yale.edu/),
in the astronomy department.

Other things on my mind: the various formluations of a model (as a scientific
hypothesis, a probabilistic model, and a programing statement),
causal inference,
and the cultural difference between physics and biology.

### Writing

I try to post formal articles on [research gate](https://www.researchgate.net/profile/Charles_Margossian).
Here, I'll also lay out other projects and resources.

Journal and conference articles:

* (2019) A Review of automatic differentiation and its efficient implementation [[article](https://onlinelibrary.wiley.com/doi/10.1002/widm.1305), [preprint](https://arxiv.org/abs/1811.05031)]
* (2018) Computing Steady States with Stan's Nonlinear Algebraic Solver [[article](https://www.researchgate.net/publication/323834530_Computing_steady_states_with_Stan's_nonlinear_algebraic_solver), [code](https://github.com/stan-dev/stancon_talks/tree/master/2018/Contributed-Talks/08_margossian), [talk](https://www.youtube.com/watch?v=JhwZIX5ryw0&feature=youtu.be)]
* (2017) Gaining Efficiency by Combining Analytical and Numerical Methods to Solve ODEs: Implementation in Stan and Application to Bayesian PK/PD Modeling (with Bill Gillespie) [[poster](https://www.researchgate.net/publication/323834519_Gaining_efficiency_by_combining_analytical_and_numerical_methods_to_solve_ODEs_Implementation_in_Stan_and_application_to_Bayesian_PKPD_modeling)]
* (2017) Differential equation based models in Stan (with Bill Gillespie) [[article](http://mc-stan.org/events/stancon2017-notebooks/stancon2017-margossian-gillespie-ode.html), [code](https://github.com/stan-dev/stancon_talks/tree/master/2017/Contributed-Talks/05_margossian), [talk](https://www.youtube.com/watch?v=DJ0c7Bm5Djk&feature=youtu.be&t=2h53m26s)]
* (2016) Stan Functions for pharmacometrics (with Bill Gillespie) [[poster](https://www.researchgate.net/publication/323834461_Stan_functions_for_pharmacometrics_modeling)]
* (2015) Testing the effects of close-in giant planets on stellar magnetic activity (senior thesis)
* (2014) Planet Hunters. VII. Discovery of a new low-mass, low-density (PH3 C) orbiting Kepler-289
with mass measurements of two additional plamets of two additional planets (PH3 B and D) (by Joseph Schmitt et al.) [[article](http://iopscience.iop.org/article/10.1088/0004-637X/795/2/167/meta;jsessionid=43641D4C5B1CC7595015BE11DDF1239F.c1)]

Software documentation (manuals, technical reports, and short articles):

* The Stan Book (with the Stan development team) [[manual](https://mc-stan.org/docs/2_18/stan-users-guide/index.html)]
* Torsten User Manual (with Bill Gillespie and Yi Zhang) [[manual](https://metrumresearchgroup.github.io/Torsten/)]
* (2018) Technical appendix for Torsten [[technical report](https://github.com/charlesm93/presentations-and-writing/blob/master/TorstenAppendix/Torsten_appendix.pdf)]
* Contributing New Functions to Stan (with some colleagues on the Stan development team) [[wiki page](https://github.com/stan-dev/stan/wiki/Contributing-New-Functions-to-Stan)]


### Softwares

* Stan: a probabilistic programing language (with the Stan development team) [[Home page](https://mc-stan.org/)]
* Torsten: a pharmacometrics library for Stan (with Bill Gillespie and Yi Zhang) [[GitHub](https://github.com/metrumresearchgroup/Torsten)]
* mrgsolve: pharmacometrics and quantitative systems pharmacology simulation in R (led by Kyle Baron) [[Home page](https://mrgsolve.github.io/)]
