📈 Stock Market Analysis & Reddit Sentiment Tracker

A Python-based stock market analysis project that combines real-time and historical stock market data with Reddit discussions to explore market activity and investor sentiment.

The project uses financial data APIs, Reddit scraping, stock price visualization, and a Flask web application to collect, organize, and display stock-related information.

🚀 Features
Reddit Data Collection: Collects popular posts from the r/wallstreetbets subreddit using the PRAW library.
Stock Mention Filtering: Organizes Reddit posts based on mentions of selected stocks, including:
Tesla (TSLA)
Apple (AAPL)
Meta (META)
Google (GOOGL)
S&P 500 ETF (SPY)
Stock Market Data: Retrieves historical stock prices and market information using Yahoo Finance.
Candlestick Charts: Visualizes stock price movements using Plotly.
Flask Web Application: Displays stock market information in a web-based table.
Financial Data Integration: Uses Alpha Vantage to retrieve intraday stock market data.
🛠️ Technologies Used
Technology	Purpose
Python	Main programming language
Flask	Web application framework
PRAW	Reddit API integration
yfinance	Stock market data
Alpha Vantage	Intraday financial data
Requests	HTTP requests
Plotly	Stock market visualization
HTML / CSS	Frontend interface
Jupyter Notebook	Development and experimentation
📂 Project Structure
text
FinalProject/
│
├── templates/
│   └── table.html
│
├── Scrapper.py
├── analyze.py
├── YF.py
├── graph.py
├── app.py
├── Jupyter_Code.txt
├── TestDemo.html
├── design.css
├── Scraper info.txt
└── README.md

File Descriptions
File	Description
Scrapper.py	Collects popular Reddit posts from WallStreetBets.
analyze.py	Filters collected Reddit posts according to selected stock symbols.
YF.py	Retrieves stock information and historical prices using Yahoo Finance.
graph.py	Generates interactive candlestick charts using Plotly.
app.py	Runs the Flask application and displays stock market information.
Jupyter_Code.txt	Contains experimental and development code.
design.css	Contains frontend styling.
TestDemo.html	HTML demonstration page.
⚙️ Installation
1. Clone the Repository
bash
git clone https://github.com/dhyeyfarasram/FinalProject.git


Navigate into the project directory:

bash
cd FinalProject

2. Create a Virtual Environment (Recommended)
bash
python -m venv venv


Activate it:

Windows:

bash
venv\Scripts\activate


macOS / Linux:

bash
source venv/bin/activate

3. Install Dependencies

Install the required Python libraries:

bash
pip install flask alpha_vantage requests praw yfinance plotly pandas

🔑 API Configuration

The project uses external APIs to retrieve financial and Reddit data.

Alpha Vantage
Create an account at Alpha Vantage.
Generate an API key.
Configure your API key in the application.
Reddit API
Visit Reddit Apps.
Create a Reddit application.
Obtain your client ID and client secret.
Configure your Reddit API credentials.

Important: Store API credentials in environment variables rather than committing them directly to GitHub.

▶️ Usage

The project consists of several independent Python scripts.

1. Collect Reddit Posts

Run:

bash
python Scrapper.py


This script retrieves popular submissions from r/wallstreetbets and stores post titles and scores in a local text file.

2. Analyze Stock Mentions

Run:

bash
python analyze.py


This script processes the collected Reddit posts and separates them into files based on stock mentions.

3. Retrieve Stock Market Data

Run:

bash
python YF.py


This retrieves stock information and historical market data for the selected companies.

4. Generate Stock Charts

Run:

bash
python graph.py


Enter a stock ticker when prompted.

The application generates an interactive candlestick chart showing stock price movements over the selected historical period.

5. Launch the Flask Web Application

Run:

bash
python app.py


Open your browser and navigate to:

text
http://127.0.0.1:5000/


The Flask application displays stock market information in a sortable table.

📊 Supported Stock Symbols
Company / Asset	Ticker
Tesla	TSLA
Apple	AAPL
Meta	META
Google / Alphabet	GOOGL
S&P 500 ETF	SPY
🔮 Future Improvements

Potential improvements to the project include:

Implement automated Reddit sentiment analysis using NLP.
Build a unified dashboard combining stock prices and Reddit sentiment.
Add interactive historical stock price comparisons.
Expand the list of supported stocks.
Introduce automated data collection and scheduled updates.
Add sentiment visualization and market trend indicators.
Improve error handling and API rate-limit management.
Add configurable stock selection through the web interface.
⚠️ Disclaimer

This project is intended for educational and research purposes only.

The financial information and Reddit discussions collected by this project should not be considered financial advice or investment recommendations.

Stock market data may be delayed, incomplete, or subject to API limitations.

👨‍💻 Author

Dhyey Farasram

GitHub: @dhyeyfarasram

📜 License

No license has currently been specified for this repository. Please contact the repository owner regarding usage and distribution permissions.
