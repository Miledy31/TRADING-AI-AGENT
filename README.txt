TRADING AI DASHBOARD V1.1

Files:
- Trading_Dashboard_V1_1.xlsx  = dashboard/scanner/journal
- update_trading_dashboard.py  = market-data updater
- requirements.txt             = Python dependencies

IMPORTANT:
This is a PAPER-TRADING prototype. It does not place real orders.

DATA:
- Stocks/ETFs: Alpha Vantage
- Crypto: CoinGecko

SETUP:
1. Install Python 3.10+.
2. Open a terminal in this folder.
3. Run: pip install -r requirements.txt
4. Get your own API keys from the providers.
5. Set environment variables:
   ALPHAVANTAGE_API_KEY
   COINGECKO_API_KEY
6. Run:
   python update_trading_dashboard.py

The updater calculates a simple rule-based score from price, SMA20, SMA50,
RSI, momentum, and volume where available. The score is a screening aid,
not a prediction or guarantee.

For U.S. stocks, Alpha Vantage's intraday endpoint and realtime/15-minute
delayed entitlements may require a premium plan. Daily historical data is
suitable for the first prototype.
