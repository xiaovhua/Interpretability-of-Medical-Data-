# Domain Shift

Domain shift (DS) means the distributions of source domain (e.g. training data) and target domain (e.g. test data or real world data) are different. It is very common in medical problems, various sequences, modalities and sites will lead to DS, and potential factors such as scanners, field-of view, spatial resolution, signal-to-noise ratio, and digital processing software will also result in such distribution gaps.

![DomainShift](https://github.com/xiaovhua/Interpretability-of-Medical-Data-/blob/main/png/DomainShift.gif)

Depending on whether the data from target domain is available, the techniques for addressing DS can be divided into domain adaptation and domain generalization.

# Domain Adaptation
Domain adaptation (DA) aims to address the DS problems where target domain data is available.

# Domain Generalization
Domain generalization (DG) is to address the DS problems where target domain data is not available. To generalize into unseen domain, data-based, learning-based, and representation-based methods can be applied to enrich model representation.
#### Data-based Method
The data-based methods try to enrich the diversity of training data by data augmentation or data generalization. These methods are effective for small distribution shifts but can be **_vulnerable to significant domain gaps_**. 
#### Learning-based Method
The learning-based methods aim to combine knowledge from training domains by specific strategies, including ensemble learning and meta-learning. These methods have achieved promising performance on specific target domain, but limiting the number of source domains could weaken their generalization ability.

# Reference:
Gao S, Zhou H, Gao Y, et al. BayeSeg: Bayesian Modeling for Medical Image Segmentation with Interpretable Generalizability. Medical Image Analysis, 2023.


