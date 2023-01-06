---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---



Growth and Geometry Split in Light of DES-Y3 Survey
---------------------------------------------------
In the LCDM and models that only modifies the expansion history, the overdensity of matter evolves in the same way as the background, characterized by the growth function. The evolution equation of the growth function only depends on the matter density today in LCDM. However, that is not true in any modified gravity and dark energy clustering or coupled to dark matter model. We test this relation by introducing a meta parameter that doesn't enter into the geometry but the growth of the LCDM and wCDM model. We carefully chose the geometry prior such that the constraining power only comes from dark energy survey (DES) weak lensing and galaxy clustering data and found no inconsistency between growth and geometry.

The main results are as follows. For both DES-Y1 and DES-Y3 data, we find no inconsistency between geometry and growth.

<br/><img src='/images/gg_split/plot204_v2.png'>

However, we do find internal tension between some two-point correlation function combinations. The tension is accuired over the entire parameter space using normalizing flow. The result also depend highly on the prior.

<br/><img src='/images/gg_split/internal_tension_v4.png'>

The two priors we adopt in this work can be used in other large-scale structure analyses. The first prior that we call primary CMB consists of high-l TTTEEE until l=396 and low-l EE data. This prior is chosen such that it doesn't consist of late-time information about the universe. The truncation at the first peak of TTTEEE marginalizes the effect of CMB lensing, and the exclusion of low-l TT marginalizes the ISW effect. The second prior consists of BAO, SNIa, and BBN. It is a pure geometry (distance) prior, although it can not constrain inflationary physics such as primordial amplitude.


Marginalizing EDE Predictions over Late Expansion
-------------------------------------------------
The Early Dark Energy(EDE) is a promising solution to the current Hubble tension. The simplest model of EDE however is inconsistent with the current large-scale structure data. We marginalize the late time expansion rate and test with different data set to see if a late time modification can save the EDE model.

The most obvious problem of EDE as a solution to the hubble tension is that it harms the goodness of fit to the CMB. Here, we show that by a very general late-time DE evolution (a binned w model up to 10 bins), the two problems of H0 and LSS cannot be simutaneously solved.

<br/><img src='/images/early_late/FIGURE5.png'>

Emulator of the weak lensing data vector
----------------------------------------
The weak lensing and galaxy clustering pipeline are computationally very expensive. With OpenMP and MPI, the speed is largely increased. However, the next-generation analysis requires more accurate integral and systematic calculations. For example, in the growth-geometry project, we need to run about 100 chains for various priors and analysis settings. It took several months and a lot of computational resources. There are emerging ideas to use Neural Network to boost such calculations. The boost in speed is about a factor of 1000. The time to run a weak lensing chain on an AMD EPYC 7642 48-core node with four workers thus approximately drops from 1 month to 1 day.

The emulators in the current literature assume that they can only work inside the fiducial contour. However, it would require accuracy for the entire parameter space if we want to utilize such a method to real data, or calculate evidence ratio for example. We made a lot of progress on this as shown below. We improved the architecture. The sample points are also increased, but not very expensive to compute due to the efficiency of cocoa. We are adopting such a method in a follow-up analysis of growth-geometry split and also to the tension metric analysis that requires calculating thousands of noise realization chains. 

<br/><img src='/images/emulator/emulator_chi2_2.png'>

Micro-physics of Dark Energy: Anisotropic Stress and Sound Speed
----------------------------------------------------------------
In the fluid description of dark energy, the perturbation is usually turned off artificially due to gravitational instability. In Post-Friedmann(PPF) prescription, the problem was solved by a gauge transform and matching the dark energy perturbation to that of dark matter at the large scale. The anisotropic stress part of this description is often ignored, and in this study we use the latest large-scale structure data along with CMB anisotropy at large scale to constrain the shear term. We also studied another phenomenological model of anisotropic stress and scaler field model that introduce sound speed.

The modified version of Boltzmann code CAMB and CLASS can be found on my [GitHub](https://github.com/KunhaoZhong). Unfortunately they are currently with different Boltzmann code, in the near future, we plan to implement the sound speed into CAMB, as it can be easier to integrate into the weak lensing analysis pipeline. 

