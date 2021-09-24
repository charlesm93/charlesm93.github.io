---
layout: archive
title: "Library"
permalink: /library/
author_profile: no
---
<img src="../images/Books.png" alt="hi" class="inline" style="width:50;height:75px;">

Here are some papers, books, and other resources I have found helpful, as a researcher and a student.
This is by no means an exhaustive bibliography, rather an (incomplete) list of personal favorites.

### Conceptual articles

These articles discuss the roles of a model and various approaches to analyzing data. 
While they are conceptual and even have a philosophical flavor, they still address very concrete issues.

* Philosophy and the practice of Bayesian statistics. Andrew Gelman and Cosma Rohilla Shalizi.
[[link](http://www.stat.columbia.edu/~gelman/research/published/philosophy.pdf)]. _Abstract: [...] We argue that the most successful forms of Bayesian statistics [...] accord much better with sophisticated forms of hypothetico-deductivism..._
* Mathematics for understanding disease. Robert R. Bies, Marc R. Gastonguay, and Sorell. L. Schwartz.
[[link](https://indiana.pure.elsevier.com/en/publications/mathematics-for-understanding-disease)]. _Absract: The application of mathematical models to reflect the organization and activity of biological systems can be viewed as a continuum of purpose..._

### Tutorials and case studies

These are great places to get your hands dirty with modeling and coding:

* Torwards a principled Bayesian workflow. Michael Betancourt. [[link](https://betanalpha.github.io/assets/case_studies/principled_bayesian_workflow.html)]
_Excerpt: Given a probabilistic model and a particular observation, Bayesian inference is straightforward to implement. [...] Building a probabilistic model that is useful in a given application, however, is a far more open-ended challenge._ I moreover recommend [everything Michael writes](https://betanalpha.github.io/writing/).
* Advanced Use of Stan, RStan and Torsten for Pharmacometric Applications. Bill Gillespie.
[[link](https://www.metrumrg.com/course/advanced-use-stan-rstan-torsten-pharmacometric-applications/)]
_The workshop provides a guided hands-on experience in the advanced use of Stan, rstan and Torsten for Bayesian PKPD modeling._ I also recommend the [courses offered by Metrum](https://www.metrumrg.com/courses/) for learning about pharmacometrics.

### Algorithms and numerical methods

Your code (be it for a specific model or a general purpose tool) is at its best when you understand the math, and more broadly the technical details. 
Sometimes, you need to break the black box open.
Here are some helpful places to start at:

* A Conceptual Introduction to Hamiltonian Monte Carlo. Michael Betancourt. [[link](https://arxiv.org/abs/1701.02434)]
* Automatic differentiation in machine learning: a survey. Atilim G. Baydin et al. [[link](https://arxiv.org/abs/1502.05767)] _This is a great introduction, in part because it compares automatic differentiation to other methods to compute derivatives. Note: I myself wrote a review on the topic, which focuses on the efficient implementation of autodiff. You may find the article on the research page._
* The Stan Math Library: Reverse-Mode Automatic Differentiation in C++. Bob Carpenter et al.[[link](https://arxiv.org/abs/1509.07164)] _This really gets into the details of how autodiff is implemented in Stan. Very enlightning but very dense read._
* Numerical Recipes: the art of scientific computing. William H. Press. _An old book, which I took from an uncle's library. Very handy._

### Textbooks

A classic for Bayesian analysis with a rather pragmatic discussion of the topic.

* Bayesian Data Analysis. Andrew Gelman et al.

Here are some classics with a mathematical and somewhat theoretical treatment of statistics.
Beware that it is not always obvious how to bridge theory and application!

* Statistical Inference. George Casella and Roger Berger.
* Theoretical Statistics. Robert Keener. _Note: more advanced than the previous. PhD level._
