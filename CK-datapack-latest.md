---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-10-24 06:00:17 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-10-24 06:00:10

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 0 / USD 66,829
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 668,793 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 313,131 (約 HKD 2,442,424) [報表日 2026-10-22, 落後 2 日 ⚠️ 資料落後; 同步於 2026-10-24T05:50]
  * 現金結餘: HKD -0 / USD 5,244
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 85 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 35.27 USD | 20739 USD | 5.0% | 2978 USD | 16.8% | 27.4 | 0.98 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 290.733 USD | 10176 USD | 2.4% | 1745 USD | 20.7% | 25.1 | 0.87 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 322.6 USD | 16453 USD | 4.0% | -2435 USD | -12.9% | 10.6 | 0.68 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 347.54 USD | 19462 USD | 4.7% | 2336 USD | 13.6% | 4.9 | 1.02 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 163.19 USD | 35575 USD | 8.6% | - | - | 34.2 | 0.84 | - | Flex(2026-10-22) |
| IB | PLTR | 227.0 | 131.423413062 USD | 196.19 USD | 44535 USD | 10.7% | - | - | 10.4 | 0.68 | - | Flex(2026-10-22) |
| IB | QQQM | 434.0 | 249.066141779 USD | 290.13 USD | 125916 USD | 30.3% | - | - | 25.1 | 0.87 | - | Flex(2026-10-22) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.62 USD | 38940 USD | 9.4% | - | - | 2.8 | 0.86 | - | Flex(2026-10-22) |
| IB | SPCX | 122.0 | 140.002405574 USD | 144.75 USD | 17660 USD | 4.2% | - | - | 14.2 | 1.09 | - | Flex(2026-10-22) |
| IB | URA | 840.0 | 50.432105573 USD | 34.09 USD | 28636 USD | 6.9% | - | - | 38.2 | 0.81 | - | Flex(2026-10-22) |
| IB | VRT | 85.0 | 289.688176106 USD | 195.59 USD | 16625 USD | 4.0% | - | - | 19.8 | 1.35 | - | Flex(2026-10-22) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.8% | - | - | 37.4 | 0.68 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.1% | - | - | 11.9 | 1.55 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 5.9% | - | - | 25.1 | 0.87 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$415,711**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $376,771 = **90.6%** | 目標 90% | drift +0.6% ✅
  - 防禦 (defense: SGOV+現金): $92,646 = **22.3%** | 目標 10% | drift +12.3% ⚠️ 超配
  - 戶口現金: $53,706

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $147.49 | IV Rank: 14.2 | Vol/30dAvg: 1.09 | 下次財報: -
  * P: 最新價 $123.33 | IV Rank: 79.0 | Vol/30dAvg: 0.31 | 下次財報: -
  * AVGO: 最新價 $321.68 | IV Rank: 10.6 | Vol/30dAvg: 0.68 | 下次財報: -
  * QQQM: 最新價 $290.06 | IV Rank: 25.1 | Vol/30dAvg: 0.87 | 下次財報: -
  * URA: 最新價 $34.11 | IV Rank: 38.2 | Vol/30dAvg: 0.81 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 103.31 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 19.45 | VIX9D (9日短期): 18.7 | VIX9D/VIX Ratio: 0.96 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.4% (信用違約風險, >6%=壓力)
* FOMC 倒數: 3 天 (下次 2026-10-27)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| VZ | $44.66 | 90 | 7.5 | 9.41% | 48.0 | 1.90x | -2.42% |
* 數據更新: 2026-10-24 05:33:59 HKT

## 六、建議行動 (Actionable Insights)
1. 💰 **現金/SGOV 過多 12.3%** → 錯失增長機會，考慮分批轉增長倉
2. 🎯 **Alpha 機會**: VZ (總分 90) — 考慮研究後分批建倉
3. 📅 **FOMC 倒數 3 天** → 議息前市場波動加劇，避免重倉操作

=== [END OF MAX DATA PACK v4.1] ===
