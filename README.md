# 🪙 Cryptocurrency Market Data Collection & Analysis

<p align="center">
  <b>🌐 API • 🐍 Python • 🐼 Pandas • 🔢 NumPy • 📊 Data Analysis</b>
</p>

<p align="center">
  <i>Collecting real-time cryptocurrency market data using the CoinGecko API</i>
</p>

---

## 📌 Project Overview

This project collects cryptocurrency market data using the **CoinGecko API** and processes the response using **Python, Pandas, and NumPy**.

The project demonstrates how to:

* 🌐 Connect to a cryptocurrency API
* 🔐 Authenticate API requests using an API key
* 📥 Fetch cryptocurrency market data
* 🐼 Convert API JSON data into a Pandas DataFrame
* 🔍 Explore the collected dataset
* 🧹 Clean and prepare data for analysis
* 📊 Work with cryptocurrency market indicators

The project currently retrieves **100 cryptocurrency records with 26 columns** from the API.

---

## 🛠️ Technologies Used

| Technology          | Purpose                        |
| ------------------- | ------------------------------ |
| 🐍 Python           | Programming language           |
| 🌐 Requests         | Sending API requests           |
| 🐼 Pandas           | Data manipulation and analysis |
| 🔢 NumPy            | Numerical operations           |
| 🪙 CoinGecko API    | Cryptocurrency market data     |
| 📓 Jupyter Notebook | Development environment        |

---

## 🔄 Project Workflow

```text
        🪙 CoinGecko API
               ↓
        🔐 API Authentication
               ↓
        📡 Send API Request
               ↓
          📥 Receive JSON
               ↓
       🐼 Create DataFrame
               ↓
         🔍 Explore Data
               ↓
        🧹 Data Cleaning
               ↓
        📊 Data Analysis
               ↓
       🚀 Future Visualization
```

---

## 🌐 API Data Collection

The project uses the CoinGecko cryptocurrency markets endpoint:

```python
url = "https://api.coingecko.com/api/v3/coins/markets"
```

The API request uses parameters such as:

```python
params = {
    "vs_currency": "usd",
    "order": "market_cap_desc",
    "per_page": 100,
    "page": 1
}
```

The API key is passed through the request header:

```python
headers = {
    "x-cg-demo-api-key": api_key
}
```

The response is then converted from JSON into a Pandas DataFrame.

---

## 📊 Dataset

The collected dataset contains **100 rows and 26 columns**.

Some important fields include:

* `id`
* `symbol`
* `name`
* `current_price`
* `market_cap`
* `market_cap_rank`
* `fully_diluted_valuation`
* `total_volume`
* `high_24h`
* `low_24h`
* `price_change_24h`
* `price_change_percentage_24h`
* `market_cap_change_24h`
* `market_cap_change_percentage_24h`
* `circulating_supply`
* `total_supply`
* `max_supply`
* `ath`
* `ath_change_percentage`
* `ath_date`
* `atl`
* `atl_change_percentage`
* `atl_date`
* `last_updated`

---

## 🪙 Example Cryptocurrencies

The API response includes cryptocurrencies such as:

```text
₿ Bitcoin
♦️ Ethereum
💵 Tether
🟡 BNB
💧 XRP
```

The data is ordered by **market capitalization**.

---

## 🔍 Data Exploration

The project checks the structure and size of the collected data using Pandas.

Example:

```python
df.shape
```

Output:

```text
(100, 26)
```

The first records can be viewed using:

```python
df.head()
```

---

## 🧹 Data Cleaning

The next stage of the project focuses on preparing the cryptocurrency data for analysis.

Possible cleaning tasks include:

* 🔎 Checking missing values
* ♻️ Detecting duplicate records
* 🔢 Checking data types
* 🚫 Identifying invalid values
* 📅 Converting date columns
* 🗑️ Removing unnecessary columns
* 📊 Preparing numerical columns for analysis

---

## 🔐 API Key Security

**⚠️ Important:** Never publish your real API key on GitHub.

Instead of putting your API key directly into your public notebook, use an environment variable or `.env` file.

Example:

```python
import os

api_key = os.getenv("COINGECKO_API_KEY")
```

Add `.env` to your `.gitignore`:

```gitignore
.env
```

If you accidentally publish your API key, revoke or rotate it immediately.

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone YOUR_REPOSITORY_URL
```

### 2. Open the project

```bash
cd cryptocurrency-data-analysis
```

### 3. Install required libraries

```bash
pip install requests pandas numpy jupyter
```

### 4. Configure your API key

Set your CoinGecko API key as an environment variable.

### 5. Start Jupyter Notebook

```bash
jupyter notebook
```

### 6. Run the notebook

Run the cells from top to bottom to:

**Connect → Collect → Convert → Explore → Clean → Analyze**

---

## 📈 Future Improvements

I plan to extend this project with:

* 📊 Cryptocurrency price visualization
* 🏆 Top 10 cryptocurrencies by market cap
* 💰 Market capitalization analysis
* 📈 24-hour price change analysis
* 🔥 Top gainers and losers
* 📉 Trading volume analysis
* 🔗 Correlation analysis
* 📊 Interactive dashboard using Power BI/Streamlit
* 🤖 Cryptocurrency price prediction
* 🧠 Machine Learning models

---

## 🎯 Learning Outcomes

Through this project, I practiced:

```text
🐍 Python
        ↓
🌐 API Integration
        ↓
🔐 API Authentication
        ↓
📥 JSON Data Collection
        ↓
🐼 Pandas
        ↓
🔢 NumPy
        ↓
🧹 Data Cleaning
        ↓
📊 Data Analysis
```

This project helped me understand how **real-world data can be collected directly from an API and transformed into a structured dataset for Data Science analysis.**

---

## 👨‍💻 About Me

### Gokul Chandra Swain

🎓 BCA Graduate
📊 Aspiring Data Scientist
🐍 Python
🐼 Pandas
🔢 NumPy
📈 Data Analysis
📊 Statistics
🤖 Machine Learning

I am currently building practical Data Science projects and developing my skills in **Python, Data Analysis, Statistics, SQL, and Machine Learning**.

---

## ⭐ Project Status

| Component             | Status         |
| --------------------- | -------------- |
| 🌐 API Connection     | ✅ Completed    |
| 🔐 API Authentication | ✅ Completed    |
| 📥 Data Collection    | ✅ Completed    |
| 🐼 DataFrame Creation | ✅ Completed    |
| 🔍 Data Exploration   | 🔄 In Progress |
| 🧹 Data Cleaning      | 🔄 In Progress |
| 📊 Visualization      | 🚀 Planned     |
| 🤖 Machine Learning   | 🚀 Future      |

---

## ⭐ Support

If you find this project useful or interesting, consider giving the repository a ⭐ **Star**!

<p align="center">
  <b>🚀 Learn • Build • Analyze • Repeat 📊</b>
</p>
