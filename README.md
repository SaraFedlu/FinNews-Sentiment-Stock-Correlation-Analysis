# **Financial News Sentiment and Stock Market Analysis**

## **Project Overview**
This project explores the correlation between financial news sentiment and stock market movements using natural language processing (NLP) techniques and statistical analysis. The ultimate goal is to help **Nova Financial Solutions** enhance its predictive analytics capabilities, improving financial forecasting accuracy and operational efficiency.

### **Key Objectives**
1. **Sentiment Analysis**:
   - Perform sentiment analysis on financial news headlines to gauge emotional tone (positive, negative, or neutral).
   - Quantify sentiment scores for each news article.
2. **Correlation Analysis**:
   - Establish statistical correlations between sentiment scores and stock price movements.
   - Analyze how news sentiment impacts stock performance, considering publication dates and times.
3. **Exploratory Data Analysis (EDA)**:
   - Study trends in publication frequency, headline lengths, and publisher contributions.
   - Identify keywords or significant events in the headlines (e.g., "FDA approval," "price target").
4. **Topic Modeling**:
   - Uncover topics in financial news using Latent Dirichlet Allocation (LDA).

---

## **Project Workflow**
### **1. Data Preprocessing**
- Load the dataset containing financial news headlines, publication details, and stock tickers.
- Handle missing data, remove duplicates, and parse publication dates into a usable format.
- Clean and preprocess text data for NLP tasks (e.g., remove stop words, punctuation).

### **2. Exploratory Data Analysis (EDA)**
- Analyze headline lengths and publication trends.
- Identify prolific publishers and their content types.
- Examine how news frequency varies over time and during specific market events.

### **3. Sentiment Analysis**
- Use **VADER**, **TextBlob**, or transformer-based models to assign sentiment scores to headlines.
- Categorize sentiment into positive, negative, or neutral.

### **4. Correlation Analysis**
- Merge sentiment data with stock price movements.
- Analyze statistical relationships between sentiment and stock price changes.

### **5. Topic Modeling**
- Apply LDA to extract significant topics and trends in financial news.

### **6. Visualization**
- Create visualizations to summarize findings:
  - Sentiment distributions.
  - Publication frequency over time.
  - Correlations between sentiment and stock price movements.

---

## **Project Structure**
```
FinNews-Sentiment-Stock-Correlation-Analysis/
│
├── data/
│   ├── raw/raw_analyst_ratings.csv        # Input dataset (headlines, dates, publishers, etc.)
│   ├── finance_data.csv                   # Stock price data (tickers, dates, prices, etc.)
│
├── notebooks/
│   ├── eda.ipynb                 # Exploratory data analysis
│   ├── sentiment_analysis.ipynb  # Sentiment analysis pipeline
│   ├── correlation_analysis.ipynb# Correlation analysis
│   ├── topic_modeling.ipynb      # Topic modeling using LDA
│
├── requirements.txt              # List of Python packages required
├── README.md                     # Project description
```

---

## **Dependencies**
The project requires the following Python packages:

- Data Analysis: `pandas`, `numpy`
- Visualization: `matplotlib`, `seaborn`
- Natural Language Processing:
  - `nltk` (for VADER sentiment analysis)
  - `spacy` (optional, for advanced NLP tasks)
  - `textblob` (for sentiment scoring)
  - `gensim` (for topic modeling)
- Machine Learning: `scikit-learn`, `xgboost` (optional)
- Time Series Analysis: `statsmodels`
- Others: `tqdm`, `requests`, `beautifulsoup4` (optional for scraping)

Install all dependencies using:
```bash
pip install -r requirements.txt
```

---

## **How to Run the Project**
1. **Set Up Environment**:
   - Create and activate a virtual environment:
     ```bash
     python -m venv venv
     source venv/bin/activate  # For Linux/Mac
     .\venv\Scripts\activate   # For Windows
     ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run Analysis Notebooks**:
   - Navigate to the `notebooks/` folder and execute notebooks in the recommended order:
     1. `eda.ipynb` for data exploration.
     2. `sentiment_analysis.ipynb` for sentiment scoring.
     3. `correlation_analysis.ipynb` to analyze stock price relationships.
     4. `topic_modeling.ipynb` for topic detection.



## **Future Scope**
- Fine-tune transformer-based models (e.g., BERT, RoBERTa) for more precise sentiment scoring.
- Incorporate real-time news feeds and stock price data for predictive modeling.
- Experiment with advanced time series forecasting techniques (e.g., ARIMA, Prophet).

---

## **Contributors**
- Sara Fedlu (Project Lead and Data Analyst)

For any inquiries or feedback, please contact sfedlu28@gmail.com.