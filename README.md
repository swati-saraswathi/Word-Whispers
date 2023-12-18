# Word-Whispers

This project aims to classify emotions in text data using Natural Language Processing (NLP) techniques and machine learning algorithms. The dataset used for this task is the "Emotions Dataset for NLP," which includes text samples labeled with different emotions such as joy, sadness, anger, fear, love, and surprise. The project goes through several key steps, including data loading, preprocessing, visualization, model training, and evaluation.

The initial phase involves loading the dataset and performing basic exploratory data analysis. The dataset is preprocessed by cleaning and transforming the text data. The target variable, representing emotions, is encoded into numerical labels for model training.

Data preprocessing includes text cleaning and lemmatization using the spaCy library. Stop words and punctuation are removed, and the remaining words are lemmatized to their base form. The processed text is then used for training machine learning models.

The dataset is split into training and testing sets using the train_test_split function from scikit-learn, ensuring a stratified split to maintain the distribution of emotions in both sets. Data visualization is performed to explore the class distribution and create word clouds for each emotion.

Three machine learning models—K Nearest Neighbour (KNN) Classifier, Naive Bayes Classifier, and Random Forest Classifier—are trained and evaluated using the TF-IDF vectorization of the processed text. The models' performance is assessed using classification reports, including precision, recall, and F1-score metrics.

A comparison of the models' accuracy is visualized using a bar chart, highlighting the strengths and weaknesses of each model. Confusion matrices provide insights into the models' predictions, showing the true positive, true negative, false positive, and false negative values for each emotion class.

Finally, a pipeline is created to deploy a Random Forest Classifier for predicting emotions in new text data. A sample sentence is processed, and the model predicts the corresponding emotion.
