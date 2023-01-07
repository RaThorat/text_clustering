# text_clustering
The grouping of texts into various clusters can be used to differentiate various themes within the texts
This code performs K-means clustering on a set of text documents. The first step is to import the text files and prepare them for analysis by dropping any null values, removing punctuation, and performing tokenization, stopword removal, and lemmatization. Next, the TfidfVectorizer class is used to create a vector representation of the documents, which is then used in the K-means clustering algorithm to group the documents into clusters. The centroids of these clusters are then printed, along with the features belonging to each cluster. Finally, the model is pickled and saved using the joblib.dump function, and can be used to cluster new keywords by dropping unnecessary columns and saving the output to an Excel file.

## Preparation

Importing the text files for clustering, close the popup window after uploading the file.

Creating a column named 'Corpus' from the Text

## Text tokenizing, lemmatizing, stopword removal

dropping the nan values from text

dropping the punctuation from text

tokenization

removing the stopwords

lemmatization

conversion of columns to lists

Converting vector values into string values

## K-means clustering

create vectorizer usingTfidfVectorizer class to fit and transform the document

clustering algorithm

making a list of labels

Get the centroids and features

print the centroids into which clusters they belongs

## Pickling and saving the model

use joblib.dump to pickle the model, once it has converged and to reload the model/reassign the labels as the clusters.

uncomment the below code to save your model

since I've already run my model I am loading from the pickle

## using the model to cluster the keywords

Dropping the columns unncessary for output

give name to the output excel
