## Compare the methods of multi label text classification
 The work aims to compare the differnt multi label classification methods . The kaggle 'Toxic Comment Classification Challenge' data is used for the multi label classification. A comment maight be labelled as toxic, severe toxic, obscene, threat, insult or identity hate at the same time or not belong to any class. worked over the 3 methods of comment classification. There are many methods for multi cass classification like one vs rest strategy of sklearn, adaptive algorithms,  Problem Transformation methods like 'Binary Relevance', ' Label Powerset', etc. deep learning methods etc.

## Libraries used
 - keras
 - sklearn
	
Dowload  the Toxic Comment Classification Challenge data set.


## Techniques used

 1. One vs rest
 2. Binary relevence
 3. GRU

## Preprocessing
   For the whole models bulding, clean the data, by removing punctuations, symbols etc, remove html tags inside data, the stem the each word using PorterStemmer. 

## vectorisation
  Mainly use tf idf vectorisation of sklearn.

## 1. One vs rest
 - OneVsRestClassifier with LogisticRegression
 - OneVsRestClassifier with LinearSVC

    OneVsRestClassifier with LogisticRegression have good accuracy over the other. Accuracy of both the classifiers are checked for categorical data as well as whole data
## 2. Binary Relevance
    Consider each label as seperate classification model. The accuracy score is not better as the one vs rest methods. 
## 3. GRU
	Use keras GRU. create the network with one embedding layer, 2 GRU layer and one dense layer. The output produced by this deeplearing layer is better the above adopted methods.

