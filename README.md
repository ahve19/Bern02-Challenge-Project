# Bern02-Challenge-Project
A project for analyzing different models diagnosing breast cancer. Models include both supervised and unsupervised learning.

# File Structure

- `DataVisualizations.ipynb` – exploratory data analysis and visualizations
- `Supervised_Learning.ipynb` – supervised learning models for breast cancer classification
- `unsupervised_learning.ipynb` – PCA and clustering analysis
- `data.csv` – dataset used in the analyses
- `requirements.txt` – Python packages required to run the notebooks
- `LICENSE` – license information for the project

# The problem

The goal of this project is to investigate whether features extracted from
digitized breast cell images can be used to distinguish between benign and
malignant tumors.

Supervised learning is used to evaluate how accurately diagnosis can be
predicted when labelled examples are available. Unsupervised learning is used
to investigate whether similar groups can be identified from the structure of
the features without providing the diagnosis labels to the models.

# Exploratory Data analysis

## Supervised Learning

For the Random Forest model, a confusion matrix was used to visualise the
classification results, since it makes it easier to visualize the types of errors made by the model. 

## Unsupervised Learning

For PCA, a line plot of cumulative variance was used to show how much of the total variation is explained as more principal components are included. A line plot was chosen because the number of components is ordered, and so a line plot clearly shows how the explained variance increases. Horizontal bar plots were used for the PCA loadings of PC1 and PC2 because bar plots make it easy to compare the contribution of the different features, while the horizontal layout makes the longer feature names easier to read.

For K-means, line plots were used to compare inertia and silhouette score
across different values of `k`. These plots were chosen because `k` is again ordered.

Scatter plots of PC1 against PC2 were used to visualise the K-means and
hierarchical clustering results. The original dataset contains 30 features,
so it could not be plotted directly in two dimensions, whilst PCA allowed the samples
to be displayed using two axes. The clustering result was shown next to the
known diagnosis so that the patterns could be easily compared. 

Dendrograms were used for hierarchical clustering because they show how
individual observations and clusters are joined at different linkage
distances. 

# Supervised Learning
Justify the choice and discussion of limitations of the method

# Unsupervised Learning
K-means and hierarchical clustering were chosen because they provide two
different methods of investigating whether the observations form groups naturally
without using diagnosis labels.

K-means is simple to implement and easy to interpret, but it works best when clusters are
well-separated.

Hierarchical clustering provides another view of the relationships between
observations, but the results depend on the choice of linkage method and
distance measure.

# FAIR principles
## Findable

[] make doi
This repository is public on Github and is findable through a google search. In addition, the repository is described by metadata that provides a second resource of being findable. The repository has a DOI that can also be used to find it.
## Accessible

This repository is freely accessible on Github and the license provides insight on how it can be used. The CC-BY-NC-Sa license was chosen as the dataset has this license. As a result, any code using this dataset must follow the same license.

## Interoperable (run it on other stuff)
The project uses widely supported file formats and software - the data us stored as a CSV file and the analyses are written in Jupyter Notebooks using Python. The `requirements.txt` file lists the packages needed to run the analyses.

## Reusable

The repository contains the data, notebooks, requirements file, and license needed to rerun the project. A `requirements.txt` file shows the software dependencies, and fixed random seeds are used throughout all code where relevant so that the results can be reproduced consistently for other users. 
