In this NLP project I attempt to classify Yelp Reviews into 1 or 5 star categories based on the text content in the reviews.   

The dataset is provided in csv format with 10 000 entries.  The complete dataset can be downloaded from Kaggle: [Yelp Review Data Set from Kaggle](https://www.kaggle.com/c/yelp-recsys-2013).  Each observation in this dataset is a review of a particular business by a particular user.  

In this project I use the following libraries and toolkits: Scikit-learn, Natural Language Toolkit, Seaborn, Matplotlib and  Pandas.  

Some interesting analyses and interpretations from visualizations in this project:    
* It has been found that most users rate a business with a 4 or 5 star. 
* We see a tendency of users who rate with a 4 or 5 star to write shorter reviews than those who rate with a 2 or 3 star.  We see this in all the quartiles and the means of the length of texts vs the star rating. 
* As the number of 'useful' clicks on a review increase, the number of 'cool' or 'funny' clicks on the review also tends to be more. 
* A Multinomial Naive Bayes model is fit to the data which makes good predictions on the star ratings based on the text content of the review.   

Column descriptions: (columns that will be used)  
* stars:  The number of stars (1 through 5) or rating assigned by the reviewer to the business. 
* text:  The text from the review. 
* cool:  The number of "cool" votes a specific review received from other Yelp users, i.e. a rating of the review itself 
* useful:  The number of "useful" votes a specific review received from other Yelp users, i.e. a rating of the review itself 
* funny:  The number of "funny" votes a specific review received from other Yelp users, i.e. a rating of the review itself
