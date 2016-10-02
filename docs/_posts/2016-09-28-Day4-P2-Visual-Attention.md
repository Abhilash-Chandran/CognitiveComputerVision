---
title:  "Computational Visual Attention(Day4 - II)"
subtitle: "Itti-Koch,"
author: "Abhilash"
avatar: "img/authors/Abhi.png"
image: "img/day4/day4.jpg"
date:   2016-09-29
---

In the previous part we saw some psychological models for visual attention like, Feature Integration Theory, Guided Search Model. In this part we will look into the details of _Computation Visual Attention_ models.

We need such computational models in order to enable the robots with autonomous navigation capability and enhance their decision making skills by perceiving the environment rather more accurately and quickly.

Some Reasons:

* Attention prioritization
* Quicker attention leads to quicker decisions
* Shared attention(swarm robotics - reduced overall computation)

# Attention Vs Saliency
---
Imagine you are entering your friends home. The first thing you do after entering would be naturally look around to locate objects like table, couches, television,  indoor plants, Idols etc. This is comparable to the saliency detection in computer vision. If you are a carpenter by profession you might be more interested in looking at the table design if it attracts your attention.

Likewise in a computer vision problem, given a stream images Saliency computation corresponds to the bottom-up approach of detecting salient objects which then attracts the robots attention for further processing e.g. object detection, segmentation, etc.

Applications of Saliency computation.

- Automatic cropping of images.
- Preprocessing of images for object discovery.

## Psychological Visual Attention Models(Revisit)

1. Feature Integration Theory
2. Koch-Ullman Model
  * Parallel, independent feature extraction. Compose a final map of activity.
3. Guided Search Model
  * Top-down cue based feature extraction.

# Itti-Koch model(_iNVT_)
---

![IttiKoch](img/day4/IttiKoch.png)

Itti, Koch and Niebur(1998) came up with computational model for visual attention based on the structure of Koch-Ullman model. The core steps of this _computational visual attention_ model are,

1. Separate Feature map channels
2. Image pyramid representation for each feature channel
3. Center Surround Contrast
4. Fusion of the channels
5. Maximum finder
6. Inhibition of Return(IOR)
7. Top down control information

One of the main element is the center surround contrast element which acts as the crux of a salience systems.

# The VOCUS System
---

<em>__V__</em>isual <em>__O__</em>bject Detection with a <em>__C__</em>omp<em>__U__</em>tational attention <em>__S__</em>ystem
