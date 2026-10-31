# CodeAlpha Task 4 – Sentiment Analysis

A Machine Learning and Natural Language Processing project that analyzes customer reviews and classifies them as Positive or Negative using Logistic Regression and VADER sentiment analysis.

## Project Overview

This project uses Natural Language Processing (NLP) techniques to understand customer opinions from text reviews collected from Amazon, IMDb, and Yelp.

The system performs text preprocessing, feature extraction, sentiment classification, model evaluation, and visualization.

## Dataset

**UCI Sentiment Labelled Sentences Dataset**

- Total reviews: 3,000
- Amazon: 1,000 reviews
- IMDb: 1,000 reviews
- Yelp: 1,000 reviews
- Sentiment labels: 0 (Negative), 1 (Positive)

## Technologies Used

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- NLTK
- Scikit-learn
- TF-IDF
- Logistic Regression
- VADER
- WordCloud
- Jupyter Notebook

## Project Workflow

1. Dataset loading and exploration
2. Exploratory Data Analysis (EDA)
3. Text cleaning and preprocessing
4. Stopword removal and lemmatization
5. TF-IDF feature extraction
6. Train-test splitting (80:20)
7. Logistic Regression model training
8. Model evaluation
9. VADER sentiment analysis
10. Word cloud generation
11. Custom review sentiment prediction

## Model Performance

**Logistic Regression**

- Evaluation: 80% training / 20% testing
- Test samples: 600
- Previously measured accuracy: 83.50%

**VADER**

- Rule-based sentiment analysis
- Categories: Positive, Negative, Neutral
- Previously measured binary accuracy: 85.92% among non-neutral predictions

Note: The Logistic Regression and VADER accuracy figures use different evaluation procedures and should not be interpreted as a direct model comparison.

## Visualizations

The project generates:

- Sentiment distribution
- Source-wise sentiment distribution
- Confusion matrix
- Positive review word cloud
- Negative review word cloud
- VADER sentiment distribution
- VADER comparison heatmap

Visualizations are available in the `visualizations/` directory.

## Project Structure

```text
G-Task-3/
│
├── .gitignore
├── README.md
├── dataset/
│   ├── combined_sentiment_dataset.csv
│   ├── sentiment_analysis_results.csv
│   └── sentiment labelled sentences/
│
├── notebooks/
│   └── sentiment_analysis.ipynb
│
├── reports/
│
└── visualizations/
```

## Installation and Execution

Clone the repository:

```bash
git clone https://github.com/adhithyavasan5-tech/CodeAlpha_Sentiment_Analysis.git
cd CodeAlpha_Sentiment_Analysis
```

Create and activate a virtual environment:

```bash
python -m venv .venv
```

Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn nltk scikit-learn wordcloud notebook
```

Download NLTK resources:

```python
import nltk

nltk.download('stopwords')
nltk.download('wordnet')
nltk.download('omw-1.4')
nltk.download('vader_lexicon')
```

Launch Jupyter:

```bash
jupyter notebook
```

Open `notebooks/sentiment_analysis.ipynb` and run the cells.

## Learning Outcomes

- Practical experience with NLP.
- Text preprocessing and feature extraction.
- Machine learning classification.
- Model evaluation and visualization.
- Rule-based sentiment analysis.

## Acknowledgement

This project was completed as part of the **CodeAlpha Internship – Task 4: Sentiment Analysis**.

Dataset: UCI Machine Learning Repository – Sentiment Labelled Sentences.

## Author

**Adhithya**

GitHub: [adhithyavasan5-tech](https://github.com/midula122007-tech)
