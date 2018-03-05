# Hierarchical Clustering

## Intro

 - Why clustering
 - Example use case
 - Sample dendrogram

## Common use cases

 - Proxy for difficult to observe variables (e.g. gender)
 - User profiles / user journeys
 - Segmentation
 - Added feature
 - One model per cluster

## Algorithm

 - Algorithm
   - English description: Start with one cluster per observations. At every step, merge the two most similar. 
   - Algorithm outline

 - Visualization: Dendrogram
   - Plot w/ X (arbitrary) and y (change in distance metric)
   - Describe reading
   - Describe cutting

## Gotchas


 - Linkage
 - Distance metric
   - Normalization
   - SKLearn page
 - Data types
 - Metrics
   - Divisive subject
   - Cophenetic correlation
 - Where to cut

## Recap

### Resources

Hierarchical Clustering

 - Joern's blog post: https://joernhees.de/blog/2015/08/26/scipy-hierarchical-clustering-and-dendrogram-tutorial/
 - Introduction to Statistical Learning, section 10.3.2: http://www-bcf.usc.edu/~gareth/ISL/ISLR%20Seventh%20Printing.pdf
 - SciPy docs: https://docs.scipy.org/doc/scipy/reference/cluster.hierarchy.html
 - SKLearn user guide: http://scikit-learn.org/stable/modules/clustering.html#hierarchical-clustering
 - SKLearn docs: (http://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html#sklearn.cluster.AgglomerativeClustering

Ward linkage

 - Seminal paper: http://homes.mpimf-heidelberg.mpg.de/~mhelmsta/pdf/1963%20Ward%20JASA.pdf
 - Wikipedia: (https://en.wikipedia.org/wiki/Ward%27s_method
 - SciPy docs: https://docs.scipy.org/doc/scipy-0.14.0/reference/generated/scipy.cluster.hierarchy.linkage.html#scipy.cluster.hierarchy.linkage