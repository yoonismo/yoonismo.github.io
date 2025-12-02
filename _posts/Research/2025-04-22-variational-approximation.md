---
layout: post
title:  "[Estimation Algorithm] Variational Regularized Bilevel Estimation for Exponential Random Graph Models"
date:   2025-04-22 16:36:00 -0800
last_modified_at: 2025-10-19 01:15:00 -0800
categories: Research
tag: [ERGM, Variational Approximation, Bilevel Optimization]
---

I propose an estimation algorithm for Exponential Random Graph Models (ERGM), a popular statistical network model for estimating 
structural parameters of strategic network formation in economics and finance. Existing methods often produce unreliable estimates 
of parameters for the triangle, a key network structure that captures the tendency of two persons with shared friends to connect. 
Such unreliable estimates may lead to untrustworthy policy recommendations for networks with triangles. Through a variational 
mean-field approach, my algorithm addresses the two well-known difficulties when estimating the ERGM, the intractability of its 
normalizing constant and model degeneracy. In addition, I introduce l2 regularization that ensures a unique solution to the 
mean-field approximation problem under suitable conditions. I provide a non-asymptotic optimization convergence rate analysis for 
my proposed algorithm under mild regularity conditions. Through Monte Carlo simulations, I demonstrate that my method achieves 100% 
sign recovery rate for triangle parameters for small and mid-sized networks under perturbed initialization, compared to a 50% rate 
for existing algorithms. I provide the sensitivity analysis of estimates of ERGM parameters to hyperparameter choices, offering 
practical insights for implementation.
