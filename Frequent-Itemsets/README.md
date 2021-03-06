# Frequent Itemsets

Instructor: Prof. Madhavan Mukund, Chennai Mathematical Institute

The Task

The "Bag of Words" data set from the UCI Machine Learning Repository contains five text collections in the form of bags-of-words. 
The URL for the UCI repository is http://archive.ics.uci.edu/ml/datasets/Bag+of+Words. 
Your task is to compute frequent itemsets for this data. 
In each of the text collections, each document is summarized as a bag (multiset) of words. 
The individual documents are identified by document IDs and the words are identified by word IDs. 
In each collection the vocabulary of unique words has been truncated to only keep words that occurred more 
than ten times in that collection. 

For each collection XYZ: 
•	vocab.XYZ.txt is the vocabulary file, listing all words that appear in the collection XYZ, one word per line. 
	Each word has an implicit wordID that is its line number in this file, starting with 1 
	(the word on line 1 has wordID 1, the word on line 2 has wordID 2, ...)
•	docword.XYZ.txt lists out the number of times each word in vocab.XYZ.txt occurs in each document 
	(only non-zero counts are recorded).

The file docword.XYZ.txt begins with 3 header lines
	  D
	  W
	  NNZ
	
where D is the number of documents in the collection, W is the number of words whose frequency is counted 
(i.e., W is the number of words in vocab.XYZ.txt) and NNZ is the number of non-zero frequency entries for this collection 
(i.e., NNZ is 3 less than the number of lines in docword.XYZ.txt). 

This is followed by NNZ lines of the form 
	  docID wordID count
	
where count is the number of time the word with id wordID appears in document with id docID. 
Remember that only non-zero counts are recorded. 
As usual, a K-itemset of words is a collection of words of size K that occur together in the same document. 
Your assignment is to write a program to find all K-itemsets of words occurring with frequency F, 
where K, F and the name of the dataset to use should be parameters to your program. 
