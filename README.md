---
### PROJET-6
### Recognition of categories of products from images and textual descriptions.
---

<p align="center">
<img align="center" src="support\logo.png" style="width: 300px" />
</p>

We are given a dataset which consists of pictures of goods and their descriptions. The csv file contains some other information such as the price of the product, the name of the product and its brand. There is as well a variable "product_category_tree" which defines categories and 6 subcategories of the product. This variable is defined manually by the sellers. As the size of our dataset grows up drastically, the task of associating the product to the category will be a burden. Therefore we must automatize this task by using only the pictures and the descriptions. Now the problem that we want to solve is converted into a problem of Natural Language Processing (NLP) and that of Computer Vision (CV). 

We approach to this problem of recognition of categories from different aspects. First we use only the descriptions and perform algorithms of NLP, then in later notebooks we take the tools of CV into account.

Let us see what we have as input and how it looks like. For instance, the first product is a purple curtain. 

<p align="center">
<img align="center" src="support\first_photo.png" style="width: 300px" />
</p>

And its description is:

<p align="center">
<img align="center" src="support\first_description.png" style="width: 700px" />
</p>

In this project we study the feasibility of an engine for classifying articles into different categories, with a sufficient level of precision.

---
Data source:

https://s3-eu-west-1.amazonaws.com/static.oc-static.com/prod/courses/files/Parcours_data_scientist/Projet+-+Textimage+DAS+V2/Dataset+projet+prétraitement+textes+images.zip

| DATA  |   |
|---|---|
|  number of lines |   1050 |
|  number of columns |   15 |

---

There are 5 notebooks in this project. 

**Notebook 1 :** Text mining, Unsupervised models such as TF-IDF, Word embedding via GloVe, Neural networks, Natural Language Processing. We do not use the set of pictures in this Notebook. The steps of transformations on corpus look like this:

<p align="center">
<img align="center" src="support\text_processing.png" style="width: 500px" />
</p>

**Notebook 2 :** Computer Vision via OpenCV. We test the algorithms SIFT and ORB. The dimensionality reduction method that we use here is t-SNE. The results are weak. So we pass to other strategies in the following notebooks. We transform the images as the figures below show:

<p align="center">
  <img align="center" src="support\montre_0.png" style="width: 150px" />
  <img align="center" src="support\montre_1.png" style="width: 150px" />
  <img align="center" src="support\montre_2.png" style="width: 150px" />
  <img align="center" src="support\montre_3.png" style="width: 150px" />
</p>

**Notebook 3, 4 :** Convolutional Neural Networks (CNN). We deep dive into deep learning. The first strategy concerns using CNN. Recall that the last layer called fully-connected classifies the input image of the network. After testing it, we delete this last layer and replace other classifiers. This strategy gives us opportunity to test algorithms like KNN and Random Forest.

**Notebook 5 :** Transfer Learning. We use VGG-16 model to classify the images. We test data augmentation.

**Notebook 6 :** Multi-model. Use of both textual and visual data to built a multi-model.

---
We have tested both supervised and unsupervised Machine Learning algorithms in this project. Transfer learning shows its power and gives the best results. 




