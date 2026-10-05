# Sentiment Analysis using NLP

## 📌 Project Overview

This project performs **Sentiment Analysis on tweets** using Natural Language Processing (NLP) and Machine Learning.

The **Sentiment140 dataset** is used to classify tweets into two categories:

* **Positive**
* **Negative**

The project includes data preprocessing, text cleaning, TF-IDF feature extraction, Logistic Regression, and model evaluation.

## 📂 Dataset

The project uses the **Sentiment140 dataset** downloaded using KaggleHub.

The dataset contains tweet text along with sentiment labels.

### Dataset Columns

* `sentiment` – Sentiment of the tweet
* `id` – Tweet ID
* `date` – Tweet date
* `query` – Query information
* `user` – Username
* `text` – Tweet text

For this project, only the following columns are used:

* `text`
* `sentiment`

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Regular Expressions (re)
* Scikit-learn
* KaggleHub
* NLP
* TF-IDF
* Logistic Regression

## 🔄 Project Workflow

1. Download the Sentiment140 dataset
2. Load the dataset using Pandas
3. Select the required columns
4. Check sentiment values
5. Convert sentiment values into Positive and Negative
6. Check and remove missing values
7. Remove duplicate tweets
8. Analyze sentiment distribution
9. Clean the tweet text
10. Split data into training and testing sets
11. Convert text into numerical features using TF-IDF
12. Train a Logistic Regression model
13. Predict sentiments on test data
14. Evaluate the model using accuracy, confusion matrix, and classification report

## 🧹 Text Preprocessing

The tweets are cleaned before applying machine learning.

The cleaning process includes:

* Converting text to lowercase
* Removing URLs
* Removing usernames
* Removing hashtags
* Removing special characters
* Removing extra spaces
* Removing empty text

## 🔤 TF-IDF

**TF-IDF (Term Frequency-Inverse Document Frequency)** is used to convert text into numerical values that can be understood by the machine learning model.

The project uses:

* Maximum 20,000 features
* English stop words removal
* Unigrams and bigrams using `ngram_range=(1,2)`

## 🤖 Machine Learning Model

### Logistic Regression

Logistic Regression is used to classify tweets as either:

* Positive
* Negative

The dataset is divided into:

* **80% Training Data**
* **20% Testing Data**

The split uses `random_state=42` and `stratify=y`.

## 📊 Model Evaluation

The model performance is evaluated using:

* Accuracy Score
* Confusion Matrix
* Classification Report

These metrics help to understand how well the model predicts the sentiment of tweets.

## 📈 Results

The project successfully processes the Sentiment140 dataset and builds a machine learning model for sentiment classification.

The TF-IDF features are used as input to the Logistic Regression model for predicting tweet sentiment.

## 🚀 How to Run the Project

### 1. Install Required Libraries

```bash
pip install pandas numpy matplotlib scikit-learn kagglehub
```

### 2. Open the Notebook

Open the `.ipynb` file in:

* Google Colab
* Jupyter Notebook
* VS Code

### 3. Run the Notebook

Run the cells step by step to:

* Download the dataset
* Preprocess the tweets
* Train the model
* Make predictions
* Evaluate the model

## 📁 Project Structure

```text
Sentiment-Analysis/
│
├── Copy_of_SA_NLP.ipynb
└── README.md
```

## 🎯 Objective

The main objective of this project is to use **NLP and Machine Learning** to automatically identify whether a tweet expresses a positive or negative sentiment.

## 👩‍💻 Author

**Vaishnavi Rai**

Skills used: Python | NLP | Machine Learning | Pandas | Scikit-learn
