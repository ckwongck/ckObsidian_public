---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-10-13 06:00:42 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-10-13 06:00:33

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 50,000 / USD 67,477
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 578,575 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 338,451 (約 HKD 2,639,918) [報表日 2026-10-09, 落後 4 日 ⚠️ 資料落後; 同步於 2026-10-13T05:50]
  * 現金結餘: HKD -0 / USD 5,244
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 74 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 33.29 USD | 19575 USD | 4.4% | 1814 USD | 10.2% | 14.7 | 0.74 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 307.18 USD | 10751 USD | 2.4% | 2321 USD | 27.5% | 16.9 | 0.87 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 354.816 USD | 18096 USD | 4.1% | -792 USD | -4.2% | 7.1 | 0.6 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 340.89 USD | 19090 USD | 4.3% | 1963 USD | 11.5% | 5.0 | 0.63 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 180.89 USD | 39434 USD | 8.9% | - | - | 34.9 | 0.81 | - | Flex(2026-10-09) |
| IB | PLTR | 227.0 | 131.423413062 USD | 209.05 USD | 47454 USD | 10.7% | - | - | 40.7 | 0.98 | - | Flex(2026-10-09) |
| IB | QQQM | 434.0 | 249.066141779 USD | 309.39 USD | 134275 USD | 30.4% | - | - | 16.9 | 0.87 | - | Flex(2026-10-09) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.51 USD | 38897 USD | 8.8% | - | - | 3.9 | 0.69 | - | Flex(2026-10-09) |
| IB | SPCX | 122.0 | 140.002405574 USD | 162.57 USD | 19834 USD | 4.5% | - | - | 8.4 | 0.73 | - | Flex(2026-10-09) |
| IB | URA | 840.0 | 50.432105573 USD | 38.9 USD | 32676 USD | 7.4% | - | - | 43.8 | 1.06 | - | Flex(2026-10-09) |
| IB | VRT | 85.0 | 289.688176106 USD | 242.78 USD | 20636 USD | 4.7% | - | - | 52.2 | 0.7 | - | Flex(2026-10-09) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.7% | - | - | 45.3 | 0.71 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.0% | - | - | 49.8 | 0.44 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 5.5% | - | - | 16.9 | 0.87 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$441,713**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $402,816 = **91.2%** | 目標 90% | drift +1.2% ⚠️ 超配
  - 防禦 (defense: SGOV+現金): $44,596 = **10.1%** | 目標 10% | drift +0.1% ✅
  - 戶口現金: $5,699

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $163.42 | IV Rank: 8.4 | Vol/30dAvg: 0.73 | 下次財報: -
  * P: 最新價 $155.31 | IV Rank: 59.0 | Vol/30dAvg: 0.66 | 下次財報: -
  * AVGO: 最新價 $354.73 | IV Rank: 7.1 | Vol/30dAvg: 0.6 | 下次財報: -
  * QQQM: 最新價 $307.19 | IV Rank: 16.9 | Vol/30dAvg: 0.87 | 下次財報: -
  * URA: 最新價 $37.72 | IV Rank: 43.8 | Vol/30dAvg: 1.06 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 98.47 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 15.21 | VIX9D (9日短期): 11.68 | VIX9D/VIX Ratio: 0.77 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.15% (信用違約風險, >6%=壓力)
* FOMC 倒數: 14 天 (下次 2026-10-27)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| MU | $989.04 | 75 | 10.3 | 2.60% | 32.1 | 0.92x | -0.51% |
| TSM | $444.35 | 75 | 5.2 | 31.71% | 45.7 | 0.91x | +1.35% |
* 數據更新: 2026-10-13 05:35:06 HKT

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀
2. 🎯 **Alpha 機會**: MU (總分 75) — 考慮研究後分批建倉

=== [END OF MAX DATA PACK v4.1] ===
