## CS 7641 Assignment 3: Unsupervised Learning and Dimensionality Reduction
This project seeks to understand the computatitonal and predictive qualities of two unsupervised learning techniques and four dimensionality reduction techniques.

Unsupervised Learning Methods: k-means, expectation maximization (EM)

Dimensionality Reduction Methods: principal components analysis (PCA), independent components analysis (ICA), random components analysis (RCA) and random forest selected components(RFA).

The two example datasets used in this project are:

Dataset 1: Phishing Websites - available at https://www.openml.org/d/4534

Dataset 2: Bank Marketing - available at https://www.openml.org/d/1461


## Getting Started & Prerequisites
For testing on your own machine, you need to install python 3.6 and the following packages:
- pandas, numpy, scikit-learn, matplotlib, itertools, timeit


## Running the Code
Optimal Way: Work with the iPython notebook (.ipnyb) using Jupyter or a similar environment. This allows you to "Run All" or you can run only the subsections that you are interested in.

View Only Option : Feel free to open up the (.html) file to see a snapshot of the cleaned code without any output.

The code is broken up into the following sections sections:
1. Data Load & Preprocessing -> This section loads the data, performs one-hot encoding, scales numeric features, and reorders some of the columns.
2. Helper Functions -> This section defines a few functions that are used throughout the assignment The functions include building learning curves, evaluating the classifers, performing a mode-vote routine within clusters.
3. Clustering: k-means and EM -> This section runs k-means and EM and produces some heuristic plots so that one can select the optimal number of clusters.
4. Dimensionality Reduction -> Performs PCA, ICA, RCA, and random forest dimensionality reduction on the original datasets.
5. Training Neural Network on Projected Data -> A fixed architecture neural network is trained from each of the reduced datasets. Learning curves are generated.
6. Model Comparison Plots -> Generates plots to compare each of the neural networks.
7. Training Neural Network on Projected Data and Cluster Lables -> Same as section 5, but this section adds new one-hot encoded features that represent cluster structure in the dataset.
