---
title: "Open-source Software"
permalink: /software/
author_profile: yes
output:
  html_document:
    df_print: paged
---

My research on methods and algorithms is complemented by the development of open-source software, which empower scientists to make the most out of their data.

# Stan: a probablistic programming language

<center>
<img src="../images/stan.png" alt="hi" class="inline" style="width:50;height:75px;">
</center>

[Stan](https://mc-stan.org/) is a probabilistic programming language that lets users define a probabilistic model, translates it to C++, then performs Bayesian inference using gradient-based algorithms (Markov chain Monte Carlo, variational inference). Stan is used across the physical, biological, and social sciences, as well as in finance, government, medicine, policy, and leisure.

I have been a core developer of Stan since 2016.
I have primarily contributed to Stan's automatic differentiation library and its support for implicit functions including:
* matrix exponential for solving linear ODEs
* algebraic equation solver
* suite of hidden Markov model functions
* integrated Laplace approximation (prototype)





