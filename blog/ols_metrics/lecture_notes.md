# Meta

## Audience

 - Some software engineering experience
 - Recently exposed to OLS
 - Weaker stats background

## Goals

 - Familiarity w/ core nomeclature
   - SSE, t statistic, R2, adjsuted R2
 - Ability to recognize secondary nomeclature
   - p value
   - AIC
   - BIC

## Lit review

 - [DS curriculum slides](https://github.com/thisismetis/dscurriculum_beta/blob/master/class_lectures/week03-luther2/02-null_hypo_eval/Linear_Model_Evaluation.pdf)
 - [Robert's slides]() - None
 - [Zach's slides]() - None
 - Wooldridge: 37 - 40
 - [Statsmodels example](http://www.statsmodels.org/dev/examples/notebooks/generated/ols.html)

### [DS curriculum slides](https://github.com/thisismetis/dscurriculum_beta/blob/master/class_lectures/week03-luther2/02-null_hypo_eval/Linear_Model_Evaluation.pdf)

 - From Statsmodels point of view
 - Residuals DoF: observations - # free parameters
 - Model DoF: number of parameters - 1
 - R2: 1- (SSE/SST). Portion of unexplained variance
 - SSE: Sum squared errors
 - TSS: Sum squared totals
 - F statistic (skip)
 - T statistic and P value. P value for hyp test, h_0 is that B is actually zero. Want small p
 - Omnibus: Test that errors are normally distributed. Want small p
 - Examples for testing



# Outline