---
title: HTorch - Hyperbolic Learning with MCTensor
summary: We want to build all hyperbolic learning models (with manifolds as Halfspace, Lorentz, Poincare, etc.) on top of MCTensor algorithms. 
tags:
  - Hyperbolic learning
  - Efficient high-precision floating-point arithmetic

date: '2023-10-01'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Table 3 in the [MCTensor paper](https://arxiv.org/pdf/2207.08867.pdf). 

  focal_point: Smart

url_code: 'https://github.com/ydtydr/HTorch'

slides: ""
---

We want to build all hyperbolic learning models (with manifolds as Halfspace, Lorentz, Poincare, etc.) on top of [MCTensor algorithms](https://github.com/ydtydr/MCTensor). This might address the well-known NaN problems in hyperbolic learning, especially for manifolds that are known to be numerically unrobust (Poincare). We have released a library called [HTorch](https://github.com/ydtydr/HTorch) and we will continue to develop and maintain such library. We are looking forward to writing a paper on `HTorch`.