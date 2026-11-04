---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-11-05 06:01:03 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-11-05 06:00:54

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 0 / USD 67,523
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 674,584 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 307,969 (約 HKD 2,402,155) [報表日 2026-11-03, 落後 2 日 ⚠️ 資料落後; 同步於 2026-11-05T05:51]
  * 現金結餘: HKD 0 / USD 5,242
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 97 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 36.15 USD | 21256 USD | 5.2% | 3495 USD | 19.7% | 13.9 | 1.15 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 285.7 USD | 10000 USD | 2.4% | 1569 USD | 18.6% | 23.8 | 1.62 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 327.157 USD | 16685 USD | 4.1% | -2203 USD | -11.7% | 8.0 | 1.09 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 349.824 USD | 19590 USD | 4.8% | 2464 USD | 14.4% | 3.8 | 2.18 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 167.4 USD | 36493 USD | 8.9% | - | - | 35.5 | 1.56 | - | Flex(2026-11-03) |
| IB | PLTR | 227.0 | 131.423413062 USD | 175.4 USD | 39816 USD | 9.7% | - | - | 54.3 | 1.49 | - | Flex(2026-11-03) |
| IB | QQQM | 434.0 | 249.066141779 USD | 282.23 USD | 122488 USD | 29.8% | - | - | 23.8 | 1.62 | - | Flex(2026-11-03) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.44 USD | 38870 USD | 9.5% | - | - | 3.4 | 1.11 | - | Flex(2026-11-03) |
| IB | SPCX | 122.0 | 140.002405574 USD | 141.31 USD | 17240 USD | 4.2% | - | - | 8.9 | 1.39 | - | Flex(2026-11-03) |
| IB | URA | 840.0 | 50.432105573 USD | 33.05 USD | 27762 USD | 6.8% | - | - | 56.3 | 1.28 | - | Flex(2026-11-03) |
| IB | VRT | 85.0 | 289.688176106 USD | 235.97 USD | 20057 USD | 4.9% | - | - | 74.5 | 2.05 | - | Flex(2026-11-03) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.9% | - | - | 58.2 | 1.79 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.2% | - | - | 63.1 | 2.27 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 5.9% | - | - | 23.8 | 1.62 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$411,252**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $372,382 = **90.5%** | 目標 90% | drift +0.5% ✅
  - 防禦 (defense: SGOV+現金): $44,567 = **10.8%** | 目標 10% | drift +0.8% ✅
  - 戶口現金: $5,697

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $135.92 | IV Rank: 8.9 | Vol/30dAvg: 1.39 | 下次財報: -
  * P: 最新價 $111.77 | IV Rank: 106.0 | Vol/30dAvg: 0.63 | 下次財報: -
  * AVGO: 最新價 $325.48 | IV Rank: 8.0 | Vol/30dAvg: 1.09 | 下次財報: -
  * QQQM: 最新價 $284.92 | IV Rank: 23.8 | Vol/30dAvg: 1.62 | 下次財報: -
  * URA: 最新價 $32.70 | IV Rank: 56.3 | Vol/30dAvg: 1.28 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 93.88 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 16.61 | VIX9D (9日短期): 15.19 | VIX9D/VIX Ratio: 0.91 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.4% (信用違約風險, >6%=壓力)
* FOMC 倒數: 33 天 (下次 2026-12-08)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| MU | $795.23 | 80 | 8.5 | 3.24% | 36.9 | 1.32x | -15.74% |
| FOXA | $69.65 | 65 | 7.1 | 4.07% | 63.3 | 1.25x | +8.30% |
* 數據更新: 2026-11-05 05:34:25 HKT

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀
2. 🎯 **Alpha 機會**: MU (總分 80) — 考慮研究後分批建倉

=== [END OF MAX DATA PACK v4.1] ===
