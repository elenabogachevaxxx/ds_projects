 The goal of the project is to train the model to identify toxic comments on a store’s website and evaluate the model using the F1 metric.
 
 During the work on the project, the texts of comments for training models were prepared - unnecessary characters and spaces were removed, tokenization and lemmatization of the text was carried out.


The lemmatized text was passed to the pipeline, included vectorizer TF-IDF and 3 models (Logistic Regression, DecisionTreeClassifier, KNNClassifier).

Cross-validation was carried out to select the best model and its hyperparameters, logistic regression was chosen as the best model, the F1 metric on cross-validation was 78.1%. Predictions were obtained on the test sample; the F1 metric on the test sample was 78.5%.

Thus, logistic regression, given its fast performance and satisfactory prediction quality, can be used to select toxic comments.
