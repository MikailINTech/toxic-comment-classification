# NLP Project : Toxic Comment Classification

## Introduction

In this project, I reviewed two methods to classify toxic comments in a dataset: 
 - Bag of word model, a first simple model to experiment basic concepts.
 - BERT model, using state-of-the-art model to get best possible performance.

The goal was to learn about these concepts and also to see if state-of-the-art model is not overkill for such a task.

## To test the code

The two methods are separated into two folders. In each folder, the preprocessing part and training part are done in two different notebooks. 
The data is provided in the /data folder.

## About the data

The data comes from a [Kaggle competition](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/overview) from 2017. It was submitted by the Conversation AI team, a research initiative founded by Jigsaw and Google working on tools to help improving online conversation. More specifically, the goal is to detect different types of toxicity like threats, obscenity or insults in online comments.

There is a total of 159,571 training examples, each of them consisting of the comment itself and a one-hot representation of 6 different toxic comment classes. Note that this is a multi-class classification task, where a single example can belong to zero, one or several classes. Here is an overview of the differents classes :

![image](https://user-images.githubusercontent.com/45072645/201396275-61dbe03b-d687-4d7d-bafb-746e6b93a966.png)

## Conclusions of the work

The results on the test set are given in the following table :

| **Mean ROC/AUC for bag of words** 	| **Mean ROC/AUC for BERT model** 	|
|:---------------------------------:	|:-------------------------------:	|
|               0.966               	|              0.982              	|

The BERT model performs slightly better than a simple bag of words model at the cost of much important computational ressources but with effortless data processing work.

