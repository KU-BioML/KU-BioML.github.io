---
date: 2017-12-09
description: " "
featured_image: "/images/articles/spherical_convs.png"
tags: []
title: "Spherical convolutions and their application in molecular modelling"
disable_share: true
omit_header_text : true
---

_Advances in Neural Information Processing Systems 30</br>(NIPS 2017)_

#### Wouter Boomsma, Jes Frellsen <!--more-->
</br>

#### Abstract:
Convolutional neural networks are increasingly used outside the domain of image
analysis, in particular in various areas of the natural sciences concerned with
spatial data. Such networks often work out-of-the box, and in some cases entire
model architectures from image analysis can be carried over to other problem
domains almost unaltered. Unfortunately, this convenience does not trivially
extend to data in non-euclidean spaces, such as spherical data. In this paper, we
introduce two strategies for conducting convolutions on the sphere, using either
a spherical-polar grid or a grid based on the cubed-sphere representation. We
investigate the challenges that arise in this setting, and extend our discussion to
include scenarios of spherical volumes, with several strategies for parameterizing
the radial dimension. As a proof of concept, we conclude with an assessment of the
performance of spherical convolutions in the context of molecular modelling, by
considering structural environments within proteins. We show that the models are
capable of learning non-trivial functions in these molecular environments, and that
our spherical convolutions generally outperform standard 3D convolutions in this
setting. In particular, despite the lack of any domain specific feature-engineering,
we demonstrate performance comparable to state-of-the-art methods in the field,
which build on decades of domain-specific knowledge.


[Click here for the full article](https://papers.nips.cc/paper/2017/file/1113d7a76ffceca1bb350bfe145467c6-Paper.pdf)
