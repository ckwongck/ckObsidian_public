---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-10-14 06:00:12 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-10-14 06:00:03

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 51,204 / USD 67,657
  * **實時現金結餘: USD 0 / HKD 51,204**
  * 剩餘購買力: 682,249 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 335,833 (約 HKD 2,619,498) [報表日 2026-10-12, 落後 2 日 ⚠️ 資料落後; 同步於 2026-10-14T05:50]
  * 現金結餘: HKD -0 / USD 5,244
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 75 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 33.389 USD | 19633 USD | 4.5% | 1872 USD | 10.5% | 15.7 | 0.98 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 306.3 USD | 10720 USD | 2.4% | 2290 USD | 27.2% | 18.3 | 0.9 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 357.19 USD | 18217 USD | 4.1% | -671 USD | -3.5% | 36.0 | 0.66 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 340.75 USD | 19082 USD | 4.3% | 1956 USD | 11.4% | 18.2 | 0.97 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 178.7 USD | 38957 USD | 8.9% | - | - | 37.6 | 1.07 | - | Flex(2026-10-12) |
| IB | PLTR | 227.0 | 131.423413062 USD | 209.0 USD | 47443 USD | 10.8% | - | - | 42.0 | 0.74 | - | Flex(2026-10-12) |
| IB | QQQM | 434.0 | 249.066141779 USD | 307.19 USD | 133320 USD | 30.4% | - | - | 18.3 | 0.9 | - | Flex(2026-10-12) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.52 USD | 38901 USD | 8.9% | - | - | 5.3 | 0.8 | - | Flex(2026-10-12) |
| IB | SPCX | 122.0 | 140.002405574 USD | 163.42 USD | 19937 USD | 4.5% | - | - | 38.0 | 0.75 | - | Flex(2026-10-12) |
| IB | URA | 840.0 | 50.432105573 USD | 37.72 USD | 31685 USD | 7.2% | - | - | 55.9 | 1.03 | - | Flex(2026-10-12) |
| IB | VRT | 85.0 | 289.688176106 USD | 239.36 USD | 20346 USD | 4.6% | - | - | 56.0 | 0.96 | - | Flex(2026-10-12) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.7% | - | - | 53.9 | 0.62 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.0% | - | - | 49.2 | 0.91 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 5.6% | - | - | 18.3 | 0.9 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$439,236**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $400,335 = **91.1%** | 目標 90% | drift +1.1% ⚠️ 超配
  - 防禦 (defense: SGOV+現金): $51,165 = **11.6%** | 目標 10% | drift +1.6% ⚠️ 超配
  - 戶口現金: $12,264

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $156.54 | IV Rank: 38.0 | Vol/30dAvg: 0.75 | 下次財報: -
  * P: 最新價 $156.97 | IV Rank: 59.2 | Vol/30dAvg: 0.51 | 下次財報: -
  * AVGO: 最新價 $357.31 | IV Rank: 36.0 | Vol/30dAvg: 0.66 | 下次財報: -
  * QQQM: 最新價 $306.16 | IV Rank: 18.3 | Vol/30dAvg: 0.9 | 下次財報: -
  * URA: 最新價 $37.38 | IV Rank: 55.9 | Vol/30dAvg: 1.03 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 101.09 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 15.27 | VIX9D (9日短期): 11.99 | VIX9D/VIX Ratio: 0.79 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.11% (信用違約風險, >6%=壓力)
* FOMC 倒數: 13 天 (下次 2026-10-27)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| MU | $953.19 | 65 | 9.9 | 2.70% | 30.9 | 1.12x | -3.96% |
| TSM | $445.12 | 65 | 5.1 | 31.66% | 49.1 | 0.88x | +1.47% |
* 數據更新: 2026-10-14 05:33:29 HKT

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀
2. 🎯 **Alpha 機會**: MU (總分 65) — 考慮研究後分批建倉

=== [END OF MAX DATA PACK v4.1] ===
