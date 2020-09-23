---
published: true
layout: post
author: Shreyan Chowdhury
authors: 'Mason Bretan, Larry Heck'
summary: >-
  Representation learning of symbolic music using adjacency as a
  self-supervising signal
logo: /assets/img/apad_bretan_semantic.png
link: 'http://archives.ismir.net/ismir2019/paper/000053.pdf'
is_post: true
parent: /apad.html
title: ''
post_title: Learning Semantic Similarity in Music via Self-Supervision
logo_desc: >-
  The two architectures - a) A-DSSM (Adversarial Deep Structured Semantic Model)
  and b) A-AdjD
---
## Upshot
- The authors propose two related methods for learning symbolic music embeddings such that semantically similar inputs lie closer together in the latent space than dissimilar ones.
- This is achieved by defining **adjacent sections of a musical input to be semantically similar** and constraining the embeddings to come from a **Gaussian prior distribution**.
- The prior distribution is enforced by connecting adversarial discriminator networks to the last layer of the feature extractors. 

## Wisdom
- The **ratio of easy to hard examples** is often biased towards the easy end. This produces poor performance since many examples can satisfy the constraint with a very small loss that provides no meaningful update during backpropagation. The **adversarial component naturally helps to mitigate this problem by enforcing the prior distribution**.
- Using small networks for adjacency discrimination (for A-AdjD model) forces the embedding portion to learn good features to differentiate between related and non-related inputs.
- Fitting the latent space to a prior distribution prevents the model from satisfying the similarity contraint without actually learning too many meaningful features.

## Details
-