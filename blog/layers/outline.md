# Part 0: Intro

## What is a layer?

 - Difference between DL book and Keras Layers
 - What properties do all layers have?
 - What changes between layer types

## 1D vs 2D

 - 1D: Temporal (time series, text)
 - 2d: Spatial (image)

## Cheat sheet

# Part 1: Standard layers

## Input

 - Simple pass through
 - Needs to align w/ shape of upcoming layers

## Embedding

 - Categorical / text to vector
 - Vector can be used with other (linear) algorithms
 - Can use transfer learning / pre-trained embeddings(see [example](https://blog.keras.io/using-pre-trained-word-embeddings-in-a-keras-model.html))

## Dense layers

 - Vanilla, default layer
 - Many different activations
 - Probably want to use ReLu activation

## Dropout

 - Helpful for regularization
 - Generally should not be used after input layer
 - Can select fraction of weights (`p`) to be dropped
 - Weights are scaled at train / test time, so average weight is the same for both
 - Weights are not dropped at test time

# Part 2: Specialized layers

## Convolutional layers

 - Take a subset of input
 - Create a linear combination of the elements in that subset
 - Replace subset (multiple values) with the linear combination (single value)
 - Weights for linear combination are learned

## Time series & text layers

 - Helpful when input has a specific order 
   - Time series (e.g. stock closing prices for 1 week)
   - Text (e.g. words on a page, given in a certain order)
 - Text data is generally preceeded by an embedding layer
 - Generally should be paired w/ `RMSprop` optimizer

### Simple RNN

 - Each time step is concatenated with the last time step's output
 - This concatenated input is fed into a dense layer equivalent
 - The output of the dense layer equivalent is this time step's output
 - Generally, only the output from the last time step is used
 - Specially handling for the first time step

### LSTM

 - Improvement on Simple RNN, with internal 'memory state'
 - Avoid issue of exploding / vanishing gradients

## Utility layers