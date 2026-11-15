# 台積電 (2330.TW) 歷史 K 線圖

## 說明

本專案使用 **合法公開資料來源** Yahoo Finance（透過 Python `yfinance` 套件）抓取台積電歷史股價，並產生可完全離線互動的自建網頁。

### 網頁功能

- **時間區間下拉選單**：1 個月、3 個月、6 個月、1 年、2 年
- **K 線週期**：日線 / 週線 / 月線
- **移動平均線勾選**：MA5、MA10、MA20（可任意開關）
- 蠟燭圖 + 成交量（成交量顏色依漲跌）
- 深色主題、響應式、可縮放

### 檔案

| 檔案 | 說明 |
|------|------|
| `fetch_and_generate.py` | 爬蟲 + 資料處理 + 網頁產生程式 |
| `tsmc_kline.html` / `index.html` | 完整互動網頁 |

### 使用方式

1. **線上查看**（啟用 GitHub Pages 後）
   - 前往 Settings → Pages → Source 選 Deploy from a branch → main / (root)
   - 網址會是：https://abc0989297955-lab.github.io/tsmc-kline-chart/

2. **重新抓取最新資料**
   ```bash
   pip install yfinance pandas
   python fetch_and_generate.py
   ```

### 資料來源聲明

- 資料來自 Yahoo Finance 公開歷史報價
- 僅供學習、研究與個人使用
- 不構成任何投資建議
