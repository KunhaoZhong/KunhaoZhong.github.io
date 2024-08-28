---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---
For the full list of publications, see [arxiv](https://arxiv.org/search/astro-ph?searchtype=author&query=Zhong,+K), [Inspire](https://inspirehep.net/authors/2622565?ui-citation-summary=true),or [ADS](https://ui.adsabs.harvard.edu/search/q=%3Dauthor%3A%22Zhong%2C%20Kunhao%22&sort=date%20desc%2C%20bibcode%20desc&p_=0)
----------------------------------------



Simulation-Based Inferenec with Convolutional Neural Networks [2403.01368](https://arxiv.org/abs/2403.01368)
----------------------------------------
Simulation-Based Inference (SBI), also known as Likelihood-Free Inference, is a novel approach within the Bayesian framework designed to determine the posterior distribution when the likelihood function is intractable. This technique proves invaluable in scenarios where direct simulation of the physical process is possible. It has seen considerable application in understanding neural behavior and holds significant promise in cosmology, especially in extracting non-Gaussian information critical to unraveling the universe's history and the nature of dark energy and dark matter.

Convolutional Neural Networks (CNNs), traditionally employed in image classification tasks, such as with ResNet designs, offer a powerful means for data compression in SBI at the field level. **However, cosmological data differs markedly from typical machine learning or computer vision images**, characterized by stochastic properties and a low signal-to-noise ratio. In this work, we introduce a novel regularization and data augmentation strategy that significantly enhances CNN performance. By shuffling feature maps, we disrupt large-scale correlations, mitigating overfitting and co-adaptation more effectively than traditional methods like dropout. While this approach is not a one-size-fits-all solution, its potential for broader application, including in galaxy maps or 21cm maps, is promising.

<br/><img src='/images/cnn/cnn_design_v2.png' width="650">

Emulator of the weak lensing data vector [2402.17716](https://arxiv.org/abs/2402.17716) [2403.12337](https://arxiv.org/abs/2403.12337)
----------------------------------------
The computation involved in weak lensing and galaxy clustering analyses is notoriously demanding. Despite improvements from OpenMP and MPI, the precision and systemic calculation requirements of next-generation analyses, such as those in the growth-geometry project, are immense. Typically, running about 100 chains for varied priors and analysis settings could take several months and consume vast computational resources.

Recent advancements propose using Neural Networks to accelerate these calculations, achieving speed increases by approximately 3000 times. Consequently, processing a weak lensing chain on an AMD EPYC 7642 48-core node with four workers is reduced from roughly a month to less than a day.

Traditional emulators are presumed to function within the fiducial contour alone, limiting their utility for real-data application or comprehensive parameter space analysis. Our work makes significant strides by incorporating Transformers and Self-attention mechanisms, **enabling theoretical optimality in emulator accuracy across the entire prior space**. This breakthrough allows for previously unfeasible comparisons and applications, leveraging the neural network's speed.

In the first two of a serers of investigations of emulator approach, we forcast the constraining power of growth-geometry split  formalism in LSST Year 1 data, and the calibration of different tension metric with intensive noise injection. Both of these work shows the great potential of an emulator that is highly accurate within a wide parameter space.

<br/><img src='/images/emulator/validation_lcdm_LSST_CS_2M_combined.png'  width="450">

Growth and Geometry Split in Light of DES-Y3 Survey [2301.03694](https://arxiv.org/abs/2301.03694)
---------------------------------------------------
In the LCDM and models that only modifies the expansion history, the overdensity of matter evolves in the same way as the background, characterized by the growth function. The evolution equation of the growth function only depends on the matter density today in LCDM. However, that is not true in any modified gravity and dark energy clustering or coupled to dark matter model. We test this relation by introducing a meta parameter that doesn't enter into the geometry but the growth of the LCDM and wCDM model. We carefully chose the geometry prior such that the constraining power only comes from dark energy survey (DES) weak lensing and galaxy clustering data and found no inconsistency between growth and geometry.

The main results are as follows. **For both DES-Y1 and DES-Y3 data, we find no inconsistency between geometry and growth**. The set of choicec in our work makes the treatement of non-linearities clear as compared to other work. We will extend the work to future DES-Y6 and LSST-Y1 data.

<br/><img src='/images/gg_split/plot204_v2.png'  width="550">


Marginalizing EDE Predictions over Late Expansion [2302.07333](https://arxiv.org/abs/2302.07333)
-------------------------------------------------
The Early Dark Energy(EDE) is a promising solution to the current Hubble tension. The simplest model of EDE however is inconsistent with the current large-scale structure data. We marginalize the late time expansion rate and test with different data set to see if a late time modification can save the EDE model.

The most obvious problem of EDE as a solution to the hubble tension is that it harms the goodness of fit to the CMB. Here, we show that by a very general late-time DE evolution (a binned w model up to 10 bins), the two problems of H0 and LSS cannot be simutaneously solved.


Micro-physics of Dark Energy: Anisotropic Stress and Sound Speed [2408.14628](https://arxiv.org/abs/2408.14628)
----------------------------------------------------------------
In the fluid description of dark energy, the perturbation is usually turned off artificially due to gravitational instability. In Post-Friedmann(PPF) prescription, the problem was solved by a gauge transform and matching the dark energy perturbation to that of dark matter at the large scale. The anisotropic stress part of this description is often ignored, and in this study we use the latest large-scale structure data along with CMB anisotropy at large scale to constrain the shear term. We also studied another phenomenological model of anisotropic stress and scaler field model that introduce sound speed.

The modified version of Boltzmann code CAMB and CLASS can be found on my [GitHub](https://github.com/KunhaoZhong). Unfortunately they are currently with different Boltzmann code, in the near future, we plan to implement the sound speed into CAMB, as it can be easier to integrate into the weak lensing analysis pipeline. 

