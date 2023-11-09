# BayeSeg: Bayesian Modeling for Medical Image Segmentation with Interpretable Generalizability

This is the reading report from paper ["BayeSeg: Bayesian Modeling for Medical Image Segmentation with Interpretable Generalizability"](https://arxiv.org/abs/2303.01710), 
their code can be found in ["https://zmiclab.github.io/projects.html"](https://zmiclab.github.io/projects.html).

The author of this paper is [Shangqi Gao](https://shangqigao.github.io/#), who graduates from [Prof. Xiahai Zhuang's](https://zmiclab.github.io/zxh/) team, 
and currently works as a postdoctoral researcher in University of Oxford, directed by [Prof. Clare Verrill](https://www.nds.ox.ac.uk/team/clare-verrill) and [Prof. Jens Rittscher](https://www.ndm.ox.ac.uk/team/jens-rittscher).

### Motivation
[Domain Shift](https://github.com/xiaovhua/Interpretability-of-Medical-Data-/blob/main/Concept/Domain%20Shift.md) is common in medical problems. [Domain Generalization]()(e.g. data-based, learning-based, and representation-based methods) is an effiective technique for the problem, among which extracting domain-invariant features is one of the most popular strategies for the issue. However, the **_interpretability of domain-invariant features_** remains a challenge. To this end, the authors proposed an interpretable Bayesian framework termed BayeSeg for medical image segmentation. 

Specifically, in order to extract interpretable domain-invariant features, the authors:
##### (1) assumed that an image can be represented by a spatial-correlated variable and a spatial-variant variable, and assigned hierarchical Bayesian priors to explicitly force them to model the domain-stable (cross-domain) shape and domain-specific (inter-domain) appearance information respectively; 
##### (2) modeled the segmentation as a locally smooth variable only related to the spatial-correlated variable, or termed domain-stable (cross-domain) shape;
##### (3) developed a variational Bayesian framework to infer the posterior distributions of these explainable variables (shape, apperance, segmentation)

Prostate segmentation and cardiac segmentation tasks are applied for evaluation.

### Related Work

