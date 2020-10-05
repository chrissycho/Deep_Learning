# Chrissy Cho's Deep_Learning
### Table of Contents
[ 1. Project Overview ](#desc)<br /> 
[ 2. Resources ](#resc)<br /> 
[ 3. Objectives ](#obj)<br /> 
[ 4. Challenge Overview ](#chal)<br /> 
[ 5. Challenge Objective ](#chalsum)<br /> 
[ 6. Final Thoughts ](#find)<br />


<a name="desc"></a>
## Project Overview
In this module, we've learned building a basic neural network and deep learning model. In the later module, we also learned the differences between supervised learning models and neural network models. 

<a name="resc"></a>
## Resources
- Data Source: [Alphabet Soup Challenge Data](https://github.com/chrissycho/Deep_Learning/blob/main/challenge/charity_data.csv)
- Software: Jupyter Notebook, Python3 

<a name="obj"></a>
## Objectives
- Describe the differences between supervised and unsupervised learning, including real-world examples of each.
- Preprocess data for unsupervised learning.
- Cluster data using the K-means algorithm.
- Determine the best amount of centroids for K-means using the elbow curve.
- Use PCA to limit features and speed up the model.

<a name="chal"></a>
## Challenge Overview
In this challenge, we have to build our own machine learning model that will be able to predict the success of a venture paid by Alphabet soup.
## Challenge Background
From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received various amounts of funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization such as the following:

- EIN and NAME—Identification columns
- APPLICATION_TYPE—Alphabet Soup application type
- AFFILIATION—Affiliated sector of industry
- CLASSIFICATION—Government organization classification
- USE_CASE—Use case for funding
- ORGANIZATION—Organization type
- STATUS—Active status
- INCOME_AMT—Income classification
- SPECIAL_CONSIDERATIONS—Special consideration for application
- ASK_AMT—Funding amount requested
- IS_SUCCESSFUL—Was the money used effectively

We've created a binary classifier that is capable of predicting whether or not an applicant will be successful if funded by Alphabet Soup. The model is expected to have 75% accuracy.

<a name="chalsum"></a>
## Challenge Objective
- Import, analyze, clean, and preprocess a “real-world” classification dataset.
- Select, design, and train a binary classification model of your choosing.
- Optimize model training and input data to achieve desired model performance.

<a name="find"></a>
## Final Thoughts
1. How many neurons and layers did you select for your neural network model? Why?
In this model, we've created two hidden layers with 8 neurons and 5 neurons, respectively. This is done by trial and error since adding more neurons do not increase accuracy, the optimal result was shown with 8 and 5 neurons. 

2. Were you able to achieve the target model performance? What steps did you take to try and increase model performance?
At first, we didn't achive the target model performance, which should be higher than 75% accuracy. To increase the accuracy, we've added more neurons and tested the model out. We also added more epochs in the model. The disadvantage with many neurons and more epochs is a risk of overfitting. The disadvantage with more neurons and epochs is a risk of overfitting.  Lastly, we've also tried changing the activation function in the output to tanh but it actually decreased the model so we kept relu in the input and sigmoid in the output. 

3. If you were to implement a different model to solve this classification problem, which would you choose? Why?
If I were to implement a different model to solve the classification problem, I'd compare with other machine learning models such as logistic regression, support vector machine and random forest. Sometimes, logistic regression models can return the output quickly than deep learning models with the same accuracy level.