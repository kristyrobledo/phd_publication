---
# Example from https://joss.readthedocs.io/en/latest/submitting.html
title: 'VarReg: An R package for regression in the location, shape and scale'
tags:
  - R
  - algorithms
  - semi parametric
authors:
  - name: Kristy P Robledo
    orcid: 0000-0003-0213-7652
    affiliation: 1 # (Multiple affiliations must be quoted)
  - name: Ian C MArschner 2
    orcid: 0000-0000-0000-0000
    affiliation: 1
affiliations:
 - name: NHMRC Clinical Trials Centre, University of Sydney
   index: 1
citation_author: Robledo KP et. al.
date: 5 February 
year: 2020
formatted_doi: 0000/joss.0000
bibliography: references.bib
output: rticles::joss_article
csl: apa.csl
journal: JOSS
---

# Introduction

Variance regression models arise in a variety of contexts, including measurement error and variance heterogeneity in standard linear regression analysis. Such models are necessary when the variance of the outcome measure changes as a covariate changes. The use of a variance regression model in these contexts allows the modelling of the variance in terms of covariates, either because the variance itself is of interest, or to increase the precision in estimation of the mean. In some areas, such as biomarker analysis, it may be that the variance itself is of interest.

We can consider the variance regression model as
\begin{equation} 
X_i \sim N\left( f(x_i), g(x_i) \right), ~~~ i=1,2,...,n
\end{equation}
where $g( )$ and $h( )$ are known functions of a covariate $x_i$. This can also be extended to 
 \begin{equation} 
X_i \sim N\left(\sum f(x_{ij}), \sum g(z_{ij}) \right), ~~~ i=1,2,...,n
\end{equation}
where we consider multiple covariates, and also that the covariates in the mean model are not necessarily the same covariates as the variance model.

Generally, the variance regression model [@Aitkin1987; @Verbyla1993; @Smyth2002] uses a log-link model, $h(z)=\log(z)$, and thus the covariates affect the variance multiplicatively. This is primarily because covariate effects in variance heterogeneity models can be negative as well as positive, and the use of a multiplicative model ensures that the overall error variance remains non-negative. Since this is simply a computational convenience, it may be that additive variance heterogeneity is more appropriate in some contexts. Indeed, additive decomposition of the variance is standard in other contexts, such as variance components models and genome-wide association studies. An attractive property of additive variance models is that spline models are effectively additive models, so semi-parametric models are obtained with little additional effort.

# General model

## Variance regression

## Censoring

## Location, Shape and Scale

# Computational method

# `VarReg` Package

## Input arguments and examples

## Computational methods

## Output and plots

# Discussion


# Acknowledgements

?None

# References