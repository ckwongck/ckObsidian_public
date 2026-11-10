---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-11-10 09:22:10 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.2] ===
* 數據提取時間 (HKT): 2026-11-10 09:22:01

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.2 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 0 / USD 66,608
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 667,859 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 292,497 (約 HKD 2,281,475) [報表日 2026-11-06, 落後 4 日 ⚠️ 資料落後; 同步於 2026-11-10T05:50]
  * 現金結餘: HKD 0 / USD 7,218
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 102 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.2*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 35.68 USD | 20980 USD | 5.1% | 3219 USD | 18.1% | 19.8 | 1.26 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 279.35 USD | 9777 USD | 2.4% | 1347 USD | 16.0% | 28.9 | 1.24 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 319.4 USD | 16289 USD | 4.0% | -2598 USD | -13.8% | 65.9 | 1.56 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 350.79 USD | 19644 USD | 4.8% | 2518 USD | 14.7% | 27.9 | 1.06 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 160.93 USD | 35083 USD | 8.5% | -7733 USD | -18.1% | 57.2 | 0.68 | - | yf-live |
| IB | PLTR | 227.0 | 131.423413062 USD | 169.20 USD | 38408 USD | 9.3% | 8575 USD | 28.7% | 59.3 | 0.94 | - | yf-live |
| IB | QQQM | 434.0 | 249.066141779 USD | 279.52 USD | 121312 USD | 29.5% | 13217 USD | 12.2% | 28.9 | 1.24 | - | yf-live |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.50 USD | 38894 USD | 9.5% | -71 USD | -0.2% | 4.0 | 1.06 | - | yf-live |
| IB | SPCX | 122.0 | 140.002405574 USD | 142.07 USD | 17333 USD | 4.2% | 252 USD | 1.5% | 73.1 | 0.99 | - | yf-live |
| IB | URA | 840.0 | 50.432105573 USD | 34.34 USD | 28846 USD | 7.0% | -13517 USD | -31.9% | 62.5 | 1.18 | - | yf-live |
| IB | VRT | 85.0 | 289.688176106 USD | 200.47 USD | 17040 USD | 4.1% | -7584 USD | -30.8% | 87.5 | 1.04 | - | yf-live |
| Firstrade | CEG | 29.0 | 272.2 USD | 276.09 USD | 8007 USD | 1.9% | 113 USD | 1.4% | 65.1 | 1.61 | - | yf-live |
| Firstrade | GEV | 9.0 | 945.0 USD | 829.34 USD | 7464 USD | 1.8% | -1041 USD | -12.2% | 69.9 | 1.3 | - | yf-live |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 279.52 USD | 24137 USD | 5.9% | -1717 USD | -6.6% | 28.9 | 1.24 | - | yf-live |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$410,886**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $364,319 = **88.7%** | 目標 90% | drift -1.3% ⚠️ 不足
  - 防禦 (defense: SGOV+現金): $46,567 = **11.3%** | 目標 10% | drift +1.3% ⚠️ 超配
  - 戶口現金: $7,673

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.2*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $142.07 | IV Rank: 73.1 | Vol/30dAvg: 0.99 | 下次財報: -
  * P: 最新價 $102.84 | IV Rank: 100.0 | Vol/30dAvg: 0.67 | 下次財報: -
  * AVGO: 最新價 $319.48 | IV Rank: 65.9 | Vol/30dAvg: 1.56 | 下次財報: -
  * QQQM: 最新價 $279.52 | IV Rank: 28.9 | Vol/30dAvg: 1.24 | 下次財報: -
  * URA: 最新價 $34.34 | IV Rank: 62.5 | Vol/30dAvg: 1.18 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.2 升級*
* MOVE Index: 85.98 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 19.92 | VIX9D (9日短期): 19.88 | VIX9D/VIX Ratio: 1.0 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.42% (信用違約風險, >6%=壓力)
* FOMC 倒數: 28 天 (下次 2026-12-08)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.2 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200 + IT全收/Communication Services排除傳統媒體) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| FOXA | $67.69 | 70 | 7.1 | 3.12% | 51.5 | 1.30x | +4.70% |
* 數據更新: 2026-11-10 05:34:00 HKT

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀
2. 🎯 **Alpha 機會**: FOXA (總分 70) — 考慮研究後分批建倉

=== [END OF MAX DATA PACK v4.1] ===
