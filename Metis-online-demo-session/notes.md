# Hierarchical clustering lit review

## Backlog

 - Find blogs
 - Review ISL
 - Review SKLearn docs & examples
 - Review my previous code w/ clustering
 - Review SciPy docs

## Prioritized backlog

 - Find my previous code w/ clustering
 - Review ISL
 - Review SciPy docs
 - Review SKLearn docs & examples
 - Review my previous code w/ clustering

## Notes

### My code

 - Can't find in Developer or on GH

### Review ISL

 - Downloading [book](http://www-bcf.usc.edu/~gareth/ISL/ISLR%20Seventh%20Printing.pdf)
 - Hierarchical and K-means are most common clustering
   - K means: K non-overlapping clusters, using iterative approach. Minimize distance (squared euclidean) between cluster members. Compute cluster centroid, assign observations to closest centroid. Repeat until assignments stop changing
   - Hierarchical clustering: Agglomerative clustering. Merge nearest points, height on y axis is distance from merge

Hierarchical clustering

 - Dendrogram introduciton
 - Issue w/ non-nested clusters (e.g. gender, nationality)
 - Algorithm:
   - Similarity metric: often Euclidean
   - Begin w/ n clusters for n observations
   - Fuse most similar clusters (using pairwise cluster comparison) until only 1 remains
 - Linkage: Dissimilairty between clusters
   - Complete: (Maximal). Largest pairwise distance between observations of the 2 clusters
   - Average: Average pairwise distance between observations of the 2 clusters
   - Single: (Minimal) Smallest pairwise distance between observations of the 2 clusters
   - Centroid: Compute centroid for each cluster, compaire centroids pair-wise
  - Linkage issues:
   - Single: Can lead to long, trailing clusters
   - Centroid: Inversion issue, two clusters can be fused below where clusters were created
   - Basically use Complete or average
 - Dissimilairty measures:
   - Correlation based: Comparing two observations
   - Consider scaling
 - Practical concerns w/ clustering
   - Standardization
   - Hyperparameters (dissimilarity measure, linkage, where to cut)
   - ValidationNo consensus (See Hastie et al. (2009))
   - Most clustering assumes mutually-exclusive groups
   - Robustness: Small pertubations / changes in data set cause big differences