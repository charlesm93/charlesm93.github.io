---
title: '💭 One of my favorite papers (that I have written)'
date: November 15th 2025
permalink: /posts/2025/09/blog-post-3/
tags:
  - research
  - variational inference
---

During my academic job search, I was sometimes asked what my favorite paper was.
I like this question because it's an invitation to discuss not simply a good
paper but also a good story, one that dives into the inevitable setbacks
of research, the joy of overcoming them and the beauty of doing it all with
great colleagues. Today, I'd like to share one such story.

The paper is [Variational Inference for Uncertainty Quantification](https://arxiv.org/abs/2403.13748),
written with Lawrence Saul and Loucas Pillaud-Vivien to appear in the
_Journal of Machine Learning Research_ and here's the abstract:

_Given an intractable distribution $p$, the problem of variational inference (VI) is to find the best approximation from some more tractable family $\mathcal Q$. Commonly, one chooses $\mathcal Q$ to be a family of factorized distributions (i.e., the mean-field assumption), even though $p$ itself does not factorize. We show that this mismatch can lead to an impossibility theorem: if $p$ does not factorize and furthermore has a non-diagonal covariance matrix, then any factorized approximation $q \in \mathcal Q$ can correctly estimate at most one of the following three measures of uncertainty: (i) the marginal variances, (ii) the marginal precisions, or (iii) the generalized variance (which for elliptical distributions is closely related to the entropy). In practice, the best variational approximation in $\mathcal Q$ is found by minimizing some divergence $D(q,p)$ between distributions, and so we ask: how does the choice of divergence determine which measure of uncertainty, if any, is correctly estimated by VI? We consider the classic Kullback-Leibler divergences, the more general $\alpha$-divergences, and a score-based divergence which compares $\nabla \log p$ and $\nabla \log q$. We thoroughly analyze the case where $p$ is a Gaussian and $q$ is a (factorized) Gaussian. In this setting, we show that all the considered divergences can be ordered based on the estimates of uncertainty they yield as objective functions for VI. Finally, we empirically evaluate the validity of this ordering when the target distribution p is not Gaussian._

**Disclaimer:** During the job search, this was _not_ the paper I spoke about :)
My favorite paper (that I've written) is probably still the [nested $\widehat R$ paper](https://arxiv.org/abs/2110.13017).
But when I got home from an interview, I started thinking, the VI for uncertainty
_could've_ also been a good paper to discuss and I drafted this blog post way
back in February.

(February 9th 2025)

A textbook question
---

A little over two years ago, I started working on variational inference (VI).
As I read the literature, I kept coming across the comment that “VI
underestimates uncertainty” and I wanted to convince myself of this fact with
a simple example. Say I approximate a non-factorized Gaussian with a factorized
Gaussian, can I show that the approximation always underestimates the marginal
variances? So I scribbled and scribbled, and I didn’t get anywhere.
No problem: VI legend Lawrence Saul was down the hall
(at the [Flatiron Institute](https://www.simonsfoundation.org/flatiron/center-for-computational-mathematics/)),
and I submitted this textbook problem to him. He agreed the result seemed elementary.
In fact, many books and review papers proved the claim in 2-D, and it seemed
straightforward to generalize it to higher dimensions.

So we went to the black board, and we tinkered, and tinkered, and… hmmm…
could this problem be harder than we thought?

We did eventually write a proof: it was short but unintuitive. (I didn’t like
this proof.) (The excellent paper by [Turner & Sahini (2011)](https://www.gatsby.ucl.ac.uk/~maneesh/papers/turner-sahani-2010-ildn.pdf)
has a statement of the result, albeit without a proof.)
Then we derived more results on variance estimation and wrote a [precursor](https://proceedings.mlr.press/v216/margossian23a/margossian23a.pdf) to our paper on VI uncertainty.


A fleeting shadow
---

Lawrence felt strongly that in addition to variance we should also analyze entropy
as a measure of uncertainty. And we did find that VI also underestimates entropy.
But when I ran numerical experiments, something surprising
transpired. As dimension increased, I found that estimates of the variance
became worst, while estimates of the entropy improved. This contradicted our
visuals: the volume of the approximating sphere was clearly much smaller than
the volume of the target ellipsoid. For entropies to match, you would need
the volumes of the two objects to be the same.

<br><center>
<img src="{{ '/images/ellipse.png' | relative_url }}" alt="hi" class="inline" style="width:100;height:150px;">
</center><br>
Fig1. _Factorized Gaussian approximation of an $n$-dimensional Gaussian. The target
has a covariance matrix with constant off-diagonal element $\varepsilon$._

I checked and double-checked my code, and I couldn’t find an error. And then I
had a happy thought. The two dimensional picture we were looking at was
misleading. The sphere was not smaller than the ellipsoid, even though its shadow was.
Each time we “added” back a dimension, the sphere would grow in every direction, while the
ellipsoid would only grow a little bit. Until eventually, the volume of the
two objects nearly matched.

Here’s another way to understand the result. Setting correlations to 0 (as one
does with the factorized/mean-field approximation) increases entropy. If our
goal is to match the entropy of the target, the increase in volume caused by
the null correlation must be compensated by a shrinkage in the marginal variances.
Conversely, matching the variances means overestimating the entropy of the target. The two
measures of uncertainty therefore compete with one another. This fact is
elegantly captured by an equation we termed the _shrinkage-delinkage trade-off_.
Here it is, without any proper definition of the terms but just to highlight its simplicity:
<br><center>
$$ \Delta \mathcal H = \frac{1}{2} \log |S| - \frac{1}{2} \log |C|^{-1}. $$
</center><br>
This late result became the main character of our precursor paper.

I [presented this result at the UAI conference 2023](https://www.youtube.com/watch?v=2q5azatd-Ko) in Pittsburg. It was a fun
conference, mostly because I met some amazing PhD students and postdocs to
hang out with. I should now mention that all the work Lawrence and I did was
based on minimizing the reverse Kullback-Leibler divergence,
<br><center>
$$
\text{KL}(q||p) = \int (\log q(z) - \log p(z)) q(z) \text d z,
$$
</center><br>
which is the usual
objective function we minimize in VI. Many people asked me if I had thought
about what would happen if I minimized other divergences
and I figured this would be a straightforward extension.
It would also allow me to address a question that had long pre-occupied me,
namely what is the best way to compare probability distributions?


Thanksgiving break
---

So back to the blackboard (we have beautiful blackboards at the Flatiron
Institute). I looked at a few divergences and even some metrics. Did you
know there is not analytical expression for the total variation distance
between two multivariate Gaussians? It turned out the KL-divergence was
particularly easy to manipulate, with other divergences posing additional
challenges. Still, we made progress, one divergence at a time.

I had another small breakthrough on Thanksgiving. I remember I was taking the
bus to Pennsylvania. I had missed my original bus and then, I received an email,
telling me another paper of mine had gotten rejected. I read the reviews and
felt absolutely gutted. I can still see it: the overcrowded bus terminal, the
endless waiting, the phone call I made to a close one, the reviews I read and
re-read and re-read. It was a sunny day. I was fortunate to be with family that
day. And the next morning, I woke up early and felt the need to make amends
for my “failure”. I sat in the kitchen and extended the shrinkage-delinkage
trade-off to a three-way impossibility theorem between precision, variance,
and entropy.


Loucas’ napkin
---

I had intended to submit a manuscript by the end of November, with the hope
that within a year, my paper would be reviewed and accepted, and that this
would strengthen my application for my next job. (None of this happened.) Some
of the results resisted us. Lawrence and I had an incredibly difficult time
proving an “ordering” of the Renyi $\alpha$-divergences. We felt close: each
week, we believed we would finish the proof; and each week, the last piece
of the puzzle eluded us.

One day, I was working at the white board, messing around with the terms of
an equation. My then fellow post-doc Loucas Pillaud-Vivien walked by and asked
me what I was working on. So I explained the problem. He then grabbed a marker
and began working in his corner of the white board. He shared his ideas, his
perspective as a theorist and a probabilist. He spoke about “agreeable facts”,
he dug out results from linear algebra that I wasn’t familiar with. It was also
fun for me to revisit the topic in French, somehow it gave me a fresh
perspective. (Loucas was also French.)


And so, Loucas joined forces with Lawrence and I. I remember the day when we
finally cracked the proof. It was a Friday. We  felt close (as always) and it
was getting late. Another one of our colleagues brought beers and we drank
them in front of the white board. Now we were one or two details away from
the contradiction that would complete the proof. But I had a ballroom dance
practice and I left the office.

Later that night, while I was warming up at the dance studio, I got a message
from Loucas: "I think I got it. You can dance in peace." Dance in peace?? No,
I had to see the proof for myself before being "at peace". Right after practice,
Loucas and I met at the usual Mexican bar and he completed the proof on a napkin, which is
a cliche, but we had ran out of paper.

After that, it took me quite a bit of time to check all the proofs, scattered
in my notebooks, and patch together the missing details. And of course,
Lawrence made an heroic effort editing the manuscript and making sure it lived
up to his very high writing standards.
I suppose the story is far from finished, since the paper is still under review…!


Afterthought
---
(November 11th)

I don’t believe there’s anything extraordinary about this project. It’s a
typical good research story and illustrates one of the happy collaborations I
had as a postdoc. Some of the results seem elementary, or to use a more
flattering word, fundamental. (A reviewer criticized results I had in another
paper as "elementary" and it had never occurred to me that this word could
have a negative connotation.) I trust we will see the results we derived in
upcoming textbooks. With time, I was able to simplify several of the proofs.
At this point, I am aware of four proofs to show VI underestimates variance,
each offering its particular perspective.

p.s. The paper was desk-rejected from a first journal. We then revised it quite
a bit and sent it to JMLR. After a few months, we got requests for some
minor revisions and the paper was published another few months later.
