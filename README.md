# BrainWave_Matrix_Intern_Task2

# Social Media Sentiment Analysis with VADER (NLP Project)

This project performs sentiment analysis on synthetic social media posts using NLP techniques and the VADER sentiment analyzer. The goal is to understand public sentiment trends by analyzing social text and visualizing sentiment distribution.

---

## Dataset

I used the **Social Media Sentiments Analysis** dataset from Kaggle, which includes synthetic posts from platforms like Reddit and Twitter.

🔗 Dataset link: [Social Media Sentiments Analysis on Kaggle](https://www.kaggle.com/datasets/ravishah912/social-media-sentiments-analysis)

---

## Files in This Repository

| File                         | Description |
|-----------------------------|-------------|
| `Train.csv`                 | Labeled dataset with social media text and sentiment. |
| `Test.csv`                  | Test dataset without labels. |
| `Sentiment_Analysis.ipynb` | Jupyter Notebook with full analysis (Colab-ready). |
| `Train_with_Predicted_Sentiment.csv` | Output with predicted sentiment labels. |
| `README.md`                | This file. |

---

## Tools & Libraries Used

- **Python** 3.11+
- **Pandas** for data handling
- **NLTK** for stopwords and VADER sentiment scoring
- **Seaborn & Matplotlib** for visualizations
- **RegEx** for text preprocessing
- **Google Colab** for cloud execution

---

## Data Preprocessing

1. Removed URLs, mentions, hashtags
2. Lowercased all text
3. Removed punctuation and stopwords using NLTK
4. Applied VADER sentiment analysis to generate a `compound` score

---

## Sentiment Classification Logic

- **Positive** if `compound > 0.05`
- **Negative** if `compound < -0.05`
- **Neutral** otherwise

---

## Visualizations

- **Pie Chart**: Proportion of predicted sentiment
- **Bar Chart**: Count of each sentiment class

---

## Output

Final output file: `Train_with_Predicted_Sentiment.csv` contains original text and predicted sentiment labels.

---

## How to Run

1. Open `Sentiment_Analysis.ipynb` in **Google Colab**
2. Upload `Train.csv` and `Test.csv` via the Colab file uploader
3. Run all cells to clean, analyze, visualize, and export sentiment predictions

---

