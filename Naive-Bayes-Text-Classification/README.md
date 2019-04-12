# Naïve Bayes Text Classification

Instructor: Prof. Madhavan Mukund, Chennai Mathematical Institute

The Task

The "Reuters-21578 Text Categorization Collection Data Set" data set from the 
UCI Machine Learning Repository contains 21578 news articles that appeared on 
Reuters newswire in 1987. The documents were assembled and indexed with categories. 

The URL for the UCI repository is 
http://archive.ics.uci.edu/ml/datasets/Reuters-21578+Text+Categorization+Collection. 

The articles are grouped into 21 SGML files, with 1000 articles per SGML file. 
Articles may have no topics assigned or even multiple topics. 
Details about the SGML format are given at 
http://archive.ics.uci.edu/ml/machine-learning-databases/reuters21578-mld/README.txt. 
Your task is to build a naïve Bayesian classifier for the Reuters data to assign 
topics to articles, using the topic tags in the training set. Note that an article 
may be assigned more than one topic. You are free to choose a strategy to assign 
multiple topic labels to a document. Preprocessing the SGML data to extract details about 
individual articles and their topic labels is part of the task. 

