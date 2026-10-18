---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-10-19 06:00:43 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-10-19 06:00:35

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 0 / USD 66,427
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 666,547 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 315,390 (約 HKD 2,460,041) [報表日 2026-10-16, 落後 3 日 ⚠️ 資料落後; 同步於 2026-10-19T05:50]
  * 現金結餘: HKD -0 / USD 5,244
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 80 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 34.35 USD | 20198 USD | 4.8% | 2437 USD | 13.7% | 15.2 | 1.09 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 292.26 USD | 10229 USD | 2.4% | 1799 USD | 21.3% | 24.4 | 1.42 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 328.75 USD | 16766 USD | 4.0% | -2122 USD | -11.2% | 39.9 | 1.23 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 343.46 USD | 19234 USD | 4.6% | 2107 USD | 12.3% | 25.1 | 1.48 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 169.84 USD | 37025 USD | 8.9% | - | - | 33.9 | 1.12 | - | Flex(2026-10-16) |
| IB | PLTR | 227.0 | 131.423413062 USD | 186.03 USD | 42229 USD | 10.1% | - | - | 54.1 | 1.41 | - | Flex(2026-10-16) |
| IB | QQQM | 434.0 | 249.066141779 USD | 292.26 USD | 126841 USD | 30.4% | - | - | 24.4 | 1.42 | - | Flex(2026-10-16) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.59 USD | 38928 USD | 9.3% | - | - | 2.5 | 1.04 | - | Flex(2026-10-16) |
| IB | SPCX | 122.0 | 140.002405574 USD | 146.03 USD | 17816 USD | 4.3% | - | - | 49.9 | 0.96 | - | Flex(2026-10-16) |
| IB | URA | 840.0 | 50.432105573 USD | 35.43 USD | 29761 USD | 7.1% | - | - | 51.0 | 1.27 | - | Flex(2026-10-16) |
| IB | VRT | 85.0 | 289.688176106 USD | 206.42 USD | 17546 USD | 4.2% | - | - | 65.5 | 1.18 | - | Flex(2026-10-16) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.8% | - | - | 59.6 | 1.06 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.1% | - | - | 54.6 | 1.23 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 5.9% | - | - | 24.4 | 1.42 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$417,568**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $378,639 = **90.7%** | 目標 90% | drift +0.7% ✅
  - 防禦 (defense: SGOV+現金): $44,627 = **10.7%** | 目標 10% | drift +0.7% ✅
  - 戶口現金: $5,699

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $146.03 | IV Rank: 49.9 | Vol/30dAvg: 0.96 | 下次財報: -
  * P: 最新價 $124.01 | IV Rank: 80.6 | Vol/30dAvg: 0.57 | 下次財報: -
  * AVGO: 最新價 $328.75 | IV Rank: 39.9 | Vol/30dAvg: 1.23 | 下次財報: -
  * QQQM: 最新價 $292.26 | IV Rank: 24.4 | Vol/30dAvg: 1.42 | 下次財報: -
  * URA: 最新價 $35.43 | IV Rank: 51.0 | Vol/30dAvg: 1.27 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 101.1 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 19.99 | VIX9D (9日短期): 20.12 | VIX9D/VIX Ratio: 1.01 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.23% (信用違約風險, >6%=壓力)
* FOMC 倒數: 8 天 (下次 2026-10-27)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| TSM | $412.61 | 80 | 3.9 | 56.22% | 31.6 | 1.54x | -5.52% |
| VZ | $44.79 | 75 | 7.4 | 9.39% | 43.5 | 0.81x | -2.76% |
| TXN | $276.48 | 65 | 27.3 | 1.40% | 48.3 | 1.40x | -0.20% |
| ADI | $395.44 | 65 | 28.7 | 2.16% | 50.0 | 1.48x | +1.53% |
* 數據更新: 2026-10-19 05:34:10 HKT

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀
2. 🎯 **Alpha 機會**: TSM (總分 80) — 考慮研究後分批建倉

=== [END OF MAX DATA PACK v4.1] ===
