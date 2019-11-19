
+++ title = "Text Classification " 
summary = " Naive Bayes Text classifier " 
+++
## Background 
Naive Bayes is based on Bayes' Rule which finds the probability of an event occuring given the probability of another even that has already occured. It is based on prior probability. We use a **feature matrix** and a **response vector** 
 ![YES](/post/naiveBayes.png)
We divide the data set into parts. 40% training set, 20% for development, and 20% for  test data
For this dataset of Trending Youtube videos I divided the Categories into 4 different Categories: Comedy, Entertainment, How-to, Culture

## General Idea
## Link to Github 
Link to repository on github and Readme instructions on how to run. 
[Github](https://github.com/sergiog23/YoutubeSearchClassify/blob/master/README.md)

## Challenges faced:
 Some of the challenges I faced when developing Phase in was getting used to dealing with a large data set and implementing TF-IDF without using a prebuilt library. My dataset was also not the best for this project because in my Youtube video dataset the textual component in  ['description'] did not give very good insight on the content of the video. It had many links to Youtuber's references and information not related to the video. Also, when I was trying to tokenize the file I ran into problems because some of the rows sections was empty so it was getting wrong data.
## Overcoming Challenges
Luckily I had many resources available to get me back on the right track. I used Pandas a python library that is very helpful to building a dataset. For filering out the non-alphabetic content I used a regular expression. 
## Experiments 
I did an experiment with and without stopwords. When I did not remove the stop words I had alot of results that did not include what I was looking for. Since most of the entries had stop words I would get back many results since many of the documents had stop words. When I used the stemmer I got better results because it was more focused on the key words in the search. 

## References: 