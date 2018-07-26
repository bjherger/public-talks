# [Cheat Sheet: Linear Regression Model Evaluation](https://www.hergertarian.com/cheat-sheet-linear-regression-model-evaluation)

**tl;dr:** Cheat sheet for linear regression metrics, and common approaches to improving metrics 

![Rexthor](/s/linear_regression_2x.png)

*One of the many reasons we care about model evaluation. Image courtesy the fantastic [XKCD](https://xkcd.com/1725/)*

## Intro

I'll cut to the chase; linear regression is very well studied, and there are many, many metrics and model statistics
to keep track of. Frustratingly, I've never found a convenient reference sheet for these metrics. So, I wrote a cheat 
sheet, and have iterated on it with considerable community input, as part of my role teaching data science to companies 
and individuals at Metis. 

I'll also highlight that most of my work has been in leading [Deep Learning](https://www.hergertarian.com/detecting-toxic-comments-with-multitask-deep-learning)
 and [fraud](https://www.youtube.com/watch?v=u72FD79tsxA), which have rarely involved linear models; I am, by no means,
 a domain expert. I've used this point of view to help write this reference for a general audience.  

## Cheat sheet

Below are the most common and most fundamental metrics for linear regression (OLS) models. This list is a work in 
progress, so feel free to reach out with any corrections, or stronger descriptions. 

![Cheat sheet](/s/cheat_sheet.jpg)

### Correcting issues

The natural next question is "What happens when your metrics aren't where you'd like them to be?" Well, hen, the hunt 
is afoot!

While model building is more of an art than a science, below are a few helpful (priority ordered) approaches to 
improving models. 

 - Trying another algorithm
 - Using regularization (lasso, ridge or elasticnet)
 - Changing functional forms for each feature (e.g. log scale, inverse scale)
 - Adding polynomial terms
 - Including other features
 - Using more data (bigger training set)
