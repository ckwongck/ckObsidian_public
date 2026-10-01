---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-10-01 08:08:54 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-10-01 08:08:35

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 50,000 / USD 66,615
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 650,766 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 327,188 (約 HKD 2,552,065) [報表日 2026-09-29, 落後 2 日 ⚠️ 資料落後; 同步於 2026-10-01T08:08]
  * 現金結餘: HKD -0 / USD 2,108
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 62 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 32.67 USD | 19210 USD | 4.4% | 1449 USD | 8.2% | 20.8 | 0.9 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 305.63 USD | 10697 USD | 2.5% | 2267 USD | 26.9% | 20.0 | 1.14 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 371.0 USD | 352.8 USD | 17993 USD | 4.2% | -928 USD | -4.9% | 46.4 | 0.72 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 333.9 USD | 18698 USD | 4.3% | 1572 USD | 9.2% | 29.9 | 1.21 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 178.27 USD | 38863 USD | 9.0% | - | - | 33.2 | 0.68 | - | Flex(2026-09-29) |
| IB | PLTR | 227.0 | 131.423413062 USD | 186.97 USD | 42442 USD | 9.8% | - | - | 49.5 | 0.61 | - | Flex(2026-09-29) |
| IB | QQQM | 434.0 | 249.066141779 USD | 303.83 USD | 131862 USD | 30.5% | - | - | 20.0 | 1.14 | - | Flex(2026-09-29) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.68 USD | 38963 USD | 9.0% | - | - | 3.8 | 1.42 | - | Flex(2026-09-29) |
| IB | SPCX | 122.0 | 140.002405574 USD | 149.24 USD | 18207 USD | 4.2% | - | - | 48.7 | 0.93 | - | Flex(2026-09-29) |
| IB | URA | 840.0 | 50.432105573 USD | 40.04 USD | 33634 USD | 7.8% | - | - | 50.6 | 0.69 | - | Flex(2026-09-29) |
| IB | VRT | 85.0 | 289.688176106 USD | 248.34 USD | 21109 USD | 4.9% | - | - | 57.9 | 0.83 | - | Flex(2026-09-29) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.8% | - | - | 56.0 | 1.62 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.1% | - | - | 54.3 | 0.81 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 5.7% | - | - | 20.0 | 1.14 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$432,673**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $393,710 = **91.0%** | 目標 90% | drift +1.0% ✅
  - 防禦 (defense: SGOV+現金): $41,526 = **9.6%** | 目標 10% | drift -0.4% ✅
  - 戶口現金: $2,563

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $150.86 | IV Rank: 48.7 | Vol/30dAvg: 0.93 | 下次財報: -
  * P: 最新價 $130.78 | IV Rank: 62.0 | Vol/30dAvg: 0.46 | 下次財報: -
  * AVGO: 最新價 $351.19 | IV Rank: 46.4 | Vol/30dAvg: 0.72 | 下次財報: -
  * QQQM: 最新價 $304.64 | IV Rank: 20.0 | Vol/30dAvg: 1.14 | 下次財報: -
  * URA: 最新價 $39.85 | IV Rank: 50.6 | Vol/30dAvg: 0.69 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 110.45 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 16.34 | VIX9D (9日短期): 14.2 | VIX9D/VIX Ratio: 0.87 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: -0.07% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.08% (信用違約風險, >6%=壓力)
* FOMC 倒數: 26 天 (下次 2026-10-27)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| AMZN | $249.15 | 75 | 16.5 | 0.12% | 46.9 | 1.21x | -1.79% |
| DIS | $104.90 | 75 | 11.0 | 2.68% | 47.1 | 1.34x | +0.60% |
* 數據更新: 2026-10-01 05:33:49 HKT

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀
2. 🎯 **Alpha 機會**: AMZN (總分 75) — 考慮研究後分批建倉

=== [END OF MAX DATA PACK v4.1] ===
