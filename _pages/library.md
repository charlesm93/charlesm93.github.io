---
# layout: archive
title: "Library"
permalink: /library/
author_profile: no
---
<img src="../images/Books.png" alt="hi" class="inline" style="width:50;height:75px;">

Here are some papers, books, and other resources I have found helpful,
as a researcher and a student.
This is by no means an exhaustive bibliography, rather a list of personal favorites.
I'm very open to recommendations, if you have some suggestions.

### Conceptual articles

These articles discuss the roles of a model and various
approaches to analyzing data. While they are conceptual and even have a philosophical flavor,
they still address very concrete issues.

* **Mathematics for understanding disease** by Robert R. Bies, Marc R. Gastonguay, and Sorell. L. Schwartz.
[[link](https://indiana.pure.elsevier.com/en/publications/mathematics-for-understanding-disease)]
 *Absract: The application of mathematical models to reflect the organization and activity of biological systems can be viewed as a continuum of purpose...*
* **Philosophy and the practice of Bayesian statistics** Andrew Gelman and Cosma Rohilla Shalizi.
[[link](http://www.stat.columbia.edu/~gelman/research/published/philosophy.pdf)]
*Abstract: [...] We argue that the most successful forms of Bayesian statistics [...] accord much better with sophisticated forms of hypothetico-deductivism...*

### Tutorials and case studies

These are great places to get your hands dirty with modeling and coding:

* **Torwards a principled Bayesian workflow** by Michael Betancourt. [[link](https://betanalpha.github.io/assets/case_studies/principled_bayesian_workflow.html)]
*Excerpt: Given a probabilistic model and a particular observation, Bayesian inference is straightforward to implement. [...] Building a probabilistic model that is useful in a given application, however, is a far more open-ended challenge.* I moreover recommend [everything Michael writes](https://betanalpha.github.io/writing/).
* **Advanced Use of Stan, RStan and Torsten for Pharmacometric Applications** by Bill Gillespie.
[[link](https://www.metrumrg.com/course/advanced-use-stan-rstan-torsten-pharmacometric-applications/)]
*The workshop provides a guided hands-on experience in the advanced use of Stan, rstan and Torsten for Bayesian PKPD modeling.* I also recommend most of the [courses offered by Metrum](https://www.metrumrg.com/courses/), for learning about pharmacometrics.

### Algorithms and numerical methods

Your code (be it for a specific model or a general purpose tool) is at its best when you understand the math,
and more broadly the technical details. Sometimes, you need to break the black box open.
Here are some helpful places to start at:

* **A Conceptual Introduction to Hamiltonian Monte Carlo** by Michael Betancourt [[link](https://arxiv.org/abs/1701.02434)]
* **Automatic differentiation in machine learning: a survey** by Atilim G. Baydin et al. [[link](https://arxiv.org/abs/1502.05767)] *Note: this is a great introduction, in part because it compares automatic differentiation to other methods to compute derivatives. Other note: I myself wrote a review on the topic, which in certain ways complements this survey. You may find a preprint on the research page.*
* **The Stan Math Library: Reverse-Mode Automatic Differentiation in C++** by Bob Carpenter et al.[[link](https://arxiv.org/abs/1509.07164)] *Note: this really gets into the details of how autodiff is implemented in Stan. Very enlightning but very dense read.* 
* **Numerical Recipes: the art of scientific computing** by William H. Press. *Note: an old book, which I took from an uncle's library. Very handy.*

### Mathematical statistics

Here are some great books with a proper mathematical treatment of statistics.

* **Statistical Inference** by George Casella and Roger Berger.
* **Theoretical Statistics** by Robert Keener. *Note: more advanced than the previous. PhD level.*

Unfortunately, it is not always clear how to bridge the theory and the applications.
