---
title:
excerpt: About me
permalink: /
redirect_from:
- /about/
- /about.html
author_profile: yes
font-size: 12pt
---


I am a Research Fellow in Computational Mathematics at the [Flatiron Institute](https://www.simonsfoundation.org/flatiron/), a part of the [Simons Foundation](https://www.simonsfoundation.org/). In 2022, I earned a PhD in Statistics from Columbia University. You can find out more by browsing this website or looking at my [CV](http://charlesm93.github.io/files/charlesmcv.pdf).

# News

* <span style="color:Tomato">I am on the job market this year!</span> I am looking for research positions, including faculty positions, in statistics, data science, and machine learning which would start in the summer/fall of 2025. Feel free to reach out if you wish to share an opportunity.

* I will be attending the workshop on "Recent Advances and Future Directions for Sampling" at Yale on October 16th - 18th.

(last updated: October 2024)

# About

My primary research interest lies in statistics and probabilistic machine learning. My work bridges methodology, computation, and application through the development of probabilistic programing languages such as [Stan](http://mc-stan.org/) and [TensorFlow Probability](https://www.tensorflow.org/probability). Some keywords:

* **Computation:** Markov chain Monte Carlo, Variational inference, (integrated) Laplace approximation, automatic differentiation
* **Modeling:** Bayesian workflow, Hierarchical models, ODE-based models
* **Applications:** Pharmacometrics, Epidimeology, (Astro)physics



<!--### Past news-->
<!---->
<!--* [StanCon 2024](https://mc-stan.org/events/stancon2024/) will be held at Oxford University in the UK, September 12th - 14th!-->
<!--* This June, I'll be teaching a course on Monte Carlo methods, as part of the [Nordic Probabilistic AI school](https://nordic.probabilistic.ai/) in Copenhagen, Denmark.-->
<!--* I was the invited guess for the podcast [learning Bayesian statistics](https://learnbayesstats.com/episode/90-demystifying-mcmc-variational-inference-charles-margossian/), hosted by Alex Andorra. Our episode: "Demystifying MCMC and Variational Inference".-->
<!--* My [interview](https://www.simonsfoundation.org/2023/06/12/between-knowing-nothing-and-knowing-for-sure-the-science-of-uncertainty/) for the Simons Foundation with science writer Mara Johnson-Groh is out. It provides an accessible overview of my research.-->

# Papers

* (2024) <span style="color:maroon">Variational Inference in Location-Scale Families: Exact Recovery of the Mean and Correlation Matrix.</span> C.Margossian and L. Saul. [[pdf](https://arxiv.org/abs/2410.11067)]
* (2024) <span style="color:maroon">Variational Inference for Uncertainty Quantification: an Analysis of Trade-Offs.</span> C. Margossian, L. Pillaud-Vivien and L. Saul. [[pdf](https://arxiv.org/abs/2403.13748), [Code](https://github.com/charlesm93/VI-ordering)]
* (2024) <span style="color:maroon">Nested $\widehat R$: Assessing the convergence of Markov chain Monte Carlo when running many short chains.</span> C. Margossian, M. Hoffman, P. Sountsov, L. Riou-Durand, A. Vehtari and A. Gelman. _Bayesian Analysis_ [[article](https://projecteuclid.org/journals/bayesian-analysis/advance-publication/Nested-R%cb%86--Assessing-the-Convergence-of-Markov-Chain-Monte/10.1214/24-BA1453.full), [pdf](https://arxiv.org/abs/2110.13017), [code](https://github.com/charlesm93/nested-rhat)]
* (2024) <span style="color:maroon">EigenVI: score-based variational inference with orthogonal function expansions.</span> D. Cai, C. Modi, C. Margossian, R. Gower, D. Blei and L. Saul. _Advances in Neural Information Processing Sysmtes_ (spotlight)
* (2024) <span style="color:maroon">Listening to the Noise: Blind Denoising with Gibbs Diffusion.</span> D. Heurtel-Depeiges, C. Margossian, R. Ohana and B. Regaldo-Saint Blancard. _PMLR: International Conference on Machine Learning_ [[article](https://proceedings.mlr.press/v235/heurtel-depeiges24a.html), [pdf](https://arxiv.org/pdf/2402.19455.pdf), [code](https://github.com/rubenohana/Gibbs-Diffusion)]
* (2024) <span style="color:maroon">Batch and match: black-box variational inference with a score-based divergence.</span> D. Cai, C. Modi, L. Pillaud-Vivien, C. Margossian, R. Gower, D. Blei and L. Saul. _PMLR: International Conference on Machine Learning_ (spotlight) [[article](https://proceedings.mlr.press/v235/cai24d.html), [pdf](https://arxiv.org/abs/2402.14758), [code](https://github.com/modichirag/GSM-VI)]
* (2024) <span style="color:maroon">Amortized Variational Inference: when and why?</span> C. Margossian and D. Blei. _PMLR: Uncertainty in Artificial Intelligence_ [[article](https://proceedings.mlr.press/v244/margossian24a.html),[pdf](https://arxiv.org/abs/2307.11018), [code](https://github.com/charlesm93/AVI-when-and-why), [talk](https://www.youtube.com/watch?v=vluu7BxA6js)]
* (2024) <span style="color:maroon">For how many iterations should we run Markov chain Monte Carlo?</span> C. Margossian and A. Gelman. _Handbook of Markov chain Monte Carlo_, (upcoming) 2nd Edition. [[pdf](https://arxiv.org/abs/2311.02726)]
* (2023) <span style="color:maroon">Variational Inference with Gaussian Score Matching.</span> C. Modi, C. Margossian, Y. Yao, R. Gower, D. Blei and L. Saul. _Advances in Neural Information Processing Systems_ [[article](https://proceedings.neurips.cc/paper_files/paper/2023/hash/5f9453c4848b89d4d8c5d6041f5fb9ec-Abstract-Conference.html), [pdf](https://arxiv.org/abs/2307.07849), [code](https://github.com/modichirag/GSM-VI)]
* (2023) <span style="color:maroon">The Shrinkage-Delinkage Trade-off: An Analysis of Factorized Gaussian Approximations for Variational Inference.</span> C. Margossian and L. Saul. _PMLR: Uncertainty in Artificial Intelligence_ (Oral) [[article](https://proceedings.mlr.press/v216/margossian23a/margossian23a.pdf), [pdf](https://arxiv.org/abs/2302.09163), [code](https://github.com/charlesm93/variance-delinkage), [talk](https://www.youtube.com/watch?v=2q5azatd-Ko)]
* (2022) <span style="color:maroon">Adaptive Tuning for Metropolis Adjusted Langevin Trajectories.</span> L. Riou-Durand, P. Sountsov, J. Vogrinc, C. Margossian and S. Power. _PMLR: Artificial Intelligence and Statistics_ [[article](https://proceedings.mlr.press/v206/riou-durand23a/riou-durand23a.pdf), [pdf](https://arxiv.org/abs/2210.12200), [code](https://github.com/tensorflow/probability/tree/main/discussion/adaptive_malt)]
* (2022) <span style="color:maroon">Flexible and efficient Bayesian pharmacometrics modeling using Stan and Torsten, Part I.</span> C. Margossian, Y. Zhang and  W. Gillespie. _CPT: Pharmacometrics & Systems Pharmacology_. [[article](https://ascpt.onlinelibrary.wiley.com/doi/10.1002/psp4.12812), [pdf](https://arxiv.org/abs/2109.10184), [code](https://github.com/metrumresearchgroup/torsten_tutorial_1_supplementary), [software](https://metrumresearchgroup.github.io/Torsten/)]
* (2021) <span style="color:maroon">Fast methods for posterior inference of two-group normal-normal models.</span> P. Greengard, J. Hoskins, C. Margossian, A. Gelman and A. Vehtari. _Bayesian Analysis_. [[article]( https://projecteuclid.org/journals/bayesian-analysis/advance-publication/Fast-Methods-for-Posterior-Inference-of-Two-Group-Normal-Normal/10.1214/22-BA1329.full), [pdf](https://arxiv.org/abs/2110.03055), [R package](https://github.com/pgree/fastNoNo)]
* (2021) <span style="color:maroon">Bayesian Workflow for disease transmission modeling in Stan.</span> L. Grinsztajn, E. Semenova, C. Margossian and J. Riou. _Statistics in medicine_.
[[article](https://onlinelibrary.wiley.com/doi/10.1002/sim.9164), [preprint](https://arxiv.org/abs/2006.02985),
[code](https://github.com/stan-dev/example-models/tree/master/knitr/disease_transmission),
[talk](https://www.youtube.com/watch?v=unHZhfur5Sc)]
* (2020) <span style="color:maroon">Bayesian Workflow.</span> A. Gelman et al. [[pdf](https://arxiv.org/abs/2011.01808)]
* (2020) <span style="color:maroon">Hamiltonian Monte Carlo using an adjoint-differentiated Laplace approximation: Bayesian inference for latent Gaussian models and beyond.</span> C. Margossian, A. Vehtari, D. Simpson and R. Agrawal. _Advances in Neural Information Processing Systems_. [[article](https://proceedings.neurips.cc/paper/2020/hash/673de96b04fa3adcae1aacda704217ef-Abstract.html), [poster](http://charlesm93.github.io/files/poster_ela.pdf), [pdf](https://arxiv.org/abs/2004.12550),
[code](https://github.com/charlesm93/laplace_manuscript)]
* (2020) <span style="color:maroon">Estimation of SARS-CoV-2 mortality during the early stages of an epidemic: a modelling study in Hubei, China and six regions of Europe.</span> J. Riou et al. _PLOS Medicine_. [[article](https://journals.plos.org/plosmedicine/article?id=10.1371/journal.pmed.1003189),
[pdf](https://www.medrxiv.org/content/10.1101/2020.03.04.20031104v2)]
* (2019) <span style="color:maroon">A Review of automatic differentiation and its efficient implementation.</span> C. Margossian. _Wiley interdisciplinary reviews: data mining and knowledge discovery_. [[article](https://onlinelibrary.wiley.com/doi/10.1002/widm.1305), [pdf](https://arxiv.org/abs/1811.05031)]
* (2014) <span style="color:maroon">Planet Hunters. VII. Discovery of a new low-mass, low-density (PH3 C) orbiting Kepler-289
with mass measurements of two additional plamets of two additional planets (PH3 B and D).</span> J. Schmitt et al. _Astrophysical Journal_. [[article](http://iopscience.iop.org/article/10.1088/0004-637X/795/2/167/meta;jsessionid=43641D4C5B1CC7595015BE11DDF1239F.c1)]
