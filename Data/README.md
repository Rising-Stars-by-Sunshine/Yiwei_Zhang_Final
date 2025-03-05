This data folder contains financial-domain-focused datasets for financial sentiment/emotion classification and stock market time series prediction. The first is an open access dataset comes from the paper: [StockEmotions: Discover Investor Emotions for Financial Sentiment Analysis and Multivariate Time Series](https://arxiv.org/abs/2301.09279) accepted by AAAI 2023 Bridge (AI for Financial Services). The second dataset also comes from this paper and contains 38 companies histrical price data from Yahoo finance. 
> Lee, Jean, Hoyoul Luis Youn, Josiah Poon, and Soyeon Caren Han. “StockEmotions: Discover Investor Emotions for Financial Sentiment Analysis and Multivariate Time Series.” arXiv, February 6, 2023. https://doi.org/10.48550/arXiv.2301.09279.



## Key statistics of the data<img width="1028" alt="截屏2025-02-24 08 58 54" src="https://github.com/user-attachments/assets/f0af49f2-565c-4b17-b457-cb6fbf9683dd" />

- Data collection period : **Jan 2020 - Dec 2020**
- Number of Utterance : **10,000**  (train 80%, val 10%, test 10%)
- Sentiment classes: 2 annotated by users 
    - **bullish** (~positive), **bearish** (~negative)
- Emotion classes: 12 annotated by Human & AI collaboration
    - **ambiguous, amusement, anger, anxiety, belief, confusion, depression, disgust, excitement, optimism, panic, surprise** 

## Data explained
- tweet data: train_stockemo.csv
    - **train_stockemo.csv** : In total, 8000 samples. The file has id, date, ticker, emo_label, senti_lable, original, and processed content. For the data curation, processing (e.g. emoji, CTAG, HTAG), and annotation, we refer to our paper. The dataset is used for Financial Sentiment/Emotion Classification tasks.
    - [Download the dataset](https://github.com/Rising-Stars-by-Sunshine/Yiwei_Zhang_Final/blob/main/Data/merged_stock_prices.csv)

## Data Dictionary for train_stockemo.csv

The dataset contains stock market sentiment and emotion analysis data with the following columns:

# 📌 Data Dictionary for `train_stockemo.csv`

The **`train_stockemo.csv`** dataset contains sentiment data related to stock market discussions. Each row represents a **timestamped sentiment entry** associated with a specific stock.

## 📊 Dataset Overview

| **Column Name**  | **Data Type** | **Description** |
|-----------------|------------|----------------|
| `id`           | `int`      | Unique identifier for each sentiment entry. |
| `date`         | `datetime` | Date of sentiment capture (`YYYY-MM-DD` format). |
| `ticker`       | `str`      | Stock ticker symbol associated with the sentiment (e.g., `AAPL`, `TSLA`). |
| `emo_label`    | `str`      | Emotion category assigned to the sentiment (e.g., *Optimism, Panic, Amusement*). |
| `senti_label`  | `str`      | Broad sentiment classification (`bullish` or `bearish`). |
| `original`     | `str`      | Raw text data from which sentiment was derived. |
| `processed`    | `str`      | Cleaned and preprocessed text data (stopwords removed, standardized formatting). |

---

## 📂 Sample Data (First Two Rows)

| `id`    | `date`       | `ticker` | `emo_label` | `senti_label` | `original` | `processed` |
|--------|------------|---------|------------|--------------|------------|------------|
| 100001 | 2020-01-01 | AAPL    | Excitement | Bullish      | "$AAPL skyrocketing 🚀" | "Apple skyrocketing" |
| 100002 | 2020-01-02 | TSLA    | Panic      | Bearish      | "$TSLA crashing hard 😱" | "Tesla crashing hard" |
This dataset can be used for financial sentiment/emotion classification and stock market time series prediction.

## Historical Price Data
price data: price_raw data.zip, merged_stock_prices.csv. 
- **38 companies histrical price data in the zip file** in csv format. The tweet and price dataset together are used for Multivariate Time Series tasks. 
- Tickers: 
        'AAPL', 'ABNB', 'AMT', 'AMZN', 'BA', 'BABA', 'BAC', 'BKNG', 'BRK.A', 'BRK.B', 'CCL', 'CVX',
        'DIS', 'FB', 'GOOG', 'GOOGL', 'HD', 'JNJ', 'JPM', 'KO', 'LOW', 'MA', 'MCD', 'MSFT', 'NFLX',
        'NKE', 'NVDA', 'PFE', 'PG', 'PYPL', 'SBUX', 'TM', 'TSLA', 'TSM', 'UNH', 'UPS', 'V', 'WMT', 'XOM'
        - 'FB' ticker is changed to 'META', but the time at the data collection was 'FB'.
## Data Dictionary for merged_stock_price.csv

The dataset contains historical stock price data with the following columns:

| Column Name  | Data Type  | Description  |
|-------------|------------|-----------------------------------------------|
| Date        | String     | Date of the stock price record |
| Open        | float      | Opening price of the stock on the given date |
| High        | float      | Highest price reached during the trading day |
| Low         | float      | Lowest price reached during the trading day |
| Close       | float      | Closing price of the stock on the given date |
| Adj Close   | float      | Adjusted closing price accounting for splits and dividends |
| Volume      | integer    | Number of shares traded during the day |
| Stock       | String     | Stock ticker symbol |

## Sample Data

Below is a preview of the dataset:

| Date       | Open  | High  | Low   | Close | Adj Close | Volume  | Stock |
|------------|------:|------:|------:|------:|----------:|--------:|-------|
| 2019-12-31 | 325.41 | 326.57 | 323.32 | 325.76 | 323.83 | 4,958,800 | BA |
| 2020-01-02 | 328.55 | 333.35 | 327.70 | 333.32 | 331.35 | 4,544,400 | BA |

This table provides an overview of the dataset's structure, which can be used for further analysis and modeling.

## Note

The datasets are inspired by and builds upon research in financial sentiment and investor emotions. For more details, refer to:
Lee, Jean, Hoyoul Luis Youn, Josiah Poon, and Soyeon Caren Han.  
["StockEmotions: Discover Investor Emotions for Financial Sentiment Analysis and Multivariate Time Series."](https://doi.org/10.48550/arXiv.2301.09279)  
*arXiv, February 6, 2023*.

