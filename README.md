# music-mood-classification

## Data Cleaning

### muse_v3.csv
original dataset

### data_cleaning.ipynb
Jupyter notebook containing the code to remove null data points and pull audio features from the API.
also contains code for PCA

### pca_80.csv
list of features give by the 8 PCA components (~80% variance retained)

### pca_3.csv
list of features give by the 3 PCA components

### pca_components.csv
breakdown of PCA components into original features

### cleaned.csv 
contains song titles and spotify IDs w/ null values removed

### audio_feat.csv 
contains the pulled audio features for each song

### full_data.csv 
contains the full data with song titles, artists, and audio features

### single_tags.csv
contains full data with only 1 tag per song

### relevant_features_single_tags.csv
contains fully cleaned data that removes irrelevant features (song title, artist, etc) and only has 1 tag per song

### tags.csv
list of different tags present in the dataset alongside their number of occurrences

## K-Means

### K_means.ipynb
original kmeans implementation, without using PCA features (Depreciated)

### kmeans_3.csv
full data labeled using the original kmeans without PCA (Depreciated)

### K_means_standardized.ipynb
kmeans implmentation using standardized features, without using PCA features (Depreciated)

### kmeans_3_standardized.csv
full data labeled using the standardized kmeans without PCA (Depreciated)

### K_means_reduced.ipynb
kmeans implementation using 7 PCA features (retain ~80% of variance)

### kmeans_pca_80.csv
full data labeled using kmeans with 7 PCA features (retain ~80% variance)

### K_means_pca3.ipynb
kmeans implementation using 3 PCA features

### kmeans_pca_3.csv
full data labeled using kmeans with 3 PCA features

### visualization.ipynb
visualization of the kmeans clustering (only shows kmeans with 3 and 7 PCA features)

## DBScan

### dbscan_pca80.ipynb
implementation of dbscan using the 7 PCA features 
also includes visualization

### dbscan_pca80.csv
full data labeled using dbscan with 7 PCA features

### dbscan_pca3.ipynb
implementation of dbscan using the 3 PCA features
also includes visualization

### dbscan_pca3.ipynb
full data labeled using dbscan with the 3 PCA features


