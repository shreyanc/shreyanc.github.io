---
published: true
comments: true
post_title: Can a Pop Music Feature Extractor Work for Classical Piano?
author: Shreyan Chowdhury
summary: Deep feature extractors for music - how do they perform on an unseen genre, and can domain adaptation help?  
logo: /assets/img/blog_imgs/2021-10-04-domain-adaptation/transfer.png
tags: research

type: blog
layout: blog
is_post: true
parent: /blog.html
title: ''
---

In learning from music content, hand-coded algorithms have been traditionally used as feature extractors. These algorithms extract features that capture information about various properties of sound, such as its tone colour (spectral descriptors), harmonic content, percussive elements and onsets, pitched content, noise, and several others. 

More recently though, deep neural networks have proven to be better extractors for some features that cannot be objectively defined, and the network learns these from annotated data. One such set of features is called Mid-level features, which I talk about in my previous blog post (TL;DR: these features lie in between objective, low-level sound attributes, and subjective, high-level musical concepts). In their 2018 paper, Aljanaki et al. introduced an annotated dataset of seven mid-level features.

<br>

## The Mid-level Features

The Midlevel Dataset consists of audio tracks and the collected values between 1 and 10 for the seven mid-level features -- _melodiousness, articulation, rhythmic complexity, rhythmic stability, dissonance, tonal stability,_ and _minorness_ (or _mode_), as shown below:

![](/assets/img/blog_imgs/2021-10-04-domain-adaptation/midlevel_dataset.png)

A deep neural network can be trained to predict these values given an audio clip as an input. Any sequential network architecture (VGG, ResNet, etc.) that takes spectrograms as inputs and gives seven continuous values as outputs could be trained to do this, and in my previous post, I give an example of such a network. This trained network can then be used get the mid-level features of a new audio clip. Why is this useful? Mid-level features have been shown to be useful for better prediction of music emotion and adds a layer of explainability -- it is easier to explain predictions when the explanations come in the form of human-understandable intuitive concepts. Mid-level features do exactly that. 

<br>

## The Problem of Out-of-Domain Transfer
Suppose, in your application, you want to predict emotions or generate explanations for a particular set of music. Say you want to build a classical music recommender, that responds to users' specific queries about how a piece of piano music has been performed. For this, you need a mid-level feature extractor. This extractor has been trained on the Mid-level dataset (as this is the only dataset available). We immediately notice a problem in this scenario.
Below, you can see the distribution of genres in the Midlevel Dataset<sup>1</sup>. 

![](/assets/img/blog_imgs/2021-10-04-domain-adaptation/midlevel_genres.png)

The Midlevel Dataset contains mostly pop and electronic songs. Even among songs classified as "classical", there are few that are solo piano. We thus find that the kind of data we are interested in is not reflected adequately in the training set. This results in what is known as covariate shift between the training and test data, which makes direct transfer of a feature extractor less reliable.

<br>

## Dealing with Covariate Shift

Machine learning literature is replete with numerous techniques to deal with different kinds of dataset shifts. In our case, we look at the following observations to choose a technique:

1. We have very few target domain samples.
2. It is possible to obtain a large collection of unlabeled solo piano recordings.

This looks like a job for -- Unsupervised Domain Adaptation! The idea is to somehow use a large number of unlabelled audio from the target domain to train a model that works well on that target domain.  

First we do a baseline test. We construct a test set out of the few solo piano samples that we do have in the Midlevel Dataset. We train a VGG-like model on the remaining data and test the resulting model on the test data. We see a big drop in performance (the performance metric being average Pearson correlation coefficient between each predicted and true mid-level feature value).

Instead of a VGG-like model, can we use a model architecture that is regularised (and hence might have better _generalizability_)? Koutini et al. showed that receptive field regularization (reducing kernel size of convolutional layers and reducing model complexity) is a plausible way to generalize audio models.




