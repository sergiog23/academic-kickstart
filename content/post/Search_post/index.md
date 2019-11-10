
+++ title = "Search " 
summary = " Search Engine using TF-IDF in python " 
+++
## Phase I.
In this part of the project I developed a search engine using Python3, numpy,Flask, nltk, and pythonanywhere. 
I used TF-IDF to compute the score of each document in the Data. 
Link to Readme with explanation on deployment instructions 
Term frequency was calculated using how many times the term appeared in the document. 
 ![YES](/post/TFiDF.png)

        ' for row in dataset:
            for term in row:
                    tf = row.count(term)/len(row)
                    df = sum(1 for document in final_document if term in document)
                    toat = tf * math.log10(len(dataset)/df)'
## Link to Github 
[Github](https://github.com/sergiog23/YoutubeSearchClassify/blob/master/README.md)

## Challenges faced:
 Some of the challenges I faced when developing Phase in was getting used to dealing with a large data set and implementing TF-IDF without using a prebuilt library. My dataset was also no the best for this project because the Youtube video description did not give very good insight on what the video was about. It had many links to Youtuber's references and information not related to the video. Also, when I was trying to tokenize the file I ran into problems because some of the rows sections was empty so it was getting wrong data. 
## Overcoming Challenges

## Experiments 
## References: 
[TF-IDF]("https://www.tfidf.com/")
[Flask]("https://www.youtube.com/watch?v=MwZwr5Tvyxo&list=PL-osiE80TeTs4UjLw5MM6OjgkjFeUxCYH")
[Python TF-IDF]("https://www.freecodecamp.org/news/how-to-process-textual-data-using-tf-idf-in-python-cd2bbc0a94a3/")
