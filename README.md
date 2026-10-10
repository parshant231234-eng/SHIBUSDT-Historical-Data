# SHIBUSDT 1-Minute Historical Kline Dataset

An institutional-grade, open-source archive of cleaned, standardized, and validated **1-minute intraday historical kline data** for **SHIBUSDT** (Binance Spot).

---

## 📊 Dataset Specifications
- **Symbol:** `SHIBUSDT`
- **Market:** Binance Spot
- **Timeframe:** 1 Minute (`1m`)
- **Total Months:** `66` months
- **Total Candles:** `2,848,629` 1-minute candles
- **Schema:** `timestamp, datetime_utc, open, high, low, close, volume, quote_volume, trade_count, taker_buy_volume, taker_buy_quote_volume`

---

## 🏛️ Directory Hierarchy
```text
SHIBUSDT-Historical-Data/
├── README.md
└── 1m/
    └── <YYYY>/
        └── <MM>/
            └── SHIBUSDT_1m_<YYYY-MM>.csv
```

---

## ⚡ 1-Line Pandas Stream Loader
Load any month directly from GitHub's raw CDN without cloning the repository:

```python
import pandas as pd

url = "https://raw.githubusercontent.com/parshant231234-eng/SHIBUSDT-Historical-Data/main/1m/2026/09/SHIBUSDT_1m_2026-09.csv"
df = pd.read_csv(url)
print(df.head())
```
