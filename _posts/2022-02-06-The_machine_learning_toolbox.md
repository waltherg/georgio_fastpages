---
title: The Machine Learning Toolbox
description: The open source landscape for data science and machine learning is pretty vast and ever-expanding. Here, I am trying to keep track of some of these packages.
permalink: /mltoolbox
toc: true
comments: true
layout: post
author: Georg Walther
categories: [machine learning, data science]
image: images/code_and_glasses.jpg
---

## Communities

### ML Collective

The ML Collective is a nonprofit organization that connects you with other machine learning practicioners.

[Link to ML Collective](https://mlcollective.org/)

### Kaggle

The primary supervised learning machine learning competition platform

[Link to Kaggle](https://www.kaggle.com/)

## Concepts

### Degenerate feedback loops

- Predictions influence feedback, where the feedback is used to extract labels (e.g. recommender systems that propose popular items based on how often they're clicked),
- Detect degenerate feedback loops using aggregate diversity or average coverage of long tail items,
- Introduce randomization into recommendations / predictions to gather more realistic feedback (downside user experience),
- Capture features of popularity (e.g. position in recommendation list) for prediction model,

#### Further reading

- [Write-up by Chip Huyen](https://docs.google.com/document/d/14uX2m9q7BUn_mgnM3h6if-s-r0MZrvDb-ZHNjgA1Uyo/edit?usp=sharing)

### Data distribution shift

For our machine learning model we call the inputs X and the outouts Y.
The training data in supervised learning is a sample of the (unknown) joint distribution P(X, Y).
In machine learning we usually model P(Y|X) - i.e. the conditional probability of the output given some observed input.

P(X, Y) = P(X|Y) P(Y) = P(Y|X) P(X)

- Covariate shift: P(X) changes while P(Y|X) is unchanged (distribution of the input changes but the distribution of the output given the input is unchanged)
- Label shift: P(Y) changes while P(X|Y) is unchanged
- Concept drift: P(Y|X) changes while P(X) is unchanged

#### Further reading

- [Write-up by Chip Huyen](https://docs.google.com/document/d/14uX2m9q7BUn_mgnM3h6if-s-r0MZrvDb-ZHNjgA1Uyo/edit?usp=sharing)

## Frameworks

### Pandas

Pandas is the primary data manipulation framework for data scientists in Python.
It entails and operates on two primary data models: Series, one-dimensional data / table columns, and dataframes, two-dimensional data akin to tables.

#### When (not) to use it

- Use when the data you're manipulating fit in memory

#### Further reading

- [Link to pandas documentation](https://pandas.pydata.org/)
- [Python for Data Analysis, 3rd edition](https://wesmckinney.com/book/)
