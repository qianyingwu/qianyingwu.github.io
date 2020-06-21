---
title: 'Playing with water splat at home'
date: 2020-06-19
excerpt: "At-home experiments on the asymmetry of water drop impacted on an inclined solid surface   <br/><img src='/images/watersplat/01.png'>"
permalink: /posts/2020/06/watersplat/
tags:
  - quarantine
  - fun project
  - experiment
---

This project is part of ME354 class taught by Professor Juan Santiago's class on Experimental Methods in Fluids Dynamics. Many thanks to the teaching team!

# Asymmetry of Water Drop Impacted on an Inclined Solid Surface

Splats are ubiquitous in the real world, for example rain drops on the cement ground. Have you taken a closer look at their shape, especially when they are impacted on inclined surfaces? You may imagine that the splat is not round anymore. I did a small project in the backyard and practiced some image processing techniques I learned in class. It turned out to be quite fun too!

![photo1](/images/watersplat/01.png)


## Set up

I built this poor man's set up - a camera was made parallel to the paper on which the drop will land, and a folding screen was meant to set the scaleplate of the height of the drop. Without a pipette at hand, I disassembled a small nozzle from a water flosser and used it as a dispenser of the drop.
An outdoor environment was chosen for better lighting, but the change in sunlight illumination in the morning and the afternoon turned out to raise complications in image processing, especially with thresholding and binarizations algorithms.

![photo1](/images/watersplat/02.png)

## Data processing

### Varying Drop Heights and Surface Inclined Angles w/ Multiple Realizations
The surface inclination is believed to be the cause of splat asymmetry, while the drop height relates to the momentum when the drop impacts the surface which also influences the asymmetry of the splat.

![photo1](/images/watersplat/03.png)

### Morphological Processing to Extract the Shape of the Drop Followed by Statistical Analysis in X and Y Directions

![photo1](/images/watersplat/04.png)
Note: (1) getting pdf w/o threshold binarization did not work well, because of the large glare presented at the center of some images (2) morphological processes are different for morning/afternoon lighting conditions

## Analysis of asymmetry

### Centroid Shifted in the Y direction > X direction
$Y centroid shift ratio =\frac{Y_{\text {shift }}}{D_{\text {eff}}}$

where

$D_{eff}=\sqrt{\frac{4 A r e a}{\pi}}$

$Y_{\text {shift}}=Y_{\text {centroid}}-Y_{\text {midpoint}}$

$Y_{\text {midpoint}}=\frac{1}{2}\left(Y_{5 \%}+Y_{95 \%}\right)$

![photo1](/images/watersplat/05.png)

### Height/Width Ratio Monotonically Increases with Larger Surface Inclined Angle

![photo1](/images/watersplat/06.png)
Note: Large surface inclined angles also result in larger variations between realizations.




