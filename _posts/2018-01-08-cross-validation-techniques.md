---
layout: post
title: Cross validation techniques
subtitle: Differences | Takeaway
image: /img/firstPost.jpeg
tags: [data science, machine learning]
comments: true
---

For instance consider the data set with 100 objects to train.

**Random subsampling**: Randomly split shuffled 100 objects into train set and test set. It can be 80–20, 70–30, 60–40. This is also called as **Hold-out**.

Good for huge data. If you are getting similar scores and optimal model’s parameters with some of your iterations.

**K-fold**: Split the shuffled 100 objects into k chunks of data. Train with (k - 1) chunks of data objects, test it on (k - 1)th chunk. Next time, include the one that you excluded in the last iteration to train your model and test it on this excluded chunk. Repeat. This should take you K iterations. This is *K times slower to random subsampling*.

Good for huge data. If you are not getting similar scores and different optimal model’s parameters when you iterate.

One can be a victim of skewed target values with Random subsampling and K-fold which can be fixed by **stratification**. Stratification makes sure that you get similar target distribution in each of your folds (chunks) of your data.

**Leave-one-out**: Special case of K-fold. K = 100 (in our example). Train your model with 99 objects, test it on 100th object. Repeat this with leaving out one object each time. This should take you 100 iterations. In our example this is *100 times slower than random subsampling*. This is also called as **JackKnife resampling**. 

Good for less data and unbalanced dataset and target values.
