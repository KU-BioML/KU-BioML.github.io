---
date: 2018-12-08
description: " "
featured_image: "/images/articles/3d_steerable_cnn.png"
tags: []
title: "3D Steerable CNNs: Learning Rotationally Equivariant Features in Volumetric Data"
disable_share: true
omit_header_text : true
---

_Advances in Neural Information Processing Systems 31 </br>(NeurIPS 2018)_

#### Maurice Weiler, Mario Geiger, Max Welling, Wouter Boomsma, Taco S. Cohen <!--more-->
</br>

#### Abstract:
We present a convolutional network that is equivariant to rigid body motions.
The model uses scalar-, vector-, and tensor fields over 3D Euclidean space to
represent data, and equivariant convolutions to map between such representations.
These SE(3)-equivariant convolutions utilize kernels which are parameterized
as a linear combination of a complete steerable kernel basis, which is derived
analytically in this paper. We prove that equivariant convolutions are the most
general equivariant linear maps between fields over R<sup>3</sup>. Our experimental results
confirm the effectiveness of 3D Steerable CNNs for the problem of amino acid
propensity prediction and protein structure classification, both of which have
inherent SE(3) symmetry.


[Click here for the full article](https://papers.nips.cc/paper/2018/file/488e4104520c6aab692863cc1dba45af-Paper.pdf)
