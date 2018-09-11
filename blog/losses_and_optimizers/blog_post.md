# [Cheat sheet: Deep learning losses & optimizers](https://www.hergertarian.com/cheat-sheet-deep-learning-losses-optimizers)

**tl;dr:** Sane defaults for deep learning loss functions and optimizers, followed by in-depth descriptions. 

## Intro

Deep Learning is a radical paradigm shift for most Data Scientists, and a still an area of active research. 
Particularly troubling is the high barrier to entry for new users, usually centered on understanding and choosing 
loss functions and optimizers. Let's dive in, and look at industry-default losses and optimizers, and get an in-depth
look at our options. 

Before we get too far, a few definitions:

 - **Loss function:** This function gives a distance between our model's predictions to the ground truth labels.
 This is the distance (loss value) that our network aims to minimize; the lower this value, the better 
 our current model describes our training data set
 - **Optimizer:** There are many, many different weights our model could learn, and brute-force testing every one would 
 take forever. Instead, we choose an optimizer which evaluates our loss value, and smartly updates our weights. 

This post builds on my [keras-pandas](https://keras-pandas.readthedocs.io/en/latest/intro.html), which lowers the 
barrier to entry for deep learning newbies, and allows more advanced users to iterate more rapidly. These defaults 
are all built into keras-pandas.  

## Defaults

If you're solely interested in building a model, look no further; you can pull the defaults from the table below:

![](/s/defaults.jpg)

## What's goin' on?

Let's dive a bit deeper, and have a look at what our options are

### Notation

Before we go on, let's define our notation. This notation is different than many other resources (such as Goodfellow's 
[The Deep Learning Book](https://www.deeplearningbook.org/), and 
[theano's documentation](http://deeplearning.net/software/theano/library/tensor/nnet/nnet.html#theano.tensor.nnet.nnet.categorical_crossentropy)), 
however it allows for a succinct and internally consistent discussion. 

![](/s/notation.jpg)

### Losses

Losses are relatively straight forward for numerical variables, and a lot more interesting for categorical variables. 

![](/s/losses.jpg)

### Optimizers

Finally, the world of optimizers is still under active development (and more of an art than a science). However, a few
industry defaults have emerged.

![](/s/optimizers.jpg)
 