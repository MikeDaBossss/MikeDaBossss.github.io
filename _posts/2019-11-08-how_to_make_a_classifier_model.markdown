---
layout: post
title:      "How to make a classifier model"
date:       2019-11-09 00:07:17 +0000
permalink:  how_to_make_a_classifier_model
---


### The first step in building a classifier model is to find a dataset.

Data science projects are more fun when the type of project has something that is interesting to you. Whether the interesting part is finding out the classification type, the overall dataset is interesting to you, or whatever your reason might be. For my classifier model project I picked a dataset whether or not people made over $50,000 per year or not. I thought this was interesting because everyone wants to know why some people make more money than others. 

### The second step is to make sure that the data is clean. 

The data needs to have no missing values, unformatted data columns, and in the right type of order for the classifier models. I worked with a dataset from the University of California Irvine machine learning dataset.  So it was already perfectly clean and had no missing values all I had to do was do a small amount of formatting . 

### The third step is to pick a type of classifier type

There are lots of classifier types that you can use. There is logistic regression, SVM's, K nearest neighbors, Decision Trees, and ensemble methods that combine multiple methods together in order to get a better result. These ensemble methods are the best because if each classifier is better than guessing then if you have lots of "votes" or classifications on each prediction then the odds would go from say 51% to something say 60% if there were 4 classifiers each doing different methods each providing 51% accuracy or better than a guess if it was a binary classification. The odds would better because if each guess is better than a random guess and you make the binary classification based on which class got the most "votes" then when you increase the amount of "voters" then you increase the odds of the overall "vote" being correct. 

### The fourth step is to split the data into test/train splits

This step is important because you do not want your classifier to overfit to the data. It is better that your model is generally accurate than 100% accurate because future data will only be generally similar not exactly similar. I split my data into 80% training and 20% testing.

### The fifth step is to train the classifier

I decided on an ensemble method called random forest which uses multiple decision trees to get "votes". It usually works pretty accurately and is a quick method for the computer to run. On my first attempt with the default settings I got 87% accuracy.

### The sixth step would be to tune the classifier

If you could have unlimited computing power you could run a huge amount of different parameters for the classifier and then you would find the best set of parameters , but since I don't have that I just looked for a few of the parameters with a few different values. I used an sklearn Grid Search to accomplish this. 

### Finally it is important to make sure that the test set is accurate 

You need to make sure that the test set is getting good results also. If the test set doesn't get good accuracy numbers then the parameter settings are not properly tuned and if the test set accuracy is much lower than the training set then the classifier has overfit and the parameters must be switched. 

### A last note

You can try different types of models and ensemble methods in order to accomplish the best accuracy. It would be more important to do feature engineering and run all sorts of different models, parameter values, and ensemble methods in order to get the best possible method. I have seen feature engineering be the biggest difference between one model winning a kaggle data competition and another model winning. Feature engineering is difficult because you have to come up with the features from nothing. This means that you have to either know what features will be important or you could try to make hundreds of features and run models to see which features would have the most effect. Also if you were a big company like google with as close as unlimited resources you could test all the features, parameters, classifiers, and ensemble methods.
