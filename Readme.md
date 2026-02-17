🚀 AI Day Trader Bot

This project is an automated AI-powered trading assistant built using n8n that analyzes stock/crypto symbols, evaluates real-time market data, checks recent news sentiment, and provides actionable Buy/Sell/Hold trade recommendations via Telegram.

📊 Features

✔ Telegram-based symbol input
✔ Fetch real-time candle data (1min, 15min, 1hr)
✔ News sentiment analysis using AI
✔ Technical + Sentiment combined decision
✔ Automatic trade recommendation
✔ Entry Price, Stop Loss, Target Price suggestions
✔ Error handling for invalid symbols

🧠 How It Works
1️⃣ User sends symbol in Telegram

Example:

AAPL
BTC/USD
TSLA

2️⃣ Bot Fetches Market Data

Using API from
👉 Twelve Data

It collects:

1 Minute candles

15 Minute candles

1 Hour candles

3️⃣ News Sentiment Analysis

Using API from
👉 NewsAPI

Then AI analyzes sentiment using OpenAI model.

Output:

Positive / Neutral / Negative

Sentiment Score

4️⃣ AI Trade Decision

Using OpenAI Agent:

Bot analyzes:

Technical candles

Market trend

News sentiment

Then sends:

BUY / SELL / HOLD
Entry Price
Stop Loss
Target Price

5️⃣ Result Sent to Telegram

User instantly receives trading recommendation.

🛠 Tech Stack

n8n Automation

Telegram Bot API

TwelveData Market API

NewsAPI

OpenAI GPT Models

JavaScript Code Node

📂 Workflow Architecture

Telegram Trigger
→ Market Data APIs
→ News Sentiment AI
→ Data Aggregation
→ AI Trading Agent
→ Telegram Output

⚙️ Setup Instructions
1️⃣ Install n8n
npm install n8n -g


Or use Docker.

2️⃣ Import Workflow

Open n8n

Import JSON file

Add API keys

3️⃣ Required API Keys

TwelveData API Key

NewsAPI Key

OpenAI API Key

Telegram Bot Token

4️⃣ Start Bot

Send stock symbol to Telegram bot.

📈 Example Output
Technical Recommendation FOR AAPL:
BUY
Entry Price: 188.20
Stop-Loss: 183.50
Target Price: 195.00

⚠️ Disclaimer

This bot provides educational trading signals only.
Not financial advice.

👨‍💻 Author

Muhammad Sohaib
Data Analyst | Automation Expert | AI Developer