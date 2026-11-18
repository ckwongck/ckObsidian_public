---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-11-19 06:09:34 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-11-19 06:00:29

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 0 / USD 67,575
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 677,427 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 297,457 (約 HKD 2,320,161) [報表日 2026-11-17, 落後 2 日 ⚠️ 資料落後; 同步於 2026-11-19T05:50]
  * 現金結餘: HKD 45,907 / USD 7,216
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 111 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 34.72 USD | 20415 USD | 5.2% | 2654 USD | 14.9% | - | - | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 271.42 USD | 9500 USD | 2.4% | 1069 USD | 12.7% | - | - | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 353.0 USD | 18003 USD | 4.6% | -885 USD | -4.7% | - | - | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.56 USD | 351.55 USD | 19687 USD | 5.0% | 2575 USD | 15.0% | 3.9 | 0.73 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 155.15 USD | 33823 USD | 8.6% | - | - | 51.7 | 2.44 | - | Flex(2026-11-17) |
| IB | PLTR | 227.0 | 131.423413062 USD | 156.56 USD | 35539 USD | 9.0% | - | - | - | - | - | Flex(2026-11-17) |
| IB | QQQM | 434.0 | 249.066141779 USD | 270.42 USD | 117362 USD | 29.9% | - | - | - | - | - | Flex(2026-11-17) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.59 USD | 38928 USD | 9.9% | - | - | 6.0 | 1.08 | - | Flex(2026-11-17) |
| IB | SPCX | 122.0 | 140.002405574 USD | 141.7 USD | 17287 USD | 4.4% | - | - | 11.3 | 0.82 | - | Flex(2026-11-17) |
| IB | URA | 840.0 | 50.432105573 USD | 30.04 USD | 25234 USD | 6.4% | - | - | 60.9 | 1.44 | - | Flex(2026-11-17) |
| IB | VRT | 85.0 | 289.688176106 USD | 190.37 USD | 16181 USD | 4.1% | - | - | - | - | - | Flex(2026-11-17) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.9% | - | - | 52.4 | 0.66 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.3% | - | - | 66.5 | 0.82 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 6.2% | - | - | - | - | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$392,955**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $354,026 = **90.1%** | 目標 90% | drift +0.1% ✅
  - 防禦 (defense: SGOV+現金): $52,485 = **13.4%** | 目標 10% | drift +3.4% ⚠️ 超配
  - 戶口現金: $13,557

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: [需 Futu Basic 訂閱 / yfinance 離線] | IV Rank: 11.3 | Vol/30dAvg: 0.82 | 下次財報: -
  * P: [需 Futu Basic 訂閱 / yfinance 離線] | IV Rank: - | Vol/30dAvg: - | 下次財報: -
  * AVGO: [需 Futu Basic 訂閱 / yfinance 離線] | IV Rank: - | Vol/30dAvg: - | 下次財報: -
  * QQQM: [需 Futu Basic 訂閱 / yfinance 離線] | IV Rank: - | Vol/30dAvg: - | 下次財報: -
  * URA: [需 Futu Basic 訂閱 / yfinance 離線] | IV Rank: 60.9 | Vol/30dAvg: 1.44 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: None (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): None | VIX9D (9日短期): None | VIX9D/VIX Ratio: - (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.43% (信用違約風險, >6%=壓力)
* FOMC 倒數: 19 天 (下次 2026-12-08)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
*今日無標的達標，AI 陣營缺乏黃金坑，維持戰略靜默。*

## 六、建議行動 (Actionable Insights)
1. 💰 **現金/SGOV 過多 3.4%** → 錯失增長機會，考慮分批轉增長倉

=== [END OF MAX DATA PACK v4.1] ===
