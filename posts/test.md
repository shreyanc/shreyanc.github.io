---
layout: post
published: true
author: Shreyan
---
## Towards Explainable Music Emotion Recognition: The Route via Mid-level Features - 1

<ul class="downloads">
  <li><a href="https://arxiv.org/abs/1907.03572"><strong>Paper</strong></a></li>
  <li><a href="#"><strong>Poster</strong></a></li>
  <li><a href="https://shreyanc.github.io/ismir_example.html"><strong>Demo</strong></a></li>
 </ul>

Emotional aspects play an important part in our interaction with music. However, modelling these aspects in MIR systems have been notoriously challenging since emotion is an inherently abstract and subjective experience, thus making it difficult to quantify or predict in the first place, and to make sense of the predictions in the next. In an attempt to create a model that can give a musically meaningful and intuitive explanation for its predictions, we propose a VGG-style deep neural network that learns to predict emotional characteristics of a musical piece together with (and based on) human-interpretable, mid-level perceptual features. We compare this to predicting emotion directly with an identical network that does not take into account the mid-level features and observe that the loss in predictive performance of going through the mid-level features is surprisingly low, on average. The design of our network allows us to visualize the effects of perceptual features on individual emotion predictions, and we argue that the small loss in performance in going through the mid-level features is justified by the gain in explainability of the predictions.
