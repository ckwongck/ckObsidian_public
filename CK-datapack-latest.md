---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-11-13 06:00:47 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-11-13 06:00:38

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 0 / USD 69,467
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 691,764 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 306,904 (約 HKD 2,393,852) [報表日 2026-11-11, 落後 2 日 ⚠️ 資料落後; 同步於 2026-11-13T05:50]
  * 現金結餘: HKD 0 / USD 7,218
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 105 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 35.92 USD | 21121 USD | 5.1% | 3360 USD | 18.9% | 37.5 | 0.81 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 283.59 USD | 9926 USD | 2.4% | 1495 USD | 17.7% | 26.2 | 0.92 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 363.693 USD | 18548 USD | 4.5% | -339 USD | -1.8% | 46.8 | 1.76 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 354.86 USD | 19872 USD | 4.8% | 2746 USD | 16.0% | 17.6 | 0.69 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 162.54 USD | 35434 USD | 8.6% | - | - | 61.1 | 0.43 | - | Flex(2026-11-11) |
| IB | PLTR | 227.0 | 131.423413062 USD | 172.4 USD | 39135 USD | 9.5% | - | - | 41.0 | 0.49 | - | Flex(2026-11-11) |
| IB | QQQM | 434.0 | 249.066141779 USD | 284.23 USD | 123356 USD | 30.1% | - | - | 26.2 | 0.92 | - | Flex(2026-11-11) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.52 USD | 38901 USD | 9.5% | - | - | 3.0 | 0.92 | - | Flex(2026-11-11) |
| IB | SPCX | 122.0 | 140.002405574 USD | 139.75 USD | 17050 USD | 4.2% | - | - | 59.2 | 0.89 | - | Flex(2026-11-11) |
| IB | URA | 840.0 | 50.432105573 USD | 33.64 USD | 28258 USD | 6.9% | - | - | 58.5 | 0.75 | - | Flex(2026-11-11) |
| IB | VRT | 85.0 | 289.688176106 USD | 206.51 USD | 17553 USD | 4.3% | - | - | 57.3 | 0.76 | - | Flex(2026-11-11) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.9% | - | - | 56.9 | 0.81 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.2% | - | - | 49.1 | 0.81 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 6.0% | - | - | 26.2 | 0.92 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$410,148**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $371,247 = **90.5%** | 目標 90% | drift +0.5% ✅
  - 防禦 (defense: SGOV+現金): $46,574 = **11.4%** | 目標 10% | drift +1.4% ⚠️ 超配
  - 戶口現金: $7,673

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $139.94 | IV Rank: 59.2 | Vol/30dAvg: 0.89 | 下次財報: -
  * P: 最新價 $110.10 | IV Rank: 132.2 | Vol/30dAvg: 0.58 | 下次財報: -
  * AVGO: 最新價 $364.36 | IV Rank: 46.8 | Vol/30dAvg: 1.76 | 下次財報: -
  * QQQM: 最新價 $283.39 | IV Rank: 26.2 | Vol/30dAvg: 0.92 | 下次財報: -
  * URA: 最新價 $32.36 | IV Rank: 58.5 | Vol/30dAvg: 0.75 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 98.43 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 18.7 | VIX9D (9日短期): 17.51 | VIX9D/VIX Ratio: 0.94 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.3% (信用違約風險, >6%=壓力)
* FOMC 倒數: 25 天 (下次 2026-12-08)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| FOXA | $65.71 | 75 | 7.2 | 3.21% | 47.8 | 0.76x | +1.22% |
| TSM | $405.49 | 65 | 3.9 | 57.21% | 46.5 | 0.83x | -3.62% |
* 數據更新: 2026-11-13 05:34:17 HKT

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀
2. 🎯 **Alpha 機會**: FOXA (總分 75) — 考慮研究後分批建倉

=== [END OF MAX DATA PACK v4.1] ===
