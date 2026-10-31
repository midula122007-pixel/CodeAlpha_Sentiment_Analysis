# Sentiment Analysis Using Machine Learning and NLP

A Python-based sentiment analysis project developed as part of the **CodeAlpha Data Analytics / Python Internship – Task 4**.

This project analyzes customer reviews from Amazon, IMDb, and Yelp using Natural Language Processing (NLP), Logistic Regression, and VADER sentiment analysis.

## Project Overview

The system classifies customer reviews into:
- Positive
- Negative
- Neutral (VADER only)

It also generates visualizations to understand sentiment patterns and model performance.

## Dataset

**UCI Sentiment Labelled Sentences Dataset**

| Dataset | Number of Reviews |
|---|---:|
| Amazon | 1,000 |
| IMDb | 1,000 |
| Yelp | 1,000 |
| **Total** | **3,000** |

- Positive reviews: 1,500
- Negative reviews: 1,500

## Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- NLTK
- Scikit-learn
- WordCloud
- Jupyter Notebook

## Project Structure

```text
G-Task-3/
│
├── dataset/
│   ├── sentiment labelled sentences/
│   │   ├── amazon_cells_labelled.txt
│   │   ├── imdb_labelled.txt
│   │   ├── yelp_labelled.txt
│   │   └── readme.txt
│   ├── combined_sentiment_dataset.csv
│   └── sentiment_analysis_results.csv
│
├── notebooks/
│
├── reports/
│
├── visualizations/
│   ├── confusion_matrix.png
│   ├── sentiment_distribution.png
│   ├── source_sentiment.png
│   ├── positive_wordcloud.png
│   ├── negative_wordcloud.png
│   ├── vader_sentiment_distribution.png
│   └── vader_comparison.png
│
├── src/
│
├── sentiment_analysis.ipynb
└── README.md
```

## Project Workflow

1. Load and combine the Amazon, IMDb, and Yelp datasets.
2. Explore the dataset and inspect missing values and duplicates.
3. Clean and preprocess review text.
4. Convert text into numerical features using TF-IDF.
5. Train a Logistic Regression classifier.
6. Evaluate the classifier using accuracy, classification report, and confusion matrix.
7. Generate positive and negative word clouds.
8. Perform VADER sentiment analysis.
9. Compare VADER predictions with original sentiment labels.
10. Test the trained model using custom reviews.

## Results

### Logistic Regression

| Metric | Result |
|---|---:|
| Accuracy | **83.50%** |
| Training reviews | 2,400 |
| Testing reviews | 600 |

### VADER

| Metric | Result |
|---|---:|
| Total reviews | 3,000 |
| Non-neutral predictions | 2,330 |
| Neutral predictions | 670 |
| Binary accuracy on non-neutral reviews | **85.92%** |

*Note: Logistic Regression and VADER were evaluated on different sets of reviews. Their accuracy values are not directly comparable.*

## Visualizations

Generated charts are available in the `visualizations/` directory:

- Confusion matrix
- Overall sentiment distribution
- Source-wise sentiment distribution
- Positive word cloud
- Negative word cloud
- VADER sentiment distribution
- VADER comparison heatmap

## Installation

Clone the repository:

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd G-Task-3
```

Create a virtual environment:

```bash
python -m venv .venv
```

Activate it on Windows:

```powershell
.venv\Scripts\Activate.ps1
```

Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn nltk scikit-learn wordcloud jupyter ipykernel
```

Download the required NLTK resources by running:

```python
import nltk

nltk.download("stopwords")
nltk.download("wordnet")
nltk.download("omw-1.4")
nltk.download("vader_lexicon")
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open `sentiment_analysis.ipynb` and run the cells in order.

## Learning Outcomes

- Data loading and preprocessing with Pandas.
- Text cleaning and lemmatization using NLTK.
- TF-IDF feature extraction.
- Sentiment classification using Logistic Regression.
- Evaluation of classification models.
- Rule-based sentiment analysis using VADER.
- Data visualization using Matplotlib and Seaborn.
- Word cloud generation.

## Acknowledgement

Developed as part of the **CodeAlpha Internship – Task 4: Sentiment Analysis**.

Dataset source: UCI Machine Learning Repository – Sentiment Labelled Sentences.

---

**Author:** Adhithya  
**Project:** Sentiment Analysis  
**Language:** Python
