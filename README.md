---
### PROJET-6
### Recognition of categories of products from images and textual descriptions.
---

<p align="center">
<img align="center" src="support\logo.png" style="width: 300px" />
</p>

We are given a dataset which consists of pictures of goods and their descriptions. The csv file contains some other information such as the price of the product, the name of the product and its brand. There is as well a variable "product_category_tree" which defines categories and 6 subcategories of the product. This variable is defined manually by the sellers. As the size of our dataset grows up drastically, the task of associating the product to the category will be a burden. Therefore we must automatize this task by using only the pictures and the descriptions. Now the problem that we want to solve is converted into a problem of Natural Language Processing (NLP) and that of Computer Vision (CV). 

We approach to this problem of recognition of categories from different aspects. First we use only the descriptions and perform algorithms of NLP, then in later notebooks we take the tools of CV into account.

Let us see what we have as input and how it looks like. For instance, the first product is a purple curtain. its description

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
<img align="center" src="support\first_photo.png" style="width: 300px" />
</p>

