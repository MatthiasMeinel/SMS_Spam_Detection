# SMS_Spam_Detection

This project is aimed at building a model to detect SMS spam using a dataset containing labeled SMS messages. We employ a Linear Support Vector Machine classifier along with TF-IDF vectorization to process the text data and train the model.

Dependencies
Python 3.7
Pandas
NumPy
Scikit-learn
Dataset
The dataset used in this project is the smsspamcollection.tsv file which contains SMS messages labeled as 'ham' (non-spam) or 'spam'. Each message is also accompanied by its length and punctuation count.

#Project Structure

The initial part of the script imports necessary libraries.

The dataset is loaded using pandas and some preliminary exploratory data analysis is performed to check for missing values and inspect the balance of labels.

The data is split into training and testing sets, and TF-IDF vectorization is applied to the text data.
A Linear Support Vector Machine classifier is trained on the vectorized text data.

To streamline the process, a scikit-learn pipeline is created which encapsulates the vectorization and classification steps.

The model is evaluated on the testing set using confusion matrix, classification report, and accuracy score to gauge its performance.

#Evaluation
The model achieved an accuracy of approximately 99.22% on the testing set, indicating a high level of effectiveness in distinguishing between spam and non-spam messages.

##Further Improvement
There's room for further improvement by experimenting with different classifiers, tweaking the hyperparameters, or employing additional text preprocessing techniques.
