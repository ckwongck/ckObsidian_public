---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-10-25 13:13:13 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-10-25 13:13:06

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 0 / USD 66,769
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 668,449 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 320,612 (約 HKD 2,500,771) [報表日 2026-10-23, 落後 2 日 ⚠️ 資料落後; 同步於 2026-10-25T13:00]
  * 現金結餘: HKD 56,457 / USD 5,242
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 86 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 35.27 USD | 20739 USD | 5.0% | 2978 USD | 16.8% | 18.7 | 0.99 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 290.06 USD | 10152 USD | 2.4% | 1722 USD | 20.4% | 26.1 | 0.87 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 321.68 USD | 16406 USD | 3.9% | -2482 USD | -13.1% | 40.6 | 0.68 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 347.725 USD | 19473 USD | 4.7% | 2346 USD | 13.7% | 20.1 | 1.02 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 162.68 USD | 35464 USD | 8.5% | - | - | 35.5 | 0.84 | - | Flex(2026-10-23) |
| IB | PLTR | 227.0 | 131.423413062 USD | 196.75 USD | 44662 USD | 10.7% | - | - | 52.4 | 0.74 | - | Flex(2026-10-23) |
| IB | QQQM | 434.0 | 249.066141779 USD | 290.06 USD | 125886 USD | 30.3% | - | - | 26.1 | 0.87 | - | Flex(2026-10-23) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.66 USD | 38955 USD | 9.4% | - | - | 2.9 | 0.86 | - | Flex(2026-10-23) |
| IB | SPCX | 122.0 | 140.002405574 USD | 147.49 USD | 17994 USD | 4.3% | - | - | 51.0 | 1.1 | - | Flex(2026-10-23) |
| IB | URA | 840.0 | 50.432105573 USD | 34.11 USD | 28652 USD | 6.9% | - | - | 52.1 | 0.81 | - | Flex(2026-10-23) |
| IB | VRT | 85.0 | 289.688176106 USD | 194.32 USD | 16517 USD | 4.0% | - | - | 107.5 | 1.35 | - | Flex(2026-10-23) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.8% | - | - | 52.9 | 0.74 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.1% | - | - | 77.1 | 1.55 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 5.9% | - | - | 26.1 | 0.87 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$415,895**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $376,940 = **90.6%** | 目標 90% | drift +0.6% ✅
  - 防禦 (defense: SGOV+現金): $51,891 = **12.5%** | 目標 10% | drift +2.5% ⚠️ 超配
  - 戶口現金: $12,935

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $147.49 | IV Rank: 51.0 | Vol/30dAvg: 1.1 | 下次財報: -
  * P: 最新價 $123.33 | IV Rank: 81.9 | Vol/30dAvg: 0.31 | 下次財報: -
  * AVGO: 最新價 $321.68 | IV Rank: 40.6 | Vol/30dAvg: 0.68 | 下次財報: -
  * QQQM: 最新價 $290.06 | IV Rank: 26.1 | Vol/30dAvg: 0.87 | 下次財報: -
  * URA: 最新價 $34.11 | IV Rank: 52.1 | Vol/30dAvg: 0.81 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 103.31 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 19.45 | VIX9D (9日短期): 18.7 | VIX9D/VIX Ratio: 0.96 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.4% (信用違約風險, >6%=壓力)
* FOMC 倒數: 2 天 (下次 2026-10-27)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| VZ | $44.66 | 90 | 7.4 | 9.41% | 48.0 | 1.90x | -2.42% |
* 數據更新: 2026-10-25 05:34:05 HKT

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀
2. 🎯 **Alpha 機會**: VZ (總分 90) — 考慮研究後分批建倉
3. 📅 **FOMC 倒數 2 天** → 議息前市場波動加劇，避免重倉操作

=== [END OF MAX DATA PACK v4.1] ===
