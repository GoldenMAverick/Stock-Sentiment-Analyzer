
# Reddit Stock Sentiment Analyzer

A machine learning project that uses **natural language processing (NLP)** to analyze Reddit sentiment around stocks and correlate it with real-time stock price movements. The goal is to understand the impact of crowd sentiment on the financial markets — especially from influential Reddit communities like r/WallStreetBets, r/stocks, and others.

---

## 🚀 Features

- 📅 **Data Collection**: Scrapes Reddit posts and comments using the Reddit API (PRAW or Pushshift).
- 🧠 **Sentiment Analysis**: Uses NLP models (e.g., VADER, TextBlob, or transformer-based models like BERT) to determine the sentiment (positive/negative/neutral) of each post or comment.
- 📈 **Stock Price Integration**: Pulls historical stock price data using APIs like Yahoo Finance or Alpha Vantage.
- 📊 **Correlation Engine**: Compares sentiment trends with actual stock performance to identify leading indicators or lags.
- 🗓 **Time-Series Analysis**: Visualizes sentiment vs. stock price movement over time.
- 📦 **Modular Pipeline**: Each step (scraping, analysis, visualization) is modular for easy customization and reuse.

---

## 🧰 Tech Stack

- **Languages**: Python
- **NLP**: NLTK, VADER, TextBlob, spaCy, or HuggingFace Transformers
- **Data Visualization**: Matplotlib, Seaborn, Plotly
- **APIs**: Reddit API (PRAW / Pushshift), Yahoo Finance (`yfinance`), or Alpha Vantage
- **Storage**: Pandas DataFrames, CSV, or SQLite
- **Scheduling**: Optional cron jobs or scripts for regular scraping

---

## 📁 Project Structure

```
Reddit-Stock-Sentiment-Analyzer/
│
├── data/                 # Collected Reddit & stock data
├── notebooks/            # Jupyter notebooks for EDA and modeling
├── src/
│   ├── reddit_scraper.py     # Reddit data collection
│   ├── sentiment_analyzer.py # NLP-based sentiment scoring
│   ├── stock_data.py         # Fetches historical stock prices
│   ├── correlation.py        # Compares sentiment & stock prices
│   └── visualizer.py         # Plots and dashboards
├── requirements.txt
└── README.md
```

---

## 🔍 Example Use Case

1. **Monitor GME sentiment** from Reddit between Jan–Mar 2021.
2. **Visualize spikes** in positive sentiment and compare them with real price jumps.
3. **Quantify correlation**: “Did positive sentiment lead price movement by 1–2 days?”
4. **Predictive Insight**: Explore whether current sentiment can forecast near-future price action.

---

## 📊 Sample Visualization

- Sentiment scores vs. time
- Stock closing price overlay
- Daily volume of posts/comments mentioning a stock
- Word clouds of most common bullish/bearish phrases

---

## 🔒 Disclaimer

This project is for **educational and research purposes only**. It does **not constitute financial advice**. Trading stocks involves risk, and sentiment is only one of many influencing factors.

---

## 📌 Future Improvements

- Real-time sentiment dashboard using Streamlit or Dash
- Incorporate deep learning models (e.g., RoBERTa) for better sentiment accuracy
- Automate alerts when sentiment diverges from price trend
- Add Twitter and news data for a multi-source analysis

---

## 🤝 Contributions

Pull requests, bug reports, and suggestions are welcome! Please open an issue first before making large changes.
