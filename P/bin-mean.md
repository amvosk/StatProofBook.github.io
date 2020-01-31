---
layout: proof
mathjax: true

author: "Joram Soch"
affiliation: "BCCN Berlin"
e_mail: "joram.soch@bccn-berlin.de"
date: 2020-01-16 11:06:00

title: "Mean of the binomial distribution"
chapter: "Probability Distributions"
section: "Univariate discrete distributions"
topic: "Binomial distribution"
theorem: "Mean"

dependencies:
  - theorem: "linearity of the expected value"
  - theorem: "expected value of the Bernoulli distribution"
    shortcut: "bern-mean"

sources:
  - authors: "Wikipedia"
    year: 2020
    title: "Binomial distribution"
    in: "Wikipedia, the free encyclopedia"
    pages: "retrieved on 2020-01-16"
    url: "https://en.wikipedia.org/wiki/Binomial_distribution#Expected_value_and_variance"

proof_id: "P23"
shortcut: "bin-mean"
username: "JoramSoch"
---


**Theorem:** Let $X$ be a random variable following a binomial distribution:

$$ \label{eq:bin}
X \sim \mathrm{Bin}(n,p) \; .
$$

Then, the mean or expected value of $X$ is

$$ \label{eq:bin-mean}
\mathrm{E}(X) = n p \; .
$$


**Proof:** By definition, a binomial random variable is the sum of $n$ independent and identical Bernoulli trials with success probability $p$. Therefore, the expected value is

$$ \label{eq:bin-mean-s1}
\mathrm{E}(X) = \mathrm{E}(X_1 + \ldots + X_n)
$$

and because the expected value is a linear operator, this is equal to

$$ \label{eq:bin-mean-s2}
\begin{split}
\mathrm{E}(X) &= \mathrm{E}(X_1) + \ldots + \mathrm{E}(X_n) \\
&= \sum_{i=1}^{n} \mathrm{E}(X_i) \; .
\end{split}
$$

With the expected value of the Bernoulli distribution, we have:

$$ \label{eq:bin-mean-s3}
\mathrm{E}(X) = \sum_{i=1}^{n} p = n p \; .
$$