
+++ title = "Text Classification " 
summary = " Naive Bayes Text classifier " 
+++
## Background 
Naive Bayes is based on Bayes' Rule which finds the probability of an event occuring given the probability of another even that has already occured. It is based on prior probability. We calculate the conditional probability of each term in the dataset.
 ![YES](/post/naiveBayes.png)
 ![YES](/post/posterior.png)


## General Idea
I use the prime_genre column of the dataset to categorize the app. I preporcess the dataset by tokenizing it and removing the stopwords to create a list of terms. Then I calculate the prior probability by dividing the number of documents in each class by the total number of documents. The conditional probability is calcualtes using TF in documents that belong to the class. However, in order to not get 0 in conditional probability we can use **Laplace smoothing** and use the smoothing parameter a = 1 , we add 1 to every probability, therefore the probability will never be zero
 ![YES](/post/laplace.png)
## Link to Github 
Link to repository on github and Readme instructions on how to run. 
[Github](https://github.com/sergiog23/YoutubeSearchClassify/blob/master/README.md)

## Challenges faced:
 Some of the challenges I faced when developing the classifier was

## Experiments 


## References: 
[Flask](https://www.youtube.com/watch?v=MwZwr5Tvyxo&list=PL-osiE80TeTs4UjLw5MM6OjgkjFeUxCYH)
[Naive Bayes](https://towardsdatascience.com/introduction-to-naive-bayes-classification-4cffabb1ae54)
[Train/Test](https://towardsdatascience.com/train-test-split-and-cross-validation-in-python-80b61beca4b6)