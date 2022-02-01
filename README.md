# Stock Prediction -Sentiment-Analysis-News-Headlines-Machine Learning
How Random Forest Works
Random forest is a supervised learning algorithm. The "forest" it builds, is an ensemble of decision trees, usually trained with the “bagging” method. The general idea of the bagging method is that a combination of learning models increases the overall result.

Put simply: random forest builds multiple decision trees and merges them together to get a more accurate and stable prediction.

One big advantage of random forest is that it can be used for both classification and regression problems, which form the majority of current machine learning systems. Let's look at random forest in classification, since classification is sometimes considered the building block of machine learning. Below you can see how a random forest would look like with two trees:

two tree random forest
![image](https://user-images.githubusercontent.com/97341259/151928660-28df5586-19ec-4bf3-af89-afba686a1a2a.png)

Random forest has nearly the same hyperparameters as a decision tree or a bagging classifier. Fortunately, there's no need to combine a decision tree with a bagging classifier because you can easily use the classifier-class of random forest. With random forest, you can also deal with regression tasks by using the algorithm's regressor.

Random forest adds additional randomness to the model, while growing the trees. Instead of searching for the most important feature while splitting a node, it searches for the best feature among a random subset of features. This results in a wide diversity that generally results in a better model.

Therefore, in random forest, only a random subset of the features is taken into consideration by the algorithm for splitting a node. You can even make trees more random by additionally using random thresholds for each feature rather than searching for the best possible thresholds (like a normal decision tree does).
Important Hyperparameters
The hyperparameters in random forest are either used to increase the predictive power of the model or to make the model faster. Let's look at the hyperparameters of sklearns built-in random forest function.

1. Increasing the predictive power

Firstly, there is the n_estimators hyperparameter, which is just the number of trees the algorithm builds before taking the maximum voting or taking the averages of predictions. In general, a higher number of trees increases the performance and makes the predictions more stable, but it also slows down the computation.

Another important hyperparameter is max_features, which is the maximum number of features random forest considers to split a node. Sklearn provides several options, all described in the documentation.

The last important hyperparameter is min_sample_leaf. This determines the minimum number of leafs required to split an internal node.
Naïve Bayes, which is computationally very efficient and easy to implement, is a learning algorithm frequently used in text classification problems. Two event models are commonly used: 

Multivariate Bernoulli Event Model
Multivariate Event Model
The Multivariate Event model is referred to as Multinomial Naive Bayes.

When most people want to learn about Naive Bayes, they want to learn about the Multinomial Naive Bayes Classifier. However, there is another commonly used version of Naïve Bayes, called Gaussian Naive Bayes Classification.

Naive Bayes is based on Bayes’ theorem, where the adjective Naïve says that features in the dataset are mutually independent. Occurrence of one feature does not affect the probability of occurrence of the other feature. For small sample sizes, Naïve Bayes can outperform the most powerful alternatives. Being relatively robust, easy to implement, fast, and accurate, it is used in many different fields.

For Example, Spam filtering in email, Diagnosis of diseases, making decisions about treatment, Classification of RNA sequences in taxonomic studies, to name a few. However, we have to keep in mind about the type of data and the type of problem to be solved that dictates which classification model we want to choose. Strong violations of the independence assumptions and non-classification problems can lead to poor performance. In practice, it is recommended to use different classification models on the same dataset and then consider the performance, as well as computational efficiency.

Also Read: Top Machine Learning Interview Questions

To understand how Naïve Bayes works, first, we have to understand the concept of Bayes’ rule. This probability model was formulated by Thomas Bayes (1701-1761) and can be written as:



where,
PA= the prior probability of occurring A
PBA= the condition probability of B given that A occurs
PAB= the condition probability of A given that B occurs
PB= the probability of occuring B

The posterior probability, can be interpreted as: What is the revised probability of an event occurring after taking new information into consideration?

It is a better reflection of the underlying truth of a data generating process because it includes more information.

Conditional Probability
The probability of one event A occurring when another event B with some relationship to A has already occurred is called conditional probability.


This expression is valid only when P(A) is greater than zero.

Prior Probability
This probability can be defined as the prior knowledge or belief i.e. the probability of an event computed before the collection of new data. This probability is revised as new information becomes available to produce more accurate results.

If the prior observations are used to calculate the probability, we call it prior probability.


The Bag of Words Model
Feature extraction and Selection are the most important sub-tasks in pattern classification. The three main criteria of good features are:

Salient: The features should be meaningful and important to the problem
Invariant: The features are resistant to scaling, distortion and orientation etc. 
Discriminatory:  For training of classifiers, the features should have enough information to distinguish between patterns.
Bag of words is a commonly used model in Natural Language Processing. The idea behind this model is the creation of vocabulary that contains the collection of different words, and each word is associated with a count of how it occurs. Later, the vocabulary is used to create d-dimensional feature vect

