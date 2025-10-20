---
layout: post
title:  "[Estimation Algorithm] Variational Bi-level Estimation for Exponential Random Graph Models"
date:   2025-04-22 16:36:00 -0800
last_modified_at: 2025-10-19 01:15:00 -0800
categories: Research
tag: [ERGM, Variational Approximation, Bi-level Optimization]
---

Empirical studies of social networks often focus on higher-order interdependencies such as centralization and clustering. Exponential Random Graph model (ERGM) is a popular and versatile statistical parametric model that allows estimation of interdependency terms such as $k-$stars and triangles. Estimation of ERGM is challenging due to two aspects: the intractable normalizing constant and model degeneracy. We propose a variational bilevel estimation algorithm of ERGM that addresses both dilemmas. It mitigates the intractability of normalizing constant by a mean-field approximation. In addition, adoption of $\ell_2$ (Tikhonov) regularization facilitates finding a unique solution to the mean-field approximation problem. We also provide a non-asymptotic convergence analysis of stationary points obtained by our proposed algorithm under mild regularity conditions. Through Monte Carlo simulations, we demonstrate our method's effectiveness over existing MCMC-based algorithms and variational baseline and study the sensitivity of hyperparameter choices to objective values, offering a practical guide for implementation.