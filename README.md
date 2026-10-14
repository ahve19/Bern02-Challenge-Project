# Bern02-Challenge-Project
A project for analyzing different models diagnosing breast cancer. Models include both supervised and unsupervised learning.

# File Structure
- DataVisualizations.ipynd
- Supervised_Learning.ipynd

# The problem
We are trying to compare different models on classifying breast cancer using features from a digitized cell image.

# Exploratory Data analysis

Note will need to discuss why certain graph choices were chosen

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
