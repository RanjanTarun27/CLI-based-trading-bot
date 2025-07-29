# CLI-based-trading-bot
# 🧠 Binance USDT-M Futures Trading Bot (CLI-Based)

A command-line interface (CLI) trading bot for Binance USDT-M Futures. Supports core and advanced order types, robust input validation, and structured logging.

---

## 📝 Project Log Format (README Style)

### 📌 [INIT] Project Initialized

- Structure established
- Requirements gathered:
  - Market, Limit, Stop-Limit, OCO, TWAP, Grid Orders
  - Input validation
  - Action logging (order placements, errors, execution)

---

### 🔧 [SETUP] Environment Preparation

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
python-binance
python-dotenv
API_KEY=your_api_key_here
API_SECRET=your_api_secret_here
[2025-07-29 19:44:12] INFO: Order Placed | Type: LIMIT | Symbol: BTCUSDT | Price: 28900.0 | Qty: 0.01 | Side: BUY
[2025-07-29 19:44:15] ERROR: Validation failed - Invalid quantity
[2025-07-29 19:44:18] INFO: OCO Order Triggered | TP: 29000 | SL: 28700
client = Client(API_KEY, API_SECRET)
client.FUTURES_URL = 'https://testnet.binancefuture.com'
