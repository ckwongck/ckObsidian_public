---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-11-03 06:00:53 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-11-03 06:00:44

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 0 / USD 66,344
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 665,062 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 309,816 (約 HKD 2,416,564) [報表日 2026-10-30, 落後 4 日 ⚠️ 資料落後; 同步於 2026-11-03T05:50]
  * 現金結餘: HKD 0 / USD 5,242
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 95 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 35.93 USD | 21127 USD | 5.1% | 3366 USD | 18.9% | 16.2 | 1.16 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 281.43 USD | 9850 USD | 2.4% | 1420 USD | 16.8% | 30.8 | 1.66 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 322.912 USD | 16469 USD | 4.0% | -2419 USD | -12.8% | 9.7 | 0.9 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 339.402 USD | 19007 USD | 4.6% | 1880 USD | 11.0% | 63.8 | 1.5 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 164.51 USD | 35863 USD | 8.7% | - | - | 40.8 | 0.62 | - | Flex(2026-10-30) |
| IB | PLTR | 227.0 | 131.423413062 USD | 184.11 USD | 41793 USD | 10.1% | - | - | 138.8 | 1.56 | - | Flex(2026-10-30) |
| IB | QQQM | 434.0 | 249.066141779 USD | 284.34 USD | 123404 USD | 30.0% | - | - | 30.8 | 1.66 | - | Flex(2026-10-30) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.73 USD | 38983 USD | 9.5% | - | - | 5.0 | 1.69 | - | Flex(2026-10-30) |
| IB | SPCX | 122.0 | 140.002405574 USD | 134.72 USD | 16436 USD | 4.0% | - | - | 8.5 | 0.94 | - | Flex(2026-10-30) |
| IB | URA | 840.0 | 50.432105573 USD | 33.73 USD | 28333 USD | 6.9% | - | - | 56.8 | 1.06 | - | Flex(2026-10-30) |
| IB | VRT | 85.0 | 289.688176106 USD | 232.5 USD | 19762 USD | 4.8% | - | - | 77.4 | 1.0 | - | Flex(2026-10-30) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.8% | - | - | 62.0 | 0.9 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.2% | - | - | 67.4 | 1.3 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 5.9% | - | - | 30.8 | 1.66 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$412,021**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $373,038 = **90.5%** | 目標 90% | drift +0.5% ✅
  - 防禦 (defense: SGOV+現金): $44,680 = **10.8%** | 目標 10% | drift +0.8% ✅
  - 戶口現金: $5,697

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $136.37 | IV Rank: 8.5 | Vol/30dAvg: 0.94 | 下次財報: -
  * P: 最新價 $113.78 | IV Rank: 102.7 | Vol/30dAvg: 0.9 | 下次財報: -
  * AVGO: 最新價 $322.23 | IV Rank: 9.7 | Vol/30dAvg: 0.9 | 下次財報: -
  * QQQM: 最新價 $280.49 | IV Rank: 30.8 | Vol/30dAvg: 1.66 | 下次財報: -
  * URA: 最新價 $32.93 | IV Rank: 56.8 | Vol/30dAvg: 1.06 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 100.36 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 21.15 | VIX9D (9日短期): 22.46 | VIX9D/VIX Ratio: 1.06 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.44% (信用違約風險, >6%=壓力)
* FOMC 倒數: 35 天 (下次 2026-12-08)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| MU | $833.59 | 65 | 8.8 | 3.09% | 37.9 | 1.10x | -12.60% |
* 數據更新: 2026-11-03 05:35:00 HKT

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀
2. 🎯 **Alpha 機會**: MU (總分 65) — 考慮研究後分批建倉

=== [END OF MAX DATA PACK v4.1] ===
