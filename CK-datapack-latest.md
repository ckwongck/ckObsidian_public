---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-11-12 06:00:51 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-11-12 06:00:42

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 0 / USD 68,638
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 686,543 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 301,600 (約 HKD 2,352,477) [報表日 2026-11-10, 落後 2 日 ⚠️ 資料落後; 同步於 2026-11-12T05:50]
  * 現金結餘: HKD 0 / USD 7,218
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 104 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 36.03 USD | 21186 USD | 5.2% | 3425 USD | 19.3% | 13.4 | 1.0 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 283.95 USD | 9938 USD | 2.5% | 1508 USD | 17.9% | 24.7 | 0.75 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 348.22 USD | 17759 USD | 4.4% | -1129 USD | -6.0% | 7.2 | 1.33 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 355.84 USD | 19927 USD | 4.9% | 2801 USD | 16.4% | 4.8 | 0.76 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 159.39 USD | 34747 USD | 8.6% | - | - | 38.6 | 0.7 | - | Flex(2026-11-10) |
| IB | PLTR | 227.0 | 131.423413062 USD | 168.82 USD | 38322 USD | 9.5% | - | - | 45.0 | 0.62 | - | Flex(2026-11-10) |
| IB | QQQM | 434.0 | 249.066141779 USD | 277.87 USD | 120596 USD | 29.8% | - | - | 24.7 | 0.75 | - | Flex(2026-11-10) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.53 USD | 38905 USD | 9.6% | - | - | 2.7 | 0.88 | - | Flex(2026-11-10) |
| IB | SPCX | 122.0 | 140.002405574 USD | 143.09 USD | 17457 USD | 4.3% | - | - | 5.2 | 1.06 | - | Flex(2026-11-10) |
| IB | URA | 840.0 | 50.432105573 USD | 33.15 USD | 27846 USD | 6.9% | - | - | 52.3 | 0.61 | - | Flex(2026-11-10) |
| IB | VRT | 85.0 | 289.688176106 USD | 194.22 USD | 16509 USD | 4.1% | - | - | 63.7 | 0.92 | - | Flex(2026-11-10) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.9% | - | - | 50.3 | 0.63 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.2% | - | - | 56.4 | 1.03 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 6.1% | - | - | 24.7 | 0.75 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$404,187**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $365,282 = **90.4%** | 目標 90% | drift +0.4% ✅
  - 防禦 (defense: SGOV+現金): $46,578 = **11.5%** | 目標 10% | drift +1.5% ⚠️ 超配
  - 戶口現金: $7,673

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $139.75 | IV Rank: 5.2 | Vol/30dAvg: 1.06 | 下次財報: -
  * P: 最新價 $106.50 | IV Rank: 128.5 | Vol/30dAvg: 0.98 | 下次財報: -
  * AVGO: 最新價 $345.22 | IV Rank: 7.2 | Vol/30dAvg: 1.33 | 下次財報: -
  * QQQM: 最新價 $284.23 | IV Rank: 24.7 | Vol/30dAvg: 0.75 | 下次財報: -
  * URA: 最新價 $33.64 | IV Rank: 52.3 | Vol/30dAvg: 0.61 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 92.43 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 17.49 | VIX9D (9日短期): 16.04 | VIX9D/VIX Ratio: 0.92 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.34% (信用違約風險, >6%=壓力)
* FOMC 倒數: 26 天 (下次 2026-12-08)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| TSM | $413.35 | 75 | 3.7 | 56.12% | 50.3 | 1.04x | -1.89% |
| FOXA | $67.98 | 70 | 7.1 | 3.10% | 49.3 | 1.21x | +4.77% |
| MU | $811.30 | 65 | 7.2 | 3.17% | 46.6 | 1.17x | -10.29% |
* 數據更新: 2026-11-12 05:34:23 HKT

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀
2. 🎯 **Alpha 機會**: TSM (總分 75) — 考慮研究後分批建倉

=== [END OF MAX DATA PACK v4.1] ===
