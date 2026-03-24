![BlinkX API — Developer Platform](banner.png)

<div align="center">

# BlinkX API &nbsp;—&nbsp; Developer Platform

**Official developer platform for BlinkX.**  
Build algorithmic trading apps with real-time order execution, live market feeds, and portfolio APIs.

BlinkX API gives developers direct programmatic access to India's stock markets — NSE and BSE.  
Whether you're building a quantitative trading bot, an analytics dashboard, or a full-fledged algo platform,  
our unified API handles execution, data, and risk — so you can focus on your strategy.

<br/>

[![Python SDK](https://img.shields.io/badge/Python_SDK-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://github.com/blinkx/blinkx-python)
[![Java SDK](https://img.shields.io/badge/Java_SDK-E76F00?style=for-the-badge&logo=openjdk&logoColor=white)](https://github.com/blinkx/blinkx-java)
[![Go SDK](https://img.shields.io/badge/Go_SDK-00ACD7?style=for-the-badge&logo=go&logoColor=white)](https://github.com/blinkx/blinkx-go)
[![Node.js SDK](https://img.shields.io/badge/Node.js_SDK-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://github.com/blinkx/blinkx-nodejs)

</div>

---

## ⚡ What You Can Build

| Capability | Description |
|---|---|
| **Order Management** | Place, modify and cancel MARKET, LIMIT and SL orders — up to **9 OPS** |
| **Live Market Feed** | WebSocket streaming for **1,000+ instruments** across NSE & BSE |
| **Historical Data** | Tick-by-tick and OHLCV candle data for backtesting and analysis |
| **Portfolio Management** | Real-time holdings, positions, P&L and margin data |
| **Authentication** | OAuth 2.0 — secure, stateless, daily-session based |

---

## 🚀 Quickstart

**1. Sign up and get your API key**

```
https://developeruat.blinkx.in/signup
```

**2. Install the SDK**

```bash
pip install blinkx-python          # Python
npm install blinkx-nodejs          # Node.js
go get github.com/blinkx/blinkx-go # Go
```

**3. Place your first order**

```python
# Authenticate with BlinkX TradeAPI
from blinkx import TradeAPI

client = TradeAPI(
  api_key="bx_live_••••••••••••",
  access_token="eyJhbGci..."
)

# Place an order in real-time
order = client.place_order(
  symbol="RELIANCE",
  exchange="NSE",
  quantity=10,
  order_type="MARKET",
  side="BUY"
)

# → { "order_id": "BX20260323001", "status": "PLACED" }
```

---

## 📦 Repositories

| Repository | Language | Description |
|---|---|---|
| [blinkx-python](https://github.com/blinkx/blinkx-python) | 🐍 Python | Official Python SDK |
| [blinkx-java](https://github.com/blinkx/blinkx-java) | ☕ Java | Official Java SDK |
| [blinkx-go](https://github.com/blinkx/blinkx-go) | 🐹 Go | Official Go client |
| [blinkx-nodejs](https://github.com/blinkx/blinkx-nodejs) | 🟩 Node.js | Official Node.js SDK |
| [blinkx-docs](https://github.com/blinkx/blinkx-docs) | 📄 Markdown | API documentation source |

---

## 📚 Resources

- 📖 &nbsp;[API Documentation](https://api.blinkx.in/docs)
- 🔑 &nbsp;[Get Your API Key](https://developeruat.blinkx.in/signup)
- 💬 &nbsp;[Developer Support](mailto:api-support@blinkx.in)
- 🏢 &nbsp;[LinkedIn](https://www.linkedin.com/company/getblinkx)
- 📧 &nbsp;[General Enquiries](mailto:letstalk@blinkx.in)

---

## 📋 Platform Specs

```
Rate Limit          9 orders/second (sliding window)
Max Orders/Day      14,000
Instruments         1,000+ live (NSE + BSE)
API Charges         ₹0 — free to use
Auth                OAuth 2.0 (daily session)
Data Formats        JSON / Protobuf (WebSocket)
Exchanges           NSE · BSE · NSE F&O · NSE Currency · MCX
Compliance          SEBI-compliant · Static IP mandatory
```

---

## 🛠 SEBI & Regulatory Notice

BlinkX API complies with all SEBI and exchange regulations for algorithmic trading in India.  
A **static IP address** is mandatory for all API integrations per NSE/BSE guidelines (effective August 2025).  
All order activity is logged and auditable for a minimum of 5 years.

---

<div align="center">

**© 2026 BlinkX · Powered by JM Financial**  
[api.blinkx.in](https://api.blinkx.in) &nbsp;·&nbsp; [Terms of Use](https://blinkx.in/terms) &nbsp;·&nbsp; [Privacy Policy](https://blinkx.in/privacy)

</div>
