---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-10-21 06:00:32 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-10-21 06:00:23

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 0 / USD 67,071
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 671,462 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 318,606 (約 HKD 2,485,128) [報表日 2026-10-19, 落後 2 日 ⚠️ 資料落後; 同步於 2026-10-21T05:50]
  * 現金結餘: HKD -0 / USD 5,244
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 82 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 34.68 USD | 20392 USD | 4.8% | 2631 USD | 14.8% | 12.7 | 0.92 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 298.05 USD | 10432 USD | 2.5% | 2001 USD | 23.7% | 22.1 | 1.31 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 339.339 USD | 17306 USD | 4.1% | -1582 USD | -8.4% | 34.8 | 0.67 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 338.88 USD | 18977 USD | 4.5% | 1851 USD | 10.8% | 18.2 | 0.87 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 168.8 USD | 36798 USD | 8.7% | - | - | 32.0 | 1.39 | - | Flex(2026-10-19) |
| IB | PLTR | 227.0 | 131.423413062 USD | 194.15 USD | 44072 USD | 10.5% | - | - | 47.3 | 0.63 | - | Flex(2026-10-19) |
| IB | QQQM | 434.0 | 249.066141779 USD | 295.78 USD | 128369 USD | 30.5% | - | - | 22.1 | 1.31 | - | Flex(2026-10-19) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.59 USD | 38928 USD | 9.2% | - | - | 2.6 | 0.89 | - | Flex(2026-10-19) |
| IB | SPCX | 122.0 | 140.002405574 USD | 147.96 USD | 18051 USD | 4.3% | - | - | 120.5 | 1.07 | - | Flex(2026-10-19) |
| IB | URA | 840.0 | 50.432105573 USD | 35.27 USD | 29627 USD | 7.0% | - | - | 49.2 | 1.18 | - | Flex(2026-10-19) |
| IB | VRT | 85.0 | 289.688176106 USD | 206.08 USD | 17517 USD | 4.2% | - | - | 58.2 | 1.2 | - | Flex(2026-10-19) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.8% | - | - | 52.9 | 0.83 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.1% | - | - | 53.3 | 1.08 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 5.8% | - | - | 22.1 | 1.31 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$421,464**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $382,536 = **90.8%** | 目標 90% | drift +0.8% ✅
  - 防禦 (defense: SGOV+現金): $44,627 = **10.6%** | 目標 10% | drift +0.6% ✅
  - 戶口現金: $5,699

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $147.79 | IV Rank: 120.5 | Vol/30dAvg: 1.07 | 下次財報: -
  * P: 最新價 $126.52 | IV Rank: 75.3 | Vol/30dAvg: 0.4 | 下次財報: -
  * AVGO: 最新價 $334.37 | IV Rank: 34.8 | Vol/30dAvg: 0.67 | 下次財報: -
  * QQQM: 最新價 $295.59 | IV Rank: 22.1 | Vol/30dAvg: 1.31 | 下次財報: -
  * URA: 最新價 $35.18 | IV Rank: 49.2 | Vol/30dAvg: 1.18 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 101.69 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 17.31 | VIX9D (9日短期): 16.27 | VIX9D/VIX Ratio: 0.94 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.29% (信用違約風險, >6%=壓力)
* FOMC 倒數: 6 天 (下次 2026-10-27)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| TSM | $425.08 | 75 | 3.9 | 54.57% | 36.7 | 1.15x | -2.42% |
* 數據更新: 2026-10-21 05:33:55 HKT

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀
2. 🎯 **Alpha 機會**: TSM (總分 75) — 考慮研究後分批建倉
3. 📅 **FOMC 倒數 6 天** → 議息前市場波動加劇，避免重倉操作

=== [END OF MAX DATA PACK v4.1] ===
