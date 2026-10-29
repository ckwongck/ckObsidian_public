---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-10-30 06:00:12 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-10-30 06:00:03

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 0 / USD 67,903
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 678,394 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 331,769 (約 HKD 2,587,795) [報表日 2026-10-28, 落後 2 日 ⚠️ 資料落後; 同步於 2026-10-30T05:50]
  * 現金結餘: HKD 56,457 / USD 5,242
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 91 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 35.79 USD | 21045 USD | 4.9% | 3284 USD | 18.5% | 13.6 | 1.04 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 290.41 USD | 10164 USD | 2.4% | 1734 USD | 20.6% | 21.5 | 0.86 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 334.88 USD | 17079 USD | 4.0% | -1809 USD | -9.6% | 48.5 | 0.75 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 350.707 USD | 19640 USD | 4.6% | 2513 USD | 14.7% | 13.0 | 1.05 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 169.41 USD | 36931 USD | 8.6% | - | - | 32.9 | 0.83 | - | Flex(2026-10-28) |
| IB | PLTR | 227.0 | 131.423413062 USD | 196.81 USD | 44676 USD | 10.4% | - | - | 39.9 | 0.86 | - | Flex(2026-10-28) |
| IB | QQQM | 434.0 | 249.066141779 USD | 298.71 USD | 129640 USD | 30.3% | - | - | 21.5 | 0.86 | - | Flex(2026-10-28) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.7 USD | 38971 USD | 9.1% | - | - | 2.9 | 0.95 | - | Flex(2026-10-28) |
| IB | SPCX | 122.0 | 140.002405574 USD | 145.23 USD | 17718 USD | 4.1% | - | - | 40.2 | 0.64 | - | Flex(2026-10-28) |
| IB | URA | 840.0 | 50.432105573 USD | 36.55 USD | 30702 USD | 7.2% | - | - | 51.7 | 1.11 | - | Flex(2026-10-28) |
| IB | VRT | 85.0 | 289.688176106 USD | 242.94 USD | 20650 USD | 4.8% | - | - | 54.4 | 1.61 | - | Flex(2026-10-28) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.8% | - | - | 58.1 | 0.69 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.1% | - | - | 47.5 | 1.32 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 5.7% | - | - | 21.5 | 0.86 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$428,211**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $389,240 = **90.9%** | 目標 90% | drift +0.9% ✅
  - 防禦 (defense: SGOV+現金): $51,906 = **12.1%** | 目標 10% | drift +2.1% ⚠️ 超配
  - 戶口現金: $12,935

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $143.89 | IV Rank: 40.2 | Vol/30dAvg: 0.64 | 下次財報: -
  * P: 最新價 $137.20 | IV Rank: 84.7 | Vol/30dAvg: 0.36 | 下次財報: -
  * AVGO: 最新價 $345.00 | IV Rank: 48.5 | Vol/30dAvg: 0.75 | 下次財報: -
  * QQQM: 最新價 $294.53 | IV Rank: 21.5 | Vol/30dAvg: 0.86 | 下次財報: -
  * URA: 最新價 $35.72 | IV Rank: 51.7 | Vol/30dAvg: 1.11 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 93.54 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 17.2 | VIX9D (9日短期): 15.87 | VIX9D/VIX Ratio: 0.92 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.14% (信用違約風險, >6%=壓力)
* FOMC 倒數: 39 天 (下次 2026-12-08)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| MU | $934.27 | 75 | 9.9 | 2.76% | 39.9 | 0.82x | -2.85% |
| TSM | $431.81 | 75 | 4.2 | 53.72% | 40.7 | 0.77x | -0.47% |
| MSFT | $530.14 | 65 | 20.6 | 0.42% | 46.3 | 1.74x | +4.20% |
* 數據更新: 2026-10-30 05:33:42 HKT

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀
2. 🎯 **Alpha 機會**: MU (總分 75) — 考慮研究後分批建倉

=== [END OF MAX DATA PACK v4.1] ===
