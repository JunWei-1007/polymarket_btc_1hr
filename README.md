# Polymarket NPC — BTC 1 小時市場 YES/NO → 1 分鐘 K 線視覺化工具

專案核心目的：

**取得 Polymarket「BTC 1 小時市場」的 YES / NO 訂單簿資料，並將其轉換成 1 分鐘 K 線後在前端顯示。**

---

## 功能摘要
- 自動生成 Polymarket 市場 slug（依照日期與 ET 時間）
- 透過後端 API 取得：
  - YES / NO Token ID
  - 兩者的訂單簿成交資料
- 將成交資料依 timestamp 聚合為 **1 分鐘 K 線 (1m OHLCV)**
- 若該分鐘無交易，使用上一分鐘 close 補齊
- 將 YES / NO K 線對齊後同時渲染
- 使用 Lightweight Charts 顯示：
  - K 線圖
  - 量能 Volume
  - 雙圖時間軸同步
  - 十字線同步

---

## 使用目的
- 視覺化分析 BTC 1 小時市場的短線變化
- 比較 YES / NO Token 的價量差異
- 用於預測、套利、微觀市場行為研究
