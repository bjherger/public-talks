# Meta

## Audience

 - Might be familiar w/ deep learning
 - Are familiar w/ OLS, logistic
 - May not be familiar w/ loss functions directly

## Goals

 - Good default losses and optimizers for common data types
 - Ability to discuss real valued losses
 - List of formulas for common losses
 - Links for further reading for common losses and optimizers 

## Lit review

### Backlog

 - Deep Learning book
   - 3.13: Information theory
 - [keras losses](https://keras.io/losses/)
 - [keras optimizers](https://keras.io/optimizers/)
 - [ML cheatsheet losses](https://ml-cheatsheet.readthedocs.io/en/latest/loss_functions.html)
 - [ML cheatsheet optimizers](https://ml-cheatsheet.readthedocs.io/en/latest/optimizers.html)
 - [Adam paper](https://arxiv.org/pdf/1412.6980.pdf)
 - [keras issue](https://github.com/keras-team/keras/issues/6444)
 
#### DL Book

3.13: Information theory

 - Self information: I(x) = -log(P(x)) 
 - Shannon entropy: H(x) = E(I(x))
   - Expected amount of info in a single event, drawn from distribution
   - AKA Differential entropy for continuous variables
 - KL divergence: E(log(p(x)/q(x))) for x~p
 

5.5.1: Conditional log likelihood (141)

 - KL divergence for models: KL(pdata || pmodel)
   - Removing constants: -E(log(pmodel(x))), for x ~ pdata


### Prioritized backlog

 - Deep Learning book
 
## Outline

### Losses

#### Need to have

 - MSE
 - MAE
 - MAPE
 - Categorical cross-entropy

#### Nice to have

 - Hinge
 - KL divergence

### Optimizers

#### Need to have

 - SGD
 - Adam
 - RMSprop
 
#### Nice to have 

### Defaults

 - Numerical output
 - Categorical output
 - Text input
 


