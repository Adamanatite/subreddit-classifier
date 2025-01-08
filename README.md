# Subreddit Text Data Classifier Exploration
This was a text data classification assessment I completed as part of my 3rd year of university.


## The Data
The data we were given was reddit posts. This included the post title, author, post body, ID, score (number of upvotes) and subreddit (hidden from the training data, what is to be classified). There were 2000 entries in the data set (1200 for training, 400 for validation, 400 for testing). An example of a post body in the dataset, from subrredit r/PS4, is "Long story short, I saw ESO in my library, downloaded it and it let me play it. I don’t think there is a free trial going around. I’m sure I didn’t buy the game."

## The Task
As part of this assessment, I analysed the class balance of the dataset. I then trained and tested two different types of classifier, [Logistic Regression](https://en.wikipedia.org/wiki/Logistic_regression) and [SVC (Support Vector Classifier)](https://en.wikipedia.org/wiki/Support_vector_machine) on two different encodings of the text body, [One-hot encoding](https://www.geeksforgeeks.org/one-hot-encoding-in-nlp/) and [TF-IDF encoding](https://en.wikipedia.org/wiki/Tf%E2%80%93idf). I compared these results against two dummy classifiers: one which guessed randomly based on the distribution of subreddits, and one which always guessed the most frequent subreddit in the dataset.

I analysed the results of the classifiers, including commenting on the [F1 scores](https://en.wikipedia.org/wiki/F-score) and the [confusion matrix](https://en.wikipedia.org/wiki/Confusion_matrix) of the most effective classifier. I then optimised some hyperparameters to improve model performance. Finally, I designed a better classifier, a random forest classifier using TF-IDF encoding which also included the post title, and similarly analysed its results.

