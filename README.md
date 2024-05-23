# phishing-email-classifier

# Phishing Email Detection

Kaggle Dataset - [https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset](https://www.kaggle.com/datasets/subhajournal/phishingemails/data)

The following tasks were performed in the phishing_email_classification.ipynb file

This project aims to build a  machine learning model for detecting phishing emails. It utilizes various natural language processing (NLP) techniques and machine learning algorithms to analyze email text and classify it as either safe or phishing. Below is an outline of the key steps involved in the project:

## 1. Data Loading and Cleaning
The dataset containing email text and corresponding labels (safe or phishing) is loaded and cleaned to remove any missing values. A subset of the data (10,000 rows) is sampled for model building.

## 2. Exploratory Data Analysis (EDA)
Feature extraction is performed to gain insights into the characteristics of the email text. This includes analyzing the length, complexity, and structure of emails to identify patterns related to the target variable (safe or phishing). Visualizations such as histograms, word clouds, and common word histograms provide a deeper understanding of the data.

## 3. Data Preprocessing
Text preprocessing techniques are applied, including converting text to lowercase, tokenization, removing special characters, stopwords, and punctuation, and stemming. These steps prepare the text data for further analysis and model building.

## 4. Model Building
The preprocessed text data is transformed into numerical features using TF-IDF vectorization. Various machine learning classifiers, including Naive Bayes, Support Vector Machine (SVM), Logistic Regression, Random Forest, AdaBoost, Gradient Boosting, and XGBoost, are trained and evaluated using k-fold cross-validation. Performance metrics such as accuracy and precision are calculated to assess the effectiveness of each classifier.

## 5. Model Evaluation and Visualization
The performance of each classifier is visualized using a bar chart, highlighting their accuracy and precision scores. This allows for easy comparison and selection of the most effective classifier for phishing email detection.

## 6. Ensemble Learning
Ensemble learning techniques such as Voting Classifier and Stacking Classifier are employed to further enhance model performance. These techniques combine the predictions of multiple base classifiers to improve overall accuracy and precision.

## 7. Model Deployment
Trained models and vectorizers are serialized using the `pickle` library and saved as binary files (`vectorizer.pkl` and `model.pkl`). This allows for easy deployment and reuse of the models for future email classification tasks.
