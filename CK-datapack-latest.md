---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-10-02 06:00:15 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-10-02 06:00:07

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 50,000 / USD 66,055
  * **實時現金結餘: USD 23 / HKD 0**
  * 剩餘購買力: 645,943 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 326,799 (約 HKD 2,549,033) [報表日 2026-09-30, 落後 2 日 ⚠️ 資料落後; 同步於 2026-10-02T05:50]
  * 現金結餘: HKD -0 / USD 2,162
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 63 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 32.72 USD | 19239 USD | 4.5% | 1478 USD | 8.3% | 19.6 | 1.03 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 305.493 USD | 10692 USD | 2.5% | 2262 USD | 26.8% | 19.0 | 1.32 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 345.21 USD | 17606 USD | 4.1% | -1282 USD | -6.8% | 28.5 | 0.89 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 330.11 USD | 18486 USD | 4.3% | 1360 USD | 7.9% | 19.6 | 0.85 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 177.11 USD | 38610 USD | 8.9% | - | - | 29.3 | 0.94 | - | Flex(2026-09-30) |
| IB | PLTR | 227.0 | 131.423413062 USD | 187.05 USD | 42460 USD | 9.8% | - | - | 33.7 | 0.66 | - | Flex(2026-09-30) |
| IB | QQQM | 434.0 | 249.066141779 USD | 304.64 USD | 132214 USD | 30.6% | - | - | 19.0 | 1.32 | - | Flex(2026-09-30) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.68 USD | 38963 USD | 9.0% | - | - | 3.6 | 1.82 | - | Flex(2026-09-30) |
| IB | SPCX | 122.0 | 140.002405574 USD | 150.86 USD | 18405 USD | 4.3% | - | - | 34.3 | 0.81 | - | Flex(2026-09-30) |
| IB | URA | 840.0 | 50.432105573 USD | 39.85 USD | 33474 USD | 7.8% | - | - | 55.6 | 1.21 | - | Flex(2026-09-30) |
| IB | VRT | 85.0 | 289.688176106 USD | 241.31 USD | 20511 USD | 4.8% | - | - | 47.4 | 0.7 | - | Flex(2026-09-30) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.8% | - | - | 53.2 | 1.54 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.1% | - | - | 42.1 | 1.38 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 5.7% | - | - | 19.0 | 1.32 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$431,656**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $392,693 = **91.0%** | 目標 90% | drift +1.0% ✅
  - 防禦 (defense: SGOV+現金): $41,603 = **9.6%** | 目標 10% | drift -0.4% ✅
  - 戶口現金: $2,640

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $148.07 | IV Rank: 34.3 | Vol/30dAvg: 0.81 | 下次財報: -
  * P: 最新價 $134.13 | IV Rank: 58.0 | Vol/30dAvg: 0.67 | 下次財報: -
  * AVGO: 最新價 $343.64 | IV Rank: 28.5 | Vol/30dAvg: 0.89 | 下次財報: -
  * QQQM: 最新價 $305.57 | IV Rank: 19.0 | Vol/30dAvg: 1.32 | 下次財報: -
  * URA: 最新價 $39.59 | IV Rank: 55.6 | Vol/30dAvg: 1.21 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 108.13 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 16.39 | VIX9D (9日短期): 14.0 | VIX9D/VIX Ratio: 0.85 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: -0.07% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.12% (信用違約風險, >6%=壓力)
* FOMC 倒數: 25 天 (下次 2026-10-27)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| GOOGL | $338.24 | 75 | 23.7 | 0.55% | 49.8 | 1.27x | -2.04% |
* 數據更新: 2026-10-02 05:33:55 HKT

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀
2. 🎯 **Alpha 機會**: GOOGL (總分 75) — 考慮研究後分批建倉

=== [END OF MAX DATA PACK v4.1] ===
