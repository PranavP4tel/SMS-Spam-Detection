# SMS-Spam-Detection
Worked with a dataset containing text and labels indicating the messages as spam or ham.
Dataset - https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset

---
Workflow:
1. Data Cleaning and Preprocessing - Evaluating data quality, removing irregular characters, standardizing text formats and removing stopwords
2. Data Visualization - Creating wordclouds for both the labels to spot patterns.
3. Model creation and evaulation without cross-validation - Creating a function to take the model and input data, fit a pipeline model on it and evaluate it. Used TFIDF Vectorizer in the pipeline to convert the text into numerical format.
4. Model creation and evaulation with cross-validation - Creating a function similar to the above, with cross-validation capability for 6 models.
5. Embeddings and model creation - Created word embeddings, used SCaNN from google for similarity searching and KNN Classifier, with evaluation.

---
Conclusion:
1. Via data visualization, we can spot some recurring words in the spam texts such as free, prize, win, offer, etc.
2. Multinomial Naive Bayes Classifier is known for working well on text classification problems and provided the best accuracy of 98.3% and 98.4% (with and without hyperparameter tuning).
3. Other algorithms also provided a great accuracy of above 90%.
