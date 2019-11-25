
+++ title = "Search " 
summary = " Search Engine using TF-IDF in python " 
+++
## Background 
In this Data Mining Project I used **Tf-idf** (term frequency-inverse document frequency) to develop my search feature on my 'iOS Mobile APP dataset' This dataset has about 7K entries and I am using the Title and Description as the textual component to search. Tf-idf is a very popular weighting scheme for scoring and ranking a document's relevance given a users query. 

## Phase I.
In this part of the project I developed a search engine using Python3, numpy,Flask, nltk, and pythonanywhere. 
I used TF-IDF to compute the score of each document in the Data. 
Link to Readme with explanation on deployment instructions 
Term frequency was calculated using how many times the term appeared in the document. 
 ![YES](/post/tfIDF.png)

        ' for row in dataset:
            for term in row:
                    tf = row.count(term)/len(row)
                    df = sum(1 for document in final_document if term in document)
                    toat = tf * math.log10(len(dataset)/df)'
## Link to Github 
Link to repository on github and Readme instructions on how to run. 
[Github](https://github.com/sergiog23/YoutubeSearchClassify/blob/master/README.md)

## Challenges faced:
 Some of the challenges I faced when developing Phase in was getting used to dealing with a large data set and implementing TF-IDF without using a prebuilt library. My dataset was also not the best for this project because in my Youtube video dataset the textual component in  ['description'] did not give very good insight on the content of the video. It had many links to Youtuber's references and information not related to the video. Also, when I was trying to tokenize the file I ran into problems because some of the rows sections was empty so it was getting wrong data. I got the Search feature working for that dataset but ran into problems when I was doing the classifier, I ended up changing the Data set to an iOS App Dataset I found on Kaggle, it had a better description for each app and did not have as much noise as the Youtube Dataset. 
## Overcoming Challenges
Luckily I had many resources available to get me back on the right track. I used Pandas a python library that is very helpful to building a dataset. For filering out the non-alphabetic content I used a regular expression. 
## Experiments 
I did an experiment with and without stopwords. When I did not remove the stop words I had alot of results that did not include what I was looking for. Since most of the entries had stop words I would get back many results since many of the documents had stop words. When I used the stemmer I got better results because it was more focused on the key words in the search. 

## References: 
[TF-IDF](https://www.tfidf.com/)
[Flask](https://www.youtube.com/watch?v=MwZwr5Tvyxo&list=PL-osiE80TeTs4UjLw5MM6OjgkjFeUxCYH)
[Python TF-IDF](https://www.freecodecamp.org/news/how-to-process-textual-data-using-tf-idf-in-python-cd2bbc0a94a3/)
