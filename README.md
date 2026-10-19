# Sentiment_Analysis

## 📌 Project Overview

This project focuses on classifying human emotions from text using Natural Language Processing (NLP) and machine learning techniques. The system takes a sentence as input and predicts the emotion expressed in that sentence.

Two machine learning algorithms, **Naive Bayes** and **Support Vector Machine (SVM)**, are trained and evaluated to determine which model performs better for emotion classification.

## 🎯 Objectives

- Load and explore the text dataset.
- Clean and preprocess textual data.
- Perform tokenization and stopword removal.
- Convert text into numerical features using TF-IDF.
- Train Naive Bayes and SVM classifiers.
- Evaluate the models using accuracy, precision, recall, and F1-score.
- Predict emotions for new sentences.
- Compare the performance of both models.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- NLTK
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## 📂 Project Structure

```text
Emotion-Classification/
│
├── nlp_dataset.csv
├── emotion_classification.ipynb
├── README.md
└── requirements.txt
```

*Note: Update the filenames to match your actual project files.*

## 📊 Project Workflow

### 1. Data Loading and Exploration

The dataset is loaded using Pandas and examined to understand its structure, columns, missing values, and emotion labels.

### 2. Text Preprocessing

The following preprocessing techniques are applied:

- **Text cleaning:** Removes unwanted characters and unnecessary symbols.
- **Lowercasing:** Converts text to lowercase for consistency.
- **Tokenization:** Splits sentences into individual words or tokens.
- **Stopword removal:** Removes common words that may contribute less to classification, depending on the context.

These steps help standardize text before feature extraction.

### 3. Feature Extraction

TF-IDF (Term Frequency–Inverse Document Frequency) is used to convert text into numerical feature vectors.

TF-IDF assigns weights to words based on their importance in a document relative to the dataset. These numerical representations are used as input to the machine learning models.

### 4. Model Development

Two classification algorithms are implemented:

- **Naive Bayes:** A probabilistic algorithm that uses Bayes' theorem to classify text based on learned word patterns.
- **Support Vector Machine (SVM):** A supervised learning algorithm that learns decision boundaries to distinguish between emotion classes.

### 5. Model Evaluation

Both models are evaluated using the following metrics:

- **Accuracy:** Measures the proportion of correctly classified samples.
- **Precision:** Measures how often predictions for a particular class are correct.
- **Recall:** Measures how many actual instances of a class are identified correctly.
- **F1-score:** Combines precision and recall into a single metric.

## 📈 Model Performance

The models achieved the following results on the test dataset:

| Evaluation Metric | Naive Bayes | SVM |
|---|---:|---:|
| Accuracy | 89.96% | 93.60% |
| Precision (weighted) | 90.09% | 93.61% |
| Recall (weighted) | 89.96% | 93.60% |
| F1-score (weighted) | 89.96% | 93.60% |

### Best Performing Model

**Support Vector Machine (SVM)** performed better than Naive Bayes across all reported evaluation metrics.

SVM achieved an accuracy of 93.60%, making it the preferred model among the two classifiers evaluated for this project.

## 🔍 Emotion Prediction

The trained SVM model can predict the emotion associated with a new sentence.

Example input:

```text
I am afraid of walking alone in the dark.
```

Example prediction:

```text
Predicted Emotion: Fear
```

The predicted output depends on the trained model and the emotion categories in the dataset.

## 🚀 How to Run the Project

1. Clone or download the project repository.
2. Install the required Python libraries.
3. Open `emotion_classification.ipynb` in Jupyter Notebook or Google Colab.
4. Place `nlp_dataset.csv` in the appropriate directory.
5. Run the notebook cells in order to preprocess the data, extract features, train the models, and evaluate performance.
6. Enter a new sentence to test emotion prediction.

## 📦 Installation

Install the required libraries using:

```bash
pip install pandas numpy scikit-learn nltk matplotlib seaborn jupyter
```

If your notebook uses additional libraries, install those as well.

## 🔮 Future Enhancements

- Improve performance on less frequent emotion classes.
- Experiment with additional machine learning algorithms.
- Analyze confusion matrices and per-class classification reports.
- Build an interactive web application for real-time emotion prediction.
- Explore advanced NLP techniques for improved contextual understanding.

## 📝 Conclusion

This project demonstrates how NLP preprocessing and TF-IDF feature extraction can be combined with machine learning algorithms to classify emotions from text. Both Naive Bayes and SVM achieved strong evaluation results, with SVM performing best at 93.60% accuracy.

The project provides a foundation for text-based emotion analysis and can be extended into interactive applications.

---

**Project Type:** Machine Learning / Natural Language Processing  
**Task:** Text Emotion Classification  
**Best Model:** Support Vector Machine (SVM)  
**Best Test Accuracy:** 93.60%
