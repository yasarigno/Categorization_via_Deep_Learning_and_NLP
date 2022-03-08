---
### PROJET-6
### Classification of customer profiles of OLIST, an e-commerce site
---

<p align="center">
<img align="center" src="support\olist.png" style="width: 300px" />
</p>

We provide OLIST's e-commerce teams a customer segmentation that they can use on a daily basis for their communication campaigns. The aim is to provide the marketing team an actionable description of customer segmentation and its underlying logic for optimal use. In this project we analyse types of customers through their behavior and personal data. We therefore use unsupervised methods to group customers with similar profiles. The customers has been classified into 8 profiles. 
We also provide OLIST a maintenance contract proposal based on an analysis of the stability of the classification over time.

The figure below shows one of these 8 profiles. In a nutshell, we see that customers Cluster 1 give low review scores. One of the reasons for their dissatisfaction seems to be the delivery delay. We can also say that these users live in cities farther from the seller they shop at. For this customer profile, delivery delay is a sign of unhappiness.

<p align="center">
<img align="center" src="support\profile.png" style="width: 600px" />
</p>

---
Data source:

https://www.kaggle.com/olistbr/brazilian-ecommerce

| DATA  |   |
|---|---|
|  number of lines |   119 151 |
|  number of columns |   30 |

---

There are 5 notebooks in this project. 

**Notebook 1 :** Data Cleaning and Exploratory Data Analysis. 

**Notebook 2, 3 :** K-NN algorithm is performed for two different sets of features.

**Notebook 4 :** DBSCAN is tested.

**Notebook 5 :** Hybride model. In this notebook we mix Hierarchical Clustering and K-NN. This allows us to choose the number of clusters, that is the number **K** in the KNN algorithm, by using the nice picture (which is a dendrogram) of hierarchies. Since the K-NN itself gives good results we did not need this method in order to reach a conclusion. However it can be very useful for more large datasets. 

---
We have tested the following unsupervised Machine Learning algorithms here:
  - KNN
  - DBSCAN
  - Hierarchical Clustering

<p align="center">
<img align="center" src="support\profile.png" style="width: 600px" />
</p>

