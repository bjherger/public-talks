# Hierarchical clustering lit review

## Planning

### Backlog

 - Find blogs
 - Review ISL
 - Review SKLearn docs & examples
 - Review my previous code w/ clustering
 - Review SciPy docs
 - Review Ward linkage

### Prioritized backlog

 - Find my previous code w/ clustering
 - Review ISL
 - Review SciPy docs
 - Review SKLearn docs & examples
 - Review Ward linkage

### Done

 - Find my previous code w/ clustering
 - Review ISL
 - Review SciPy docs
 - Review SKLearn docs & examples
 - Review Ward linkage

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
   - Centroid: Compute centroid for each cluster, compare centroids pair-wise
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

### Review SciPy docs

 - Reviewing [example blog post](https://joernhees.de/blog/2015/08/26/scipy-hierarchical-clustering-and-dendrogram-tutorial/)
   - Linkage transforms matrix to Z matrix w/ cluster linkage array (contains the hierarchical clustering information). Schema: `[idx1, idx2, dist, sample_count]`.
   - Metrics: [Cophenetic correlation](https://en.wikipedia.org/wiki/Cophenetic_correlation), compares pairwise distances and and 'those implied by the cluster'
   - Creating dendrogram
 - Reviewing [docs](https://docs.scipy.org/doc/scipy/reference/cluster.hierarchy.html)
   - Param, optimal ordering: Re-ordering observations in Z, better for viz. Computationally expensive
   - Can have reproducibility issues. If same distance, choice of merge is arbitrary

### Review SKLearn docs & examples

 - Reviewing [user guide](http://scikit-learn.org/stable/modules/clustering.html#hierarchical-clustering)
   - Ward linkage: Sum squared differences within all clusters. Similar to K means
   - Scaling: Can scale w/ connectivity matrix, expensive w/o connectivity restrains (many pair-wise comparisons)
   - FeatureAgglomeration: Feature reduction, using hierarchical clustering
 - Reviewing [docs](http://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html#sklearn.cluster.AgglomerativeClustering)
   - Param, connectivity: Restrain which observations are compared to each other. Pre-clustering, sometimes w/ KNN
   - Param, linkage: One of `{'ward', 'complete', 'average'}`
   - Param, pooling_function: Combines features to single value for comparison

### Review Ward linkage

 - Reading [scipy docs for ward](https://docs.scipy.org/doc/scipy-0.14.0/reference/generated/scipy.cluster.hierarchy.ward.html)
 - Reading [scipy docs for linkage](https://docs.scipy.org/doc/scipy-0.14.0/reference/generated/scipy.cluster.hierarchy.linkage.html#scipy.cluster.hierarchy.linkage)
   - Provides formula, little description
 - [Wikipedia article](https://en.wikipedia.org/wiki/Ward%27s_method)
  - At each step, merge the two clusters which produce the smallest increase of within-cluster variance. Within cluster variance is weighted squared distance between cluster centers
 - [Hierarchical Grouping to Optimize an Objective Function](http://homes.mpimf-heidelberg.mpg.de/~mhelmsta/pdf/1963%20Ward%20JASA.pdf), seminal paper
   - For each candidate grouping:
     - ESS: \sum_{i} x^2 - mean(x_i)^2, where i is the set of observations
     - Compute ESS for each group
     - Sum ESS for all groups
   - Use candidate grouping w/ smallest sum ESS
   

