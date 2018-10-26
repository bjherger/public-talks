# keras-pandas: A new package to democratize Deep Learning

 - https://us.pycon.org/2019
 - https://us.pycon.org/2019/proposals/submit/talk/
 
## Title

keras-pandas: A new package to democratize Deep Learning

## Duration

30 minutes

## Description

During this talk, we'll dive into [keras-pandas](https://keras-pandas.readthedocs.io/en/latest/)'s design, a case study
using common tabular data formats, and best in class approaches for for handling numerical, categorical, text, and timeseries data with deep learning.

 - For those new to deep learning, it drastically lowers the barrier to entry by automating the plumbing, and providing 
 cutting edge defaults without having to do a literature review
 - For those familiar with deep learning, it reduces the time to prod from hours to minutes by automating replacing 
 variable input and output setup

Deep learning provides amazing opportunities to build highly predictive models. However, historically this modeling has 
required deep domain experience, and keeping up with a massive body of literature. Further, applying these approaches 
to tabular data has been a highly-specialized field. 

My recently open sourced package, keras-pandas, allows users to rapidly prototype and deploy models by providing 
state-of-the art defaults and heuristics, based on the techniques used in Fortune 100 companies and by kaggle 
grandmasters. 


## Who and Why (Audience)

Novices:

 - For those new to deep learning, keras-pandas drastically lowers the barrier to entry by automating the plumbing, and providing 
 cutting edge defaults without having to do a literature review
 - Assumes the audience is familiar with python and tabular data (e.g. in Excel or pandas)
 - Does not assume the audience is familiar with machine learning, though familiarity with SKLearn helps
 
Experts:
 - For those familiar with deep learning, it reduces the time to prod from hours to minutes by automating replacing 
 variable input and output setup
 - Assumes the audience is familiar with building deep learning models (e.g. in keras or pytorch)

## Outline

 - Oppportunity / existing frustrations
   - DL examples commonly only include images, text and audio
   - Getting common tabular data formats into deep learning models is needlessly difficult
 - Intro to package
 - Demo
   - Example building a deep learning model in a few minutes on the Lending Club data set
 - Transformation pipeline & deep learning layers for common data types
  - Numerical, categorical, others as time allows
 - Recap & Getting started
   - What we've covered, how to get started using this package

## Additional notes

 - I've been fortunate enough to present my work at  Strata & Hadoop World, PyData, Data Day Texas, Big Data Day LA, 
 the Sentiment Analysis Symposium and IDEAS
 - I cofounded the Deep Learning center of excellence at a fortune 100 company, and have put deep learning projects 
 into production there
 - I'm the primary author of keras-pandas
 - This talk contains a code demo, which can be done live or pre-recorded (as a backup)