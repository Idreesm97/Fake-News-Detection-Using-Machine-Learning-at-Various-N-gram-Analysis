########################################################################################################
####################################        FINAL PROJECT        #######################################
########################################################################################################

 GOAL: Detection of Fake News using various Machine Learning Classifier algorithms and evaluation of 
       their performance in order to find whether the given approaches are appropriate and suitable 
       in order to accurately detect fake news.

 Task 1: Generation of DataSet

		> A. For fake news we used Kaggle’s ‘Fake News’ dataset.
		     The CSV file with data was available off the shelf for use, and we had to perform
                     extensive text pro-cessing and cleaning on this dataset in order to ensure it was suitble
		     when it came to modelling. The link to the given dataset can be found here: https://www.kaggle.com/c/fake-news/data
		     Ideally our own data source would have been much more appropriate, but due to the limited time-availability and resource 
		     at my disposal it was decided to instead use a suitable secondary dataset instead in order to ensure completion of the given 
		     project.
		> B. Once the given dataset was appropriately cleaned and conformed to the given objectives it was then time to ensure the corpus
		     was able to understood by the machine learning algorithms. This required suitable feature extraction techniques to be chosen.
		     For this approach it was decided Term-Frequency Inverse-Document-Frequency would be used along with Bag of Words.

Task 2: Implementation of Classifier Algorithms (Testing was done using a train/test split of 70:30):
		
		(Each Machine Learning Classifier chosen was implemented on both TF-IDF and Bag of Words Feature Extraction
		 technique in order to find the most suitable approach.)

		> A. Implemented Multinomial Naive Bayes Algorithm from scratch and test it against the 
                     dataset.
		> B. Implemented Logistic Regression Classifier Algorithm from scratch and test it against 
		     the dataset.
		> C. Implemented Linear Support Vector Machine Classifier Algorithm and test it against the 
		     dataset.
		> D. Implemented Random Forrest Classifier Algorithm and test it against the 
		     dataset.
		> E. Implemented 2 voting Ensembles with each ensemble being implmented on TF-IDF and Bag of Words and test it against the 
		     dataset.
Task 3: Implementation of Evaluation Measure:
 	  
 	  	> A. Implemented methods to calculate accuracy of the prediction algorithms.
		> B. Implemented methods to calculate precision of the prediction algorithms.
		> C. Implemented methods to calculate recall of the prediction algorithms.
		> D. Implemented methods to calculate F1-Score of the prediction algorithms.
		> E. Implemented methods to calculate K-Fold Cross Validation of the prediction algorithms.


######################################################################################################

OUTCOME:

		> It was found that not only with the given approach were we able to accurately detect fake news 
		  but also with a relatively high accuracy as it was noted that the Linear Support Vector Machine was
		  able to achieve 95% accuracy at 5-fold cross validation at word level for TF-IDF.
		> It can also be noted that there was minemal difference between the suitability of TF-IDF against Bag of Words
		  with both feature extraction techniques performing well at various N-Gram levels with various different classifiers.