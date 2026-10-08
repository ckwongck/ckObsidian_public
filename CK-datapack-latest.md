---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-10-09 06:00:32 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-10-09 06:00:23

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 50,000 / USD 67,725
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 580,821 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 337,708 (約 HKD 2,634,119) [報表日 2026-10-07, 落後 2 日 ⚠️ 資料落後; 同步於 2026-10-09T05:50]
  * 現金結餘: HKD -0 / USD 5,244
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 70 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 33.05 USD | 19433 USD | 4.4% | 1673 USD | 9.4% | 24.5 | 1.02 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 308.24 USD | 10788 USD | 2.4% | 2358 USD | 28.0% | 16.5 | 1.08 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 361.8 USD | 18452 USD | 4.2% | -436 USD | -2.3% | 32.4 | 1.03 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 340.38 USD | 19061 USD | 4.3% | 1935 USD | 11.3% | 16.9 | 0.85 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 179.79 USD | 39194 USD | 8.9% | - | - | 29.6 | 1.2 | - | Flex(2026-10-07) |
| IB | PLTR | 227.0 | 131.423413062 USD | 194.12 USD | 44065 USD | 10.0% | - | - | 34.2 | 1.71 | - | Flex(2026-10-07) |
| IB | QQQM | 434.0 | 249.066141779 USD | 311.94 USD | 135382 USD | 30.7% | - | - | 16.5 | 1.08 | - | Flex(2026-10-07) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.47 USD | 38882 USD | 8.8% | - | - | 5.0 | 0.81 | - | Flex(2026-10-07) |
| IB | SPCX | 122.0 | 140.002405574 USD | 167.6 USD | 20447 USD | 4.6% | - | - | 37.8 | 0.76 | - | Flex(2026-10-07) |
| IB | URA | 840.0 | 50.432105573 USD | 39.93 USD | 33541 USD | 7.6% | - | - | - | 1.6 | - | Flex(2026-10-07) |
| IB | VRT | 85.0 | 289.688176106 USD | 246.49 USD | 20952 USD | 4.7% | - | - | 54.9 | 1.18 | - | Flex(2026-10-07) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.7% | - | - | 57.0 | 1.84 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.0% | - | - | 45.2 | 1.07 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 5.5% | - | - | 16.5 | 1.08 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$441,193**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $402,311 = **91.2%** | 目標 90% | drift +1.2% ⚠️ 超配
  - 防禦 (defense: SGOV+現金): $44,581 = **10.1%** | 目標 10% | drift +0.1% ✅
  - 戶口現金: $5,699

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $160.57 | IV Rank: 37.8 | Vol/30dAvg: 0.76 | 下次財報: -
  * P: 最新價 $150.57 | IV Rank: 58.9 | Vol/30dAvg: 0.88 | 下次財報: -
  * AVGO: 最新價 $360.14 | IV Rank: 32.4 | Vol/30dAvg: 1.03 | 下次財報: -
  * QQQM: 最新價 $307.85 | IV Rank: 16.5 | Vol/30dAvg: 1.08 | 下次財報: -
  * URA: 最新價 $38.56 | IV Rank: - | Vol/30dAvg: 1.6 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 100.7 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 15.41 | VIX9D (9日短期): 12.21 | VIX9D/VIX Ratio: 0.79 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.09% (信用違約風險, >6%=壓力)
* FOMC 倒數: 18 天 (下次 2026-10-27)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| T | $24.87 | 90 | 7.4 | 5.95% | 39.8 | 1.42x | +0.40% |
| VZ | $46.35 | 75 | 7.5 | 9.07% | 33.0 | 1.01x | -2.29% |
| TSM | $457.99 | 65 | 5.4 | 30.77% | 62.6 | 1.35x | +4.67% |
* 數據更新: 2026-10-09 05:33:53 HKT

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀
2. 🎯 **Alpha 機會**: T (總分 90) — 考慮研究後分批建倉

=== [END OF MAX DATA PACK v4.1] ===
