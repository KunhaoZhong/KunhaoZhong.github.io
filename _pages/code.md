---
layout: archive
title: "Code"
permalink: /code/
author_profile: true
redirect_from:
  - /codes
---

{% include base_path %}

I have two Boltzman code in studying micro-physics of Dark Energy, jupyter notebook and scripts for presenting galaxy week lensing and clustering results, and notes on k-essence. All publicly available on my [GitHub](https://github.com/KunhaoZhong).

[CAMB-AS](https://github.com/KunhaoZhong/CAMB-AS)
-------------------------------------------------

The full PPF equation from [0801.2433](https://arxiv.org/abs/0801.2433) is implemented with special numerical stability. Yaml files are provided to reproduce the figures from the paper. There're also two models using fluid description implemented from (1402.5993)[https://arxiv.org/abs/1402.5993]. The code is with latest version of CAMB and is compatibale with Cobaya and Cocoa. The code is insipred by Wayne Hu's public code and also Vivian Miranda's private code, who is the author of Cocoa. Although the difference betweem Newtonian potential and Weyl potential is small in the range that DES can probe, we should in principal treat them differently in 2 point correlation function. The modified version of Cosmolike is available [here](https://github.com/SBU-UNESP-2022-COCOA/cocoa2/tree/astress).


[CLASS_GSF](https://github.com/KunhaoZhong/CLASS_GSF)
-----------------------------------------------------
The modified version of CLASS that calculate generalized scalar field model. The code is similar to [Hi-Class](http://miguelzuma.github.io/hi_class_public/) in design, but use the full perturbation equation in stead EFT. An improved method of shooting algorithm for finding the initial condition is also included. Three example k-essence model are implemented, with yaml file to produce background evolution. The code is compatible to do any non-coupled dark energy model, such as DBI.
