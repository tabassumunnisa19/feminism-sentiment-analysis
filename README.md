# Social Media Sentiment Intelligence: Feminism Discourse Analysis

## Project Overview
This project analyzes public sentiment surrounding feminism using Twitter data.  
By applying Natural Language Processing (NLP), sentiment analysis, topic modeling, and time-series techniques, the project extracts insights into public opinion, dominant discussion themes, and how sentiment evolves over time.

The project also includes sentiment trend forecasting to project possible future sentiment patterns.

---

## Objectives
- Analyze public sentiment toward feminism
- Classify tweets into Positive, Neutral, and Negative sentiment categories
- Identify key discussion themes using topic modeling
- Examine yearly and monthly sentiment trends
- Smooth sentiment variations to uncover underlying patterns
- Forecast future sentiment trends using time-series modeling

---

## Dataset
- **Source:** Twitter feminism discourse dataset (2018–2019)
- **Format:** CSV
- **Content Includes:**
  - Tweet text
  - Timestamp
  - Engagement metrics (likes, retweets)

---

## Methodology

### 1. Data Loading and Structural Cleaning
- Loaded raw Twitter dataset
- Selected relevant attributes
- Handled missing and invalid values
- Converted date fields to datetime format
- Generated a clean base dataset

### 2. Text Preprocessing
- Converted text to lowercase
- Removed URLs, punctuation, and numeric characters
- Removed stopwords
- Applied lemmatization
- Created a cleaned text corpus suitable for NLP tasks

### 3. Sentiment Analysis
- Applied VADER Sentiment Analyzer
- Generated polarity scores (positive, neutral, negative, compound)
- Classified tweets into Positive, Neutral, and Negative sentiment categories

### 4. Topic Modeling
- Used Latent Dirichlet Allocation (LDA)
- Identified dominant themes in feminism discourse
- Analyzed sentiment distribution across topics

### 5. Sentiment Trend Analysis
- Computed yearly sentiment distribution
- Calculated monthly average sentiment scores
- Visualized sentiment trends over time
- Applied rolling averages to smooth fluctuations

### 6. Sentiment Forecasting
- Implemented ARIMA time-series model
- Forecasted short-term sentiment trends
- Compared historical and forecasted sentiment

---

## Key Analyses Performed
- Yearly sentiment distribution (Positive / Neutral / Negative)
- Monthly average sentiment trend
- Smoothed sentiment trend using rolling averages
- Topic-wise sentiment interpretation
- Short-term sentiment forecasting

---

## Tools and Technologies
- Python
- Pandas, NumPy
- NLTK
- VADER Sentiment Analyzer
- Scikit-learn
- Matplotlib
- Statsmodels (ARIMA)

---

## Project Structure
```plaintext
feminism-sentiment-analysis/
│
├── notebooks/
│   ├── 01_data_loading_and_exploration.ipynb
│   ├── 02_text_preprocessing.ipynb
│   ├── 03_sentiment_analysis.ipynb
│   ├── 04_topic_modeling.ipynb
│   ├── 05_sentiment_trend_analysis.ipynb
│   └── 06_sentiment_forecasting.ipynb
│
├── data/
│   ├── raw/
│   │   └── feminism1.csv
│   └── processed/
│       ├── feminism_clean_base.csv
│       ├── feminism_preprocessed.csv
│       ├── feminism_sentiment_results.csv
│       ├── feminism_sentiment_trend.csv
│       └── feminism_sentiment_forecast.csv
│
├── outputs/
│   └── figures/
│
└── README.md
```

## Results and Insights
- Feminism-related discourse contains a mix of strong positive and negative sentiment
- Certain discussion themes consistently attract negative sentiment
- Public sentiment fluctuates over time rather than remaining static
- Smoothed sentiment trends highlight long-term sentiment direction beyond short-term variations
- Sentiment forecasting indicates potential stabilization or gradual shifts in public opinion

---

## Limitations
- Analysis is based on historical Twitter data from 2018–2019
- Lexicon-based sentiment analysis may not fully capture sarcasm or contextual nuances
- Sentiment forecasting represents trend projection rather than exact prediction

---

## Future Enhancements
- Real-time tweet collection and analysis
- Transformer-based sentiment models (BERT, RoBERTa)
- Interactive dashboards for sentiment visualization
- Multilingual sentiment analysis

## Author
**Tabassum Unnisa**  
Data Science | GenAI | Agentic AI
