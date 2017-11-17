# GMDBSCAN-UR Grid based Multidensity DBSCAN Using Representative points.

Density Based Spatial Clustering of Applications of Noise (DBSCAN) is one of the most popular algorithms for cluster analysis. 

It can discover clusters with arbitrary shape and separate noises. But this algorithm cannot choose its parameter according to distribution of dataset. It simply uses the global minimum number of points (MinPts) parameter, so that the clustering result of multi -density database is inaccurate. In addition, when it used to cluster large databases, it will cost too much time. 

In this project we try to solve these problems by integrated the grid-based in addition to using representative points in our new proposed density-based GMDBSCAN-UR clustering algorithm. We propose a grid-based cluster technique to reduce the time complexity. 

Grid-based technique divides the data space into cells. A number of well scattered points in each cell in the grid are chosen. These scattered points must capture the shape and extent of the dataset as all. Thus, our project adopts a middle ground between the centroid-based and the all-point extremes. 

Next we treat all data in the same cell as an object, and all the operations of clustering are done on this cell. We make local clustering in each cell and merge between the resulted clusters. We use local MinPts for every cell in the grid to overcome the problem of undetermined clusters in multi-density datasets in clustering with DBSCAN clustering algorithm case. 

This will enhance the time complexity. Next step is labelling the not chosen points to the resulted clusters. 

Finally, we make post processing and noise elimination.
