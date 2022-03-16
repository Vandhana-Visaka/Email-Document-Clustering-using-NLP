# Email/Document Clustering using NLP

The problem statement can be divided into three sub-problems.

1. Parsing and Data Cleaning
2. Data Pre-Processing and Clustering of Emails
3. LDA for topic modelling

Additionally visualization of clustering is performed.

The respective sub-problems can be found in each of the Python Notebooks named Parts 1, 2, and 3 respectively.

After parsing all 300 emails and cleaning them, the contents are tokenized and saved as a Dataframe.
The cleaned dataframe is exported as input_email.csv that can be found in this directory.

The csv is then read, pre-processed further and prepared as features.
The body of the email messages are clustered using K-means and hierarchial clustering using TF-IDF vectorization.
K-means clustering is achieved using TF-IDF matrix and cosine similarity is calculated to obtain the euclidean distance of all cluster centers.
The proximity of each cluster center to the centroid is used to sort the various coordinates and scale the data points using MDS or Multi-Dimensional Scaling.
The emails are grouped into 5 clusters.

The topics of each cluster is then analyzed using Latent Dirichlet Allocation (LDA) which can be found in Part 3 - LDA.ipynb.




