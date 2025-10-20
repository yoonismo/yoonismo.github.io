---
layout: post
title:  "[Missing Data] Wasserstein Distributionally Robust Linear Quantile Regression on Missing Data"
date:   2023-04-22 14:22:00 -0800
last_modified_at: 2025-10-19 01:16:00 -0800
categories: Research
tag: [Distributionally Robust Optimization, Missing Data, Quantile Regression]
---

This paper proposes a Distributionally Robust (DR) linear quantile estimator to handle deviations from the "Missing At Random" (MAR) assumption in incomplete data. While MAR-based estimators can perform poorly when the missingness mechanism deviates from MAR, fully assumption-free approaches yield overly conservative bounds. To address this, we introduce a distributionally robust optimization framework using the Wasserstein distance to measure departures from the MAR distribution. The estimator solves a minimax optimization problem by maximizing the worst-case expected loss over a Wasserstein ball and minimizing it with respect to the parameter of interest.