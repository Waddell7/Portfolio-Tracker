Portfolio Tracker

A self-contained, browser-based investment portfolio tracker. No sign-up, no server, no subscriptions
Built for Australian investors but works for any portfolio with support for multiple currencies, asset types, and exchanges.

---

## Features

- **Live prices** — stocks and ETFs via Yahoo Finance, crypto via CoinGecko
- **Multi-currency** — AUD, USD, GBP, EUR, JPY, CAD and more, with full FX gain/loss tracking
- **Asset types** — Stocks, ETFs, and Cryptocurrency
- **Long & short positions**
- **Margin trading** — track positions with a margin deposit rather than full cost basis
- **Sales tracking** — record partial or full sales with locked-in P&L at the time of sale
- **Dividends** — record dividend payments with franking credit support (Australian investors)
- **Performance chart** — interactive chart with timeframe filters (5D, 1M, 3M, 6M, YTD, 1Y, MAX), hover to inspect, and click-drag to compare any two points in time
- **Benchmark comparison** — overlay ASX 200 or S&P 500 (AUD-adjusted) on the performance chart
- **Portfolio breakdown** — doughnut charts by asset type and geographic exposure
- **Import / Export** — save your portfolio as a JSON file and reload it any time
- **100% private** — all data is stored in your own browser's local storage. Nothing is sent to any server.

---

## How to Use

### Use it directly in your browser (recommended)
Visit the live GitHub Pages link:

> **https://waddell7.github.io/Portfolio-Tracker/PortfolioTrack.html**

No installation required. Just open the link and start adding holdings.
Best experience on 75% zoom

---

## Getting Started

### Adding a holding
1. Click **➕ Add** in the top right
2. Search for a ticker (e.g. `CBA.AX`, `NVDA`, `BTC`) — it will auto-suggest from Yahoo Finance
3. Fill in your purchase date, quantity, price, and currency
4. For non-AUD holdings, enter the AUD/foreign exchange rate at the time of purchase for accurate FX tracking (check your broker confirmation)
5. Click **Add Holding**

### Recording a sale
Click the 🛍️ icon on any holding to record a full or partial sale. P&L is locked in at the time of sale.

### Recording a dividend
Click the 📊 icon on any holding to record a dividend payment. Enter the **net cash amount per unit** (what hit your account) in cents — the app will gross it up automatically using the franking percentage you enter.

### Importing / Exporting
- **Export** — saves your entire portfolio as a `.json` file you can back up or move between devices
- **Import** — loads a previously exported `.json` file. You can review and edit each holding before confirming.

---

## Data & Privacy

- All portfolio data is stored in **your browser's local storage** — it never leaves your device
- Live prices are fetched directly from **Yahoo Finance** (via [corsproxy.io](https://corsproxy.io)) and **CoinGecko**
- No accounts, no tracking, no analytics

> **Note:** If prices are not loading, it may be due to corsproxy.io being temporarily unavailable or rate-limiting requests. Try refreshing after a minute or two.

---

## Supported Exchanges

Tickers are passed to Yahoo Finance, which supports most major global exchanges including:

| Exchange | Suffix |
|---|---|
| ASX (Australia) | `.AX` e.g. `BHP.AX` |
| NYSE / NASDAQ (US) | No suffix e.g. `AAPL` |
| LSE (London) | `.L` e.g. `HSBA.L` |
| TSX (Toronto) | `.TO` |
| Frankfurt | `.DE` |
| Tokyo | `.T` |
| Hong Kong | `.HK` |
| Singapore | `.SI` |

Crypto tickers use CoinGecko IDs (e.g. `BTC`, `ETH`, `SOL`).

---

## Limitations

- **Historical data** on the performance chart depends on Yahoo Finance availability via corsproxy. Some tickers may have gaps.
- **Crypto prices** use CoinGecko's free API which has rate limits — if you have many crypto holdings, some prices may not load on the first refresh.
- **Exchange rates** use exchangerate-api.com with a fallback to approximate rates if the API is unavailable.
- This tool is designed for **personal tracking only** and should not be used as a source of truth for tax reporting. Always verify figures with your broker statements.

---

## Disclaimer

This tool is for **personal informational purposes only**. It is not financial advice. I am not a certified financial advisers and take no responsibility for investment decisions made using this tool. Always consult a qualified financial adviser before making investment decisions.

Price data is sourced from third-party APIs and may be delayed, inaccurate, or unavailable. Do not rely on this tool for real-time trading decisions.

---

## Contributing

Found a bug or have a feature suggestion? Open an issue or submit a pull request, contributions are most welcome.

---


